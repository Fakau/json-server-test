# JSON Server

This project uses a JSON server to simulate a REST API. The server provides endpoints for posts, comments, and profile data.

## Getting Started

### Prerequisites

- Node.js
- JSON Server

### Installation

1. Clone the repository:
    ```sh
    git clone <repository-url>
    cd <repository-directory>
    ```

2. Install JSON Server globally:
    ```sh
    npm install -g json-server
    ```

### Running the Server

1. Start the JSON server:
    ```sh
    json-server --watch data.json
    ```

2. The server will run at `http://localhost:3000`.

### Endpoints

- **Posts**
  - `GET /posts` - Get all posts
  - `GET /posts/:id` - Get a post by ID
  - `POST /posts` - Create a new post
  - `PUT /posts/:id` - Update a post by ID
  - `DELETE /posts/:id` - Delete a post by ID

- **Comments**
  - `GET /comments` - Get all comments
  - `GET /comments/:id` - Get a comment by ID
  - `POST /comments` - Create a new comment
  - `PUT /comments/:id` - Update a comment by ID
  - `DELETE /comments/:id` - Delete a comment by ID

- **Profile**
  - `GET /profile` - Get profile data
  - `PUT /profile` - Update profile data

### Example Data

The `data.json` file contains the following example data:

- **Posts**
  ```json
  [
    { "id": "1", "title": "a title", "views": 100 },
    { "id": "2", "title": "another title", "views": 200 }
  ]
