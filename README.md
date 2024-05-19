# Social Media Backend Task

## Overview

This project is the backend implementation of a social media platform, fulfilling all the requirements outlined in the provided task. It offers functionalities such as user authentication, profile management, content creation, following users, viewing feeds, liking posts, commenting on posts, and more.

## Technologies Used

- Node.js
- Express.js
- GraphQL
- MySQL - Amazon RDS
- JWT (JSON Web Tokens)

## Features

### Authentication

- Users can authenticate themselves using a custom authentication method.
- Upon successful authentication, a JWT (JSON Web Token) is generated and provided to the user for further validation of requests.

### User Management

- Users can create profiles with unique identifiers.
- Profile details include username, email, name, profile picture, cover picture, city, and website.

### Content Management

- Users can create posts containing text and/or media.
- Posts can be liked by other users.
- Users can comment on posts, with options to add, edit, or remove comments.

### Relationship Management

- Users can find and follow other users.
- The content feed is personalized for each user, showing posts from users they follow and their own posts.

### API Endpoints

#### Authentication

- **POST /login**: Endpoint to authenticate users and generate JWT.
- **POST /register**: Endpoint to register new users.

#### User Management

- **GET /user/:userId**: Endpoint to retrieve user profile by user ID.
- **POST /user/search**: Endpoint to search for users by name.
- **POST /user/follow/:userId**: Endpoint to follow another user.

#### Content Management

- **GET /post/:postId**: Endpoint to retrieve details of a single post.
- **GET /posts/feed**: Endpoint to retrieve personalized content feed for the authenticated user.
- **POST /post/create**: Endpoint to create a new post.
- **POST /post/:postId/like**: Endpoint to like a post.
- **POST /post/:postId/comment**: Endpoint to add a comment to a post.

#### Relationship Management

- **GET /relationship/:userId/followers**: Endpoint to retrieve followers of a user.
- **GET /relationship/:userId/following**: Endpoint to retrieve users followed by a user.

### Bonus Features Added in my task

- GraphQL Endpoint: Implementation of all APIs as a GraphQL endpoint for enhanced query flexibility and efficiency.

## Database Design

The database schema is designed to efficiently store user profiles, posts, comments, likes, and user relationships. I used Amazon RDS as a SQL Database  and created required tables in mysql workBench - 
![image](https://github.com/aadarsh-nagrath/assignment/assets/92307537/539dc075-a54e-4dc5-9c11-324652e38a73)


## Conclusion

This project demonstrates a comprehensive backend solution for a social media platform an assignment by [Toddle](https://github.com/toddle-edu), implementing essential features and bonus functionalities. The use of Node.js, Express.js, GraphQL, and MySQL ensures scalability, modularity, and performance. The attention to detail, code readability, and database design reflect a high-quality implementation.
