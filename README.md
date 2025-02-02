# My Taxi - Ride-Hailing Application

Welcome to My Taxi, a comprehensive ride-hailing application designed to connect passengers with drivers seamlessly. This project is built with a robust backend using Node.js, Express, and MongoDB, and a dynamic frontend using React and Vite.

## Features

- **User and Driver Authentication**: Secure registration and login for both users and drivers.
- **Ride Management**: Create, confirm, start, and end rides with real-time updates.
- **Fare Estimation**: Get accurate fare estimates based on distance and vehicle type.
- **Live Tracking**: Real-time location tracking of drivers.
- **Google Maps Integration**: Address autocomplete, distance, and time calculations using Google Maps API.

## Tech Stack

- **Backend**: Node.js, Express, MongoDB
- **Frontend**: React, Vite, Tailwind CSS
- **Authentication**: JWT (JSON Web Tokens)
- **Real-time Communication**: WebSockets

## Getting Started

### Prerequisites

- Node.js
- npm (Node Package Manager)
- MongoDB

### Installation

1. **Clone the repository**:
    ```sh
    git clone <repository_url>
    cd my_taxi
    ```

2. **Backend Setup**:
    - Navigate to the backend directory:
        ```sh
        cd Backend
        ```
    - Install dependencies:
        ```sh
        npm install
        ```
    - Create a `.env` file in the root directory and add the required environment variables:
        ```properties
        PORT=3000
        DB_CONNECT=<your_mongodb_connection_string>
        JWT_SECRET=<your_jwt_secret>
        GOOGLE_MAPS_API=<your_google_maps_api_key>
        ```

3. **Frontend Setup**:
    - Navigate to the frontend directory:
        ```sh
        cd ../frontend
        ```
    - Install dependencies:
        ```sh
        npm install
        ```

### Running the Application

1. **Start the Backend Server**:
    ```sh
    cd Backend
    npm start
    ```

2. **Start the Frontend Development Server**:
    ```sh
    cd ../frontend
    npm run dev
    ```

Open [http://localhost:3000](http://localhost:3000) to view the application in your browser.

## API Documentation

### User Endpoints

- **Register User**: `POST /users/register`
- **Login User**: `POST /users/login`
- **Get User Profile**: `GET /users/profile`
- **Logout User**: `GET /users/logout`

### Driver Endpoints

- **Register Driver**: `POST /drivers/register`
- **Login Driver**: `POST /drivers/login`
- **Get Driver Profile**: `GET /drivers/profile`
- **Logout Driver**: `GET /drivers/logout`

### Ride Endpoints

- **Create Ride**: `POST /rides/create`
- **Get Fare Estimate**: `GET /rides/get-fare`
- **Confirm Ride**: `POST /rides/confirm`
- **Start Ride**: `GET /rides/start-ride`
- **End Ride**: `POST /rides/end-ride`

### Map Endpoints

- **Get Coordinates**: `GET /maps/get-coordinates`
- **Get Distance and Time**: `GET /maps/get-distance-time`
- **Get Autocomplete Suggestions**: `GET /maps/get-suggestions`

## WebSocket Events

- **Join**: `join`
- **Update Location (Driver)**: `update-location-driver`
- **New Ride**: `new-ride`
- **Ride Confirmed**: `ride-confirmed`
- **Ride Started**: `ride-started`
- **Ride Ended**: `ride-ended`

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License.

## Acknowledgements

- [Node.js](https://nodejs.org/)
- [Express](https://expressjs.com/)
- [MongoDB](https://www.mongodb.com/)
- [React](https://reactjs.org/)
- [Vite](https://vitejs.dev/)
- [Tailwind CSS](https://tailwindcss.com/)
- [Google Maps API](https://developers.google.com/maps)

---

Thank you for checking out My Taxi! If you have any questions or feedback, feel free to reach out.