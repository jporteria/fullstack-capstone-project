# [GIFTLINK](https://giftlink-xw98.onrender.com/)

This project was built using the MERN stack (MongoDB, Express, React, and Node.js) with JWT-based authentication. The app was designed to demonstrate core web development skills, including user authentication, CRUD operations, containerized deployment using Docker, and a CI/CD (Continuous Integration/Continuous Deployment) pipeline for automating the build and deployment process. However, after evaluating its functionality and feasibility, the project was discontinued as it was deemed not suitable for real-world use.

## Features
- **User Authentication**: Implements JWT (JSON Web Token) for user login and secure authentication.
- **MongoDB**: NoSQL database for storing user data and application information.
- **Express.js**: Backend API for handling user requests and authentication.
- **React.js**: Frontend framework used to build a responsive UI.
- **Node.js**: Backend runtime to execute server-side logic and interact with MongoDB.
- **Dockerized Deployment**: The project was containerized and deployed using Docker for easy setup and environment consistency.

## Setup and Installation

### Prerequisites
Ensure you have the following installed:
- [Node.js](https://nodejs.org/)
- [MongoDB](https://www.mongodb.com/)
- [Docker](https://www.docker.com/)

### Installation Steps

1. Clone the repository:
    ```bash
    git clone https://github.com/jporteria/fullstack-capstone-project.git
    ```

2. Install dependencies for both backend and frontend:
    ```bash
    # Backend
    cd fullstack-capstone-project/giftlink-backend
    npm install

    # Frontend
    cd fullstack-capstone-project/giftlink-frontend
    npm install
    ```

3. Update the environment variables in the .env file with your own/preferred credentials.

4. Start the application by building and running docker image:
    ```bash
    docker build -t <image-name> .
    docker run -d -p <host-port>:<container-port> --name <container-name> <image-name>
    ```

## Challenges & Discontinuation

After building and testing the application, it was determined that the project had several limitations, which made it impractical for real-world use:
- Lack of scalability and complex features required for production-ready apps.
- Usability concerns and limited functionality for users.
- Incomplete error handling and edge-case scenarios in certain modules.

As a result, the decision was made to discontinue the project and focus on more feasible solutions.

## Conclusion

This capstone project served as an excellent learning experience for full-stack development using the MERN stack, containerization with Docker, and implementing secure authentication mechanisms. While the app itself was not deployed in a production environment due to feasibility issues, it showcased the fundamental skills needed for modern web development.

