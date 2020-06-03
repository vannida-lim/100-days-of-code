# 100 Days Of Code - Log

## Day 1: June 1, 2020

**Today's Progress**: Continuing building my Node and Express Task Manager app.

**Thoughts:** I've been working on my app for a while but only just pushed my code up to github. 

**Link to work:** [Repo](https://github.com/vannida-lim/Tasker)

---

## Day 2: June 2, 2020

**Today's Progress**: Continuing building my Node and Express Task Manager app. I implemented authentication on these tasks endpoints: GET /tasks/:id, PATCH /tasks/:id, DELETE /tasks/:id. I establish a User-Task model relationship and implemented deletion of all user's tasks via userSchema. I updated the userSchema with a timestamp property as a second arg. I setup query endpoints for fetching task data from users like GET /tasks?completed=true, GET /tasks?completed=false, GET /tasks?limit=10&skip=0, GET /tasks?sortBy=createdAt:desc, GET /tasks?sortBy=createdAt:asc. I added npm multer config to handle image and file uploads with validations. I added an 'avatars' property on userSchema to store user avatars. I implemented multer middleware and auth middleware to POST and DELETE /user/me/avatar. I created a route to fetch avatar images GET /users/:id/avatar. I also worked on implementing Singly Linked Lists data structures. 

**Thoughts:** I finally learned about how to wire up relationship association between models via Express and Mongoose. It's not as semantically friendly like with Rails (belongs_to, has_many, has_one etc.) but I think it's quite straight forward. My model relationships looks like this: `User--<Task` where users have many tasks. On my Task model I had to create a property to share the user id and set up the endpoint for authorrized users to that task. There are other built-in Express methods to use such as `populate()` and `execPopulate()` to establish the reference.  

**Link to work:** [Repo](https://github.com/vannida-lim/Tasker)

