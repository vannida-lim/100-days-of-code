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

---

## Day 3: June 3, 2020

**Today's Progress**: Implemented `npm sharp` on Tasker's POST /users/me/avatar to allow for server-side resizing and reformatting of avatar images. Implemented `npm @sendgrid/mail` to add email delivery upon user signup and cancellation. Added emails directory with functions and exported functions to creating and deleting user endpoints. Implemented .env variables for security. Used `npm env-cmd --save-dev` to use locally. Added API keys, MongoDB url and JWT secret to .env file. In package.json, updated dev scripts to run .env files before starting up server. Worked with a friend to  `Reverse a Linked List` on Leetcode. 

**Thoughts:** Making good progress with my app. Will deploy the backend API soon. Can't wait to build a frontend for it with React. Reversing a Linked List was difficult to implement. At first I was only getting the last node as the head bc I didn't take an extra step of reassigning the newHead to prev. I solved it iteratively with a while loop. It's difficult for me to think of a recursive solution. The best time complexity I could manage was O(n) linear time due to the while loop. 

**Link to work:** [Repo](https://github.com/vannida-lim/Tasker), [Linked List Reference](https://github.com/vannida-lim/javascript-algorithms/tree/master/src/data-structures/linked-list)

## Day 4: June 4, 2020

**Today's Progress**: Continued to work with Linked Lists. Stepped and drew out each iteration to see the reassignments of prev, head, and newHead so I could understand it better. I have a last round interview later today. 

**Thoughts:** I've been working on my app for a while but only just pushed my code up to github. 

**Link to work:** [Repo](https://github.com/vannida-lim/Tasker)

---