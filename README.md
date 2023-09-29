
# startup

You can find my detailed notes for this course in [notes.md](https://github.com/minjinnie/startup/blob/7aac121b8b527a36a82899f2dcafdb513bc87cfa/notes.md)

## RoomieMatch: Elevator Pitch
RoomieMatch is a revolutionary platform that simplifies the process of finding compatible roommates. Say goodbye to the stress of endless interviews and incompatible living situations. Our intelligent algorithm considers lifestyle preferences, habits, and personal interests to pair you with the perfect roommate match. Whether you're a student, young professional, or anyone seeking a harmonious living arrangement, RoomieMatch ensures you'll find your ideal cohabitant effortlessly.

## A sketch of application
![IMG_7CEC2F219F15-1](https://github.com/minjinnie/startup/assets/105695935/d09da718-92a0-4214-aa75-afbd2dc48b6c)

## Key Features
- **Smart Matching Algorithm**: Our advanced algorithm analyzes user profiles to suggest roommate matches based on compatibility factors such as lifestyle, cleanliness habits, and social preferences.
- **Real-time Messaging**: Seamlessly communicate with potential roommates within the platform. Get to know each other, discuss living arrangements, and share expectations before committing.
- **User Authentication**: Securely create an account and log in with ease. Your personal information is kept confidential and only shared with potential roommates after mutual interest is established.
- **Persistent Data Storage**: Store user profiles and preferences securely in our database, ensuring seamless access to your information every time you log in.
- **Real-time Updates**: Receive instant notifications when potential matches respond to messages or when new compatible roommates join the platform.

## Technologies

### HTML
- **HTML Structure**: The application employs correct HTML structure with two distinct pages: one for user login and another for roommate voting. Each page is appropriately linked for seamless navigation.

### CSS
- **Styling for Accessibility**: The CSS styling prioritizes accessibility, ensuring that the application is visually appealing on various screen sizes. It incorporates well-considered whitespace, balanced color choices, and high contrast for improved readability.

### JavaScript
- **User Authentication**: JavaScript facilitates the user authentication process. Upon login, users are directed to the voting page. Credentials are securely stored in the database, preventing unauthorized access to voting functionalities.
- **Database Integration**: JavaScript is responsible for retrieving and displaying voting choices from the database. Currently, data is temporarily stored and retrieved from local storage, with plans to transition to database integration in future iterations.
- **Real-time Voting Updates**: A placeholder for WebSocket functionality has been established, using the setInterval function to simulate real-time vote updates. This will be replaced with WebSocket messaging to ensure instantaneous and synchronized voting experiences.
- **Application Logic**: JavaScript logic dynamically updates the highlights and ranking numbers based on user selections, enhancing the interactive nature of the application.

### Backend Service (Node.js/Express)
- **HTTP Service**: A Node.js/Express backend service has been implemented, providing endpoints for user login and vote submission. Static middleware serves frontend components effectively.
- **Database Interaction**: Stubbed endpoints process and relay data to MongoDB Atlas, effectively storing user votes and associated information securely.
- **Third-party Calls (Future Implementation)**: While not yet implemented, provisions have been made to incorporate third-party endpoints for enhanced functionality.

### Database (MongoDB Atlas)
- **Database Creation**: A MongoDB Atlas database has been successfully set up to store user information, voting choices, and associated data.
- **Endpoint Handling**: Endpoints have been established to handle data processing and storage in MongoDB, ensuring seamless integration with the frontend.

### User Authentication and Registration
- **User Registration**: The system allows for user registration, creating new accounts in the database.
- **Existing User Handling**: For returning users, their votes are associated with their existing accounts, maintaining a unified record of their preferences.
- **Credential Management**: MongoDB is employed to securely store user credentials and their respective votes.
- **Functionality Restriction**: Voting functionality is restricted until users have successfully logged in. While this restriction is currently enforced only on the frontend, backend validation will be incorporated in future iterations.

### WebSocket (Real-time Updates)
- **WebSocket Setup**: The backend is configured to listen for WebSocket connections, establishing a robust real-time communication channel.
- **Frontend Integration**: The frontend initiates WebSocket connections, ensuring seamless data exchange between users.
- **Real-time Data Display**: All user votes are dynamically displayed in real-time, demonstrating the successful implementation of WebSocket functionality.

### Vue Implementation (React Replacement)
- **Vue Implementation**: Although the initial requirement was React, Vue has been used due to the developer's extensive expertise. The application is bundled, transpiled, and components are effectively utilized for login, voting list, and vote functionalities. Routing and state management are handled efficiently using Vue's native features.
