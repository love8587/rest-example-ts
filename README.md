# REST API Example

This example shows how to implement a **REST API** using [Express.JS](https://expressjs.com/de/) and Prisma.

## How to use

- Codesandbox URL: [https://codesandbox.io/s/github/prisma-csb/rest-example-ts](https://codesandbox.io/s/github/prisma-csb/rest-example-ts)
- Server endpoint: [https://5yx0y5lljk.sse.codesandbox.io/feed](https://5yx0y5lljk.sse.codesandbox.io/feed)
- Codesandbox ID: `5yx0y5lljk`

## API

#### `GET`

- `/post/:id`: Fetch a single post by its `id`
- `/feed`: Fetch all _published_ posts
- `/filterPosts?searchString={searchString}`: Filter posts by `title` or `content`

#### `POST`

- `/post`: Create a new post
  - Body:
    - `title: String` (required): The title of the post
    - `content: String` (optional): The content of the post
    - `authorEmail: String` (required): The email of the user that creates the post
- `/user`: Create a new user
  - Body:
    - `email: String` (required): The email address of the user
    - `name: String` (optional): The name of the user

#### `PUT`

- `/publish/:id`: Publish a post by its `id`

#### `DELETE`
  
- `/post/:id`: Delete a post by its `id`
