# Wanderlust

Wanderlust is a full-stack web application inspired by Airbnb. It allows users to browse and book listings, as well as hosts to list their properties. The backend is built with Node.js and Express, while MongoDB serves as the database. The project is designed to be secure, user-friendly, and scalable.

Live Link - https://wanderlust-cqmz.onrender.com/listings

## Features

- **User Authentication**: Secure login and registration using Passport.js.
- **Listing Management**: Create, edit, delete, and browse property listings.
- **Reviews**: Users can add and view reviews for listings.
- **Flash Messages**: Provides instant feedback for user actions.
- **Session Management**: Sessions are stored securely in MongoDB using `connect-mongo`.
- **Responsive Views**: Dynamic and responsive front-end using EJS templating.

## Tech Stack

- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Frontend**: EJS templating engine
- **Authentication**: Passport.js
- **Session Management**: `express-session`, `connect-mongo`
- **Additional Libraries**:
  - `method-override` for HTTP verbs
  - `ejs-mate` for EJS layouts
  - `connect-flash` for flash messages
  - `mongoose` for MongoDB object modeling

## Project Structure

```
wanderlust/
├── controllers/      # Controller logic for routes
├── init/             # Initialization scripts
├── models/           # Mongoose schemas and models
├── public/           # Static files (CSS, JS, images)
├── routes/           # Express routes
├── utils/            # Utility functions and classes
├── views/            # EJS templates
├── .gitignore        # Files and directories to be ignored by git
├── app.js            # Main application entry point
├── cloudConfig.js    # Cloud configurations (e.g., image upload)
├── middleware.js     # Custom middleware
├── package.json      # Project dependencies
├── package-lock.json # Exact versions of dependencies
├── schema.js         # Validation schemas
```

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/madhav182004/wanderlust.git
   cd wanderlust
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up the environment:
   - Create a `.env` file in the root directory with the following variables:
     ```
     CLOUD_NAME=YOUR_CLOUD_NAME
     CLOUD_API_KEY=YOUR_CLOUD_API_KEY
     CLOUD_API_SECRET=YOUR_CLOUD_API_SECRET

     ATLASDB_URL=YOUR_ATLASDB_URL

     SECRET=YOUR_SECRET_KEY
     ```

4. Start the development server:
   ```bash
   npm start
   ```

5. Access the application at `http://localhost:3000`.

## Usage

- Register or log in to start using the application.
- Browse listings, leave reviews, and interact with other users.
- Host users can add their own listings.

## Contributing

Contributions are welcome! If you have suggestions for new features or improvements, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments

- Inspired by Airbnb
- Built with 💻 and ☕ by Madhav Mundhra(https://github.com/madhav182004)

## Important Note
Do not commit your `.env` file or expose sensitive credentials publicly. Ensure your `.gitignore` file includes `.env` to prevent accidental uploads.
