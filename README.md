# Social Media Web Application

## Project Structure

Project Structure
index.js: Entry point of the application, sets up the Express server, and connects to MongoDB.
models/: Contains Mongoose models for User and Tweet.
controllers/: Implements business logic for authentication, users, and tweets.
routes/: Defines API routes for authentication, users, and tweets.
verifyToken.js: Middleware for verifying JWT tokens.
error.js: Error handling utilities.

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
