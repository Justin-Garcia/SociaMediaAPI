**Social Media API Readme**

Welcome to the Social Media API! This API allows users to interact with a social media platform by making HTTP requests. Here's how you can use it:

**Endpoints:**

1. **Add Friend:**
   - Endpoint: `/api/users/addfriend`
   - Method: POST
   - Description: Allows users to add friends to their network.
   - Parameters:
     - `userId`: The ID of the user who wants to add a friend.
     - `friendId`: The ID of the friend to be added.
   - Response: Returns a success message if the friend was added successfully.

2. **Leave Comment:**
   - Endpoint: `/api/comments/leave`
   - Method: POST
   - Description: Enables users to leave comments on their friends' posts.
   - Parameters:
     - `userId`: The ID of the user leaving the comment.
     - `friendId`: The ID of the friend whose post the comment is for.
     - `message`: The content of the comment.
   - Response: Returns a success message if the comment was posted successfully.

**Dependencies:**

- **Mongoose:** MongoDB object modeling for Node.js. Used for defining schemas, creating models, and interacting with MongoDB.
- **Express.js:** Web application framework for Node.js. Handles routing and middleware.
- **Node.js:** JavaScript runtime environment. Executes JavaScript code outside of a browser.
- **MongoDB:** NoSQL database. Stores user, friend, and comment data.

**How to Use:**

1. **Set Up MongoDB:** Ensure MongoDB is installed and running on your system.

2. **Install Dependencies:** Run `npm install` to install required Node.js modules.

3. **Start Server:** Run `npm start` to start the Express server.

4. **Make HTTP Requests:** Send POST requests to the specified endpoints with the required parameters to add friends or leave comments.

**Important Notes:**

- Ensure proper authentication and authorization mechanisms are implemented to secure the API.
- Handle errors and edge cases gracefully to provide a smooth user experience.
- Monitor API usage and performance for optimization and scalability.

Enjoy using the Social Media API! If you encounter any issues or have questions, refer to the documentation or seek assistance from the development team.