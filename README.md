# Brian-Smith-VideoCon-Demo
Video Conference Application feature FrontEnd REACT, BackEnd ,NET core
Video Chat Application - VideoApp Component
The VideoApp component is a fundamental part of the Video Chat Application, built using React. It manages the state and behavior of the application related to video chat rooms, user interactions, and room management.

Table of Contents
Introduction
Getting Started
Component Overview
Usage
Prop Types
Introduction
The VideoApp component is designed to facilitate the creation, joining, and management of video chat rooms. It interacts with an external API service and utilizes the @daily-co/daily-js and @daily-co/daily-react-hooks libraries for video conferencing functionality.

Getting Started
To use the VideoApp component, follow these steps:

Make sure you have Node.js and npm (Node Package Manager) installed on your system.

Clone or download the Video Chat Application repository.

Install the necessary dependencies by running the following command in your terminal:

Copy code
npm install
Customize the videoChatService to communicate with your backend API for room creation and management.

Update the currentUser prop with the appropriate user information.

Start your React application by running:

sql
Copy code
npm start
The VideoApp component will handle the rest of the video chat application's functionality.

Component Overview
The VideoApp component performs the following key functions:

Fetches the active room list from the backend API.
Creates new video chat rooms and retrieves room tokens.
Manages the room creation, joining, and leaving process.
Handles the states of the video chat application.
Renders appropriate UI components based on the app's state.
Displays the home screen, video call interface, and hair check.
Usage
The VideoApp component is meant to be integrated into a larger React application. Here's how to use it:

jsx
Copy code
import React from "react";
import VideoApp from "./components/VideoApp"; // Update the path to the VideoApp component
import "./App.css";

function App() {
  const currentUser = {
    id: 1,
    email: "user@example.com",
    name: "John Doe",
  };

  return (
    <div className="App">
      <VideoApp currentUser={currentUser} />
    </div>
  );
}

export default App;
Update the currentUser object with the relevant user information.

Prop Types
The VideoApp component expects the following props:

currentUser (object, required): An object containing user information, including id, email, and name.
Example:

jsx
Copy code
<VideoApp currentUser={currentUser} />
This README provides an overview of the VideoApp component and guides you through its usage in the context of the larger Video Chat Application. For more information on specific implementation details, refer to the component's source code and comments.
