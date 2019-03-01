# Posts

### Features:

* Auth
  - Register
  - Log in
  - Log out
* Profile
  - View profile
* Post
  - users can add posts
  - users can comment on their own or other people's posts
  - users can give stars (from 1 to 5) on other people's posts
* All Posts (posts from all users)
  - List
  - Filters (by has photo or not)
  - Search (by title and author)
  - Sorting (last modified, last added)
  - Pagination
  - Each post in the list must have:
    * title
    * description
    * photo (if uploaded)
    * all comments count
    * all reviews count (how many people give stars to this post)
    * average of stars
* Single Post View
  - Users can view post details where all comments will be listed. No need for nested comments, one level comments are just fine. Viewer can give stars and/or comment to post in this page.
* Manage own posts
  - List
  - View
  - Create
  - Edit
  - Delete

### Main Models and Basic Fields

* User
  - firstName
  - lastName
  - email
  - password
  - created
  - modified
* Post
  - title
  - description
  - photoUrl
  - created
  - modified
  - stars
* Comment
  - text
  - created
  - modified

Note: here are not all fields and models that is needed for minimal implementation of this description.

### Technologies

Backend:
* React
* React Router
* Apollo Client
* Styled Components
* socket.io-client

Frontend:
* express
* express-graphql
* mongodb (mongoose)
* graphql.js
* jwt (for authorization)
* socket.io

Note: You should use plain graphql.js (not apollo's graphql-tools or other lib on top of graphql.js, just plain graphql.js) to build api and you should use express-graphql to serve graphql api.