

Project Structure
  # Social Media Web Application

## Project Structure

1. `index.js`
   - The main entry point of the application responsible for setting up the Express server and connecting to MongoDB.

2. `models/`
   - This directory holds Mongoose models for User and Tweet, facilitating interaction with the MongoDB database.

3. `controllers/`
   - The controllers directory contains modules that implement the business logic for user authentication, user management, and tweet-related actions.

4. `routes/`
   - API routes for authentication, user actions, and tweet actions are defined in this directory.

5. `verifyToken.js`
   - Middleware responsible for verifying JWT tokens, enhancing the application's security.

6. `error.js`
   - A utility module providing error-handling functionalities, improving the application's robustness.


## Features

### User Authentication

- `POST /api/auth/signup`: User registration.
- `POST /api/auth/signin`: User login.

### User Actions

- `GET /api/users/find/:id`: Get user details.
- `PUT /api/users/:id`: Update user details.
- `DELETE /api/users/:id`: Delete user account.
- `PUT /api/users/follow/:id`: Follow a user.
- `PUT /api/users/unfollow/:id`: Unfollow a user.

### Tweet Actions

- `POST /api/tweets`: Create a tweet.
- `DELETE /api/tweets/:id`: Delete a tweet.
- `PUT /api/tweets/:id/like`: Like or dislike a tweet.
- `GET /api/tweets/timeline/:id`: Get all timeline tweets.
- `GET /api/tweets/user/all/:id`: Get user tweets.
- `GET /api/tweets/explore`: Get explore tweets.

## Middleware

- **verifyToken**: Middleware to verify JWT tokens.

## Error Handling

The application includes a simple error handling mechanism with custom error messages.

## Dependencies

- `express`: Web framework for Node.js.
- `mongoose`: MongoDB object modeling tool.
- `bcryptjs`: Password hashing library.
- `jsonwebtoken`: JSON Web Token library.
- `dotenv`: Environment variable loader.

## Contribution

Feel free to contribute to this project by submitting issues or pull requests. Your contributions are highly appreciated!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
