# GitHub OAuth App

This repository demonstrates a simple implementation of OAuth2 using GitHub. The template for this demo is provided by Codecademy. The main code handling the OAuth2 logic is located in the `app.js` file.

## Technologies Used

- JavaScript
- EJS
- CSS

## Features

- GitHub OAuth2 authentication using Passport.js
- Session management with express-session
- EJS templating engine for rendering views

## Getting Started

### Prerequisites

- Node.js
- npm (Node Package Manager)
- GitHub OAuth App credentials (Client ID and Client Secret)

### Setup

1. Clone the repository:

   ```sh
   git clone https://github.com/Muatasim-Aswad/github-oauth-app.git
   cd github-oauth-app
   ```

2. Install dependencies:

   ```sh
   npm install
   ```

3. Create a `.env` file in the root directory and add your GitHub OAuth App credentials and a session secret:

   ```env
   GITHUB_CLIENT_ID=your_github_client_id
   GITHUB_CLIENT_SECRET=your_github_client_secret
   SECRET=your_session_secret
   ```

4. Start the application:

   ```sh
   npm start
   ```

5. Open your browser and navigate to `http://localhost:3000`.

## Project Structure

- `app.js`: Main application file containing the server setup and OAuth2 logic.
- `views/`: Directory containing EJS templates for rendering the web pages.
- `public/`: Directory containing static assets like CSS files.

## Usage

- Visit the home page at `http://localhost:3000` to see the login option.
- Click on "Login with GitHub" to authenticate using your GitHub account.
- After authentication, you will be redirected to the home page with your GitHub profile information.

## Routes

- `/`: Home page.
- `/account`: User account page (requires authentication).
- `/login`: Login page.
- `/logout`: Logout route to end the session.
- `/auth/github`: Route to initiate GitHub authentication.
- `/auth/github/callback`: Callback route for GitHub authentication.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- Template by Codecademy
- OAuth2 authentication with Passport.js

**Note:** Parts of this documentation are auto-generated. If something is unclear or you need further information, don't hesitate to reach out.
