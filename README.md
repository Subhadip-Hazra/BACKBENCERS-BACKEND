<h1 align="center">Backbenchers</h1>

<p align="center">
  <img src="https://cdn-icons-png.flaticon.com/512/2040/2040653.png" alt="Backbenchers Logo" width="150">
</p>

<p align="center">
  <strong>Revolutionizing e-learning for college students with Backbenchers!</strong>
</p>

## Table of Contents
- [About](#about)
- [Live Demo](#live-demo)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Dependencies](#dependencies)
- [Development](#development)
- [Contributing](#contributing)
- [Contact](#contact)

## About
Created Backbenchers, an innovative e-learning platform for college students, revolutionizing the way they access educational resources. This platform implements seamless registration, login, and feedback submission features, enhancing user experience and engagement. With a responsive UI and a comprehensive range of subjects and modules tailored to branch and semester, Backbenchers offers detailed notes and engaging video lectures to deliver 90% of the curriculum.

## Live Demo
Explore the live demo: [Backbenchers](https://thanos123456790.github.io/E-learning-platform/)

## Features
- **Seamless Registration and Login**: Easy and secure user registration and login process.
- **Feedback Submission**: Users can submit feedback to improve the platform.
- **Responsive UI**: Designed using HTML, CSS, JavaScript, and Bootstrap for accessibility across devices.
- **Comprehensive Subjects and Modules**: Tailored content for different branches and semesters.
- **Detailed Notes and Video Lectures**: Provides comprehensive understanding and covers 90% of the curriculum.

## Installation
To run this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/thanos123456790/E-learning-platform.git
   ```
2. Navigate to the project directory:
   ```bash
   cd E-learning-platform
   ```
3. Install backend dependencies:
   ```bash
   npm install
   ```
4. Set up environment variables:
   - Create a `.env` file in the root directory.
   - Add your MongoDB URI, Gmail username, and Gmail password in the `.env` file:
     ```env
     MONGO_URI=your_mongodb_uri
     GMAIL_USERNAME=your_gmail_username
     GMAIL_PASSWORD=your_gmail_password
     ```

## Usage
To start the backend server, run:
```bash
npm run dev
```
Visit `http://localhost:5500` in your browser to interact with the backend API.

## API Endpoints
### User Registration
- **Endpoint**: `/register`
- **Method**: `POST`
- **Description**: Registers a new user and sends an OTP for email verification.
- **Request Body**:
  ```json
  {
    "username": "exampleUsername",
    "email": "example@example.com",
    "password": "examplePassword"
  }
  ```

### OTP Verification
- **Endpoint**: `/verify-otp`
- **Method**: `POST`
- **Description**: Verifies the OTP sent to the user's email.
- **Request Body**:
  ```json
  {
    "otp": "123456"
  }
  ```

### Login
- **Endpoint**: `/login`
- **Method**: `POST`
- **Description**: Authenticates a user using email and password.
- **Request Body**:
  ```json
  {
    "email": "example@example.com",
    "password": "examplePassword"
  }
  ```

### Resend OTP
- **Endpoint**: `/resend-otp`
- **Method**: `POST`
- **Description**: Resends the OTP to the user's email.
- **Request Query**:
  ```json
  {
    "email": "example@example.com"
  }
  ```

### Feedback Submission
- **Endpoint**: `/send-feedback`
- **Method**: `POST`
- **Description**: Submits user feedback.
- **Request Body**:
  ```json
  {
    "message": "Your feedback message"
  }
  ```

### Save Rating
- **Endpoint**: `/save-rating`
- **Method**: `POST`
- **Description**: Saves a user's rating for the platform.
- **Request Body**:
  ```json
  {
    "userId": "user_id_here",
    "rating": 5
  }
  ```

## Dependencies
- **express**: "^4.18.2"
- **mongoose**: "^6.3.0"
- **body-parser**: "^1.19.0"
- **cors**: "^2.8.5"
- **dotenv**: "^16.4.1"
- **nodemailer**: "^6.7.2"
- **otp-generator**: "^4.0.2"

## Development
- `npm run dev`: Start the backend development server.
- `npm run build`: Build the project for production.
- `npm run lint`: Lint the project files using ESLint.
- `npm run preview`: Preview the built project locally.

## Contributing
Contributions are welcome! Please refer to the [Contribution Guidelines](CONTRIBUTING.md) for more information.

## Contact
For any inquiries or feedback, feel free to reach out to me:

Name: Subhadip Hazra  
Email: [subhadip.aec.it@gmail.com](mailto:subhadip.aec.it@gmail.com)

