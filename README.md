# Discord Clone App README

Welcome to the Discord Clone app! This application is a feature-rich messaging and communication platform that replicates many of the functionalities found in the popular Discord application. It allows users to engage in one-on-one chats, join text channels, voice channels, and video channels, create servers, edit server channels, manage members, and set their roles as moderators or guests. Additionally, user authentication is implemented using Clerk. This README provides an overview of the app's features, technologies used, and deployment details.

## Features

### User Authentication

- The app uses [Clerk](https://docs.clerk.dev/) for user authentication. Users can sign up, log in, and reset their passwords securely.

### Messaging

- **One-on-One Chat**: Users can engage in private one-on-one conversations with their friends by sending text messages.

### Servers and Channels

- **Create Server**: Users can create new servers, each with its own set of text and voice channels.
- **Edit Servers and Channels**: Server owners have the ability to modify server details and channel properties.
- **Text Channels**: Users can join and participate in text-based chat channels within servers.
- **Voice Channels**: Users can join voice channels for real-time audio communication.
- **Video Channels**: Users can join video channels for real-time video communication.

### Role Management

- **Manage Members**: Server owners and moderators can manage server members, including promoting them to moderators or setting them as guests.

### Real-Time Communication

- **Sockets**: Real-time messaging is implemented using sockets, allowing for instant updates in text, voice, and video channels.
- **Polling**: The app includes a fallback mechanism for real-time communication by polling the server every few seconds in case the socket connection is lost.

## Technologies Used

The Discord Clone app is built using modern web development technologies:

- **Next.js**: A popular React framework for building the frontend of the application.
- **Tailwind CSS**: A utility-first CSS framework for designing the user interface.
- **HTML**: Used for structuring the web pages.
- **CSS**: Custom styles to enhance the user experience.
- **PlanetScale**: A SQL database is hosted on PlanetScale to store server and user data.
- **Sockets**: WebSockets are used for real-time communication.
- **Clerk**: Handles user authentication securely.
- **Railway**: The app is deployed on Railway, a platform for hosting web applications.

## Getting Started

Follow these steps to get the Discord Clone app up and running locally:

1. Clone this repository to your local machine.

2. Install the required dependencies:

3. Configure Clerk:
- Set up a Clerk account and configure your Clerk settings in the app.
- Create a `.env.local` file and add your Clerk configuration:
  ```
  CLERK_FRONTEND_API_KEY=your-frontend-api-key
  CLERK_API_KEY=your-api-key
  CLERK_API_URL=https://api.clerk.app
  ```

4. Configure PlanetScale:
- Set up a PlanetScale account and create a SQL database.
- Add your PlanetScale database configuration to `.env.local`:
  ```
  DATABASE_URL=your-database-url
  ```

5. Start the development server:

6. Open your browser and access the app at `http://localhost:3000`.

## Deployment

Follow these steps to deploy the Discord Clone app on Railway:

1. **Create an Account**: If you don't already have one, you can create a Railway account by signing up [here](https://railway.app/).

2. **Connect Your GitHub**: After creating an account, connect your GitHub account to Railway. This allows Railway to access your GitHub repositories for deployment.

3. **Create a New Project**: In your Railway dashboard, create a new project for your Discord Clone app. Give it a name that reflects your project.

4. **Select the GitHub Repository**: Once your project is created, select the GitHub repository where your Discord Clone app project is located. Railway will use this repository for deployment.

5. **Setup Environment Variables**: In your Railway project settings, set up any environment variables required for your app. These might include secret keys, API keys, or other configuration values. Make sure to save these changes.

6. **Deployment Starts Automatically**: After setting up your project and environment variables, Railway will automatically start the deployment process. You can monitor the progress and view deployment logs in your Railway dashboard.

7. **Access Your Deployed App**: Once the deployment is complete, Railway will provide you with a URL where your Discord Clone app is hosted. You can access your app using this URL.

Congratulations! Your Discord Clone app is now deployed and accessible through Railway.

Note: Railway offers a free trial account that allows you to get started with deploying your app. Depending on your project's requirements, you can explore Railway's pricing options for additional features and resources.
