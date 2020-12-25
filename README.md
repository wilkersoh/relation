# Relations

# One To Many
- a user can have many posts, *single post belongTo user*
- a post can have many commets
- a project can have many taks
- a users can have many jobs

In User Model
posts: user has many posts
user->posts: return array of posts
就是說 user可以拿到很多個posts，如果也需要post可以拿到它的user是誰的話，那就要在post model裡 寫他belongTo誰

In Post Model
user: post belongsTo user
post->user: return 

# Many To Many
In Tag Model
- a tag has many post
posts: tag belongsToMany post
tag->posts:  return all post which included the tag['vacation' || 'family']

In Post Model
- a post has many tag
tags: post belongsToMany tag
post->tags: return all tag which belongto the post



| Relations        |      A        |  B    |
|------------------|:-------------:|------:|
| A hasMany B      |               | A_id  |
| B belongsTo A    |               |       | 
| A belongsTo B    |      B_id     |       |
| B hasMany A      |               |       |
| A hasOne B       |               | A_id  |
| B belongsTo A    |               |       |
| A belongsTo B    |      B_id     |       |
| B hasOne A       |               |       |



