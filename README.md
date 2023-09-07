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

The app can be deployed to Railway using their platform. Make sure to set up your Railway environment variables and deployment configuration according to your requirements. Refer to the Railway documentation for detailed deployment instructions.


---

Enjoy using the Discord Clone app for your communication needs! If you have any questions or encounter issues, please don't hesitate to reach out to the maintainers or the community for support.
