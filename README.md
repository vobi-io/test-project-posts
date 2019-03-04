# Posts

### Features:

* Auth
  - Register
  - Log in
  - Log out
* Profile
  - View own profile
* Post
  - Users can add posts
  - Users can comment on their own or other people's posts
* All Posts (posts from all users)
  - Listing
  - Search (in title and description)
  - Each post in the list must have:
    * title
    * description
    * link to go single post view
    * all comments count
* Single Post View
  - Users can view post details where all comments will be listed (No need for nested comments, one level comments are just fine)
  - Viewer can add comment to post in this page.
* Manage own posts - CRUD (no need comments here, just basic fields)
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
  - created
  - modified
* Comment
  - text
  - created
  - modified

Note: here are not all fields and models that might be needed for minimal implementation of this description.

### Technologies

Backend:
* express
* express-graphql
* mongodb (mongoose)
* graphql.js
* jwt (for authorization)

Frontend:
* React
* React Router
* Apollo Client
* Styled Components

Note: You should use plain graphql.js (not apollo's graphql-tools or other lib on top of graphql.js, just plain graphql.js) to build api and you should use express-graphql to serve graphql api.
