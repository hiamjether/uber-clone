

# Uber Clone

This is a fully functional Uber clone application built with React Native for the mobile interface. The app replicates essential Uber features like user authentication, real-time location tracking, ride requests, and simulated payments.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Screenshots](#screenshots)
- [Installation](#installation)
  - [Prerequisites](#prerequisites)
  - [Environment Variables](#environment-variables)
  - [Running the App](#running-the-app)
- [Folder Structure](#folder-structure)
- [Future Improvements](#future-improvements)
- [License](#license)

## Features

- **User Authentication**: Users can register, log in, and manage their profiles.
- **Map and Location Services**: Real-time map integration using the Google Maps API for location selection, route calculations, and ride tracking.
- **Ride Request System**: Users can book rides, view drivers on the map, and track ride progress in real-time.
- **Ride History**: Users can access previous rides with details such as distance, fare, and duration.
- **Simulated Payments**: Demo payment processing using Stripe (optional).

## Technologies Used

- **React Native**: Cross-platform mobile app development.
- **Node.js & Express**: Backend for API services.
- **MongoDB or Firebase**: Database to store user, ride, and payment details.
- **Google Maps API**: Provides map and location services.
- **Socket.io**: Enables real-time updates for ride tracking.
- **Stripe API (optional)**: Simulates the payment process for ride booking.

## Screenshots

> Include screenshots of key app screens like login, map view, ride request, tracking, and ride history.

## Installation

### Prerequisites

- **Node.js** (14 or later)
- **React Native CLI** or **Expo CLI**
- **MongoDB** or **Firebase** for database services
- **Google Cloud Console** API key for Google Maps

### Environment Variables

Create a `.env` file in the root directory to store your keys:

```plaintext
GOOGLE_MAPS_API_KEY=your_google_maps_api_key
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret
STRIPE_SECRET_KEY=your_stripe_secret_key
```

### Running the App

1. **Clone the repository**:

   ```bash
   git clone https://github.com/your-username/uber-clone.git
   cd uber-clone
   ```

2. **Install backend dependencies**:

   ```bash
   cd backend
   npm install
   ```

3. **Start the backend server**:

   ```bash
   npm start
   ```

4. **Install React Native dependencies**:

   ```bash
   cd ../mobile
   npm install
   ```

5. **Run the mobile app**:

   - For **iOS**:

     ```bash
     npx react-native run-ios
     ```

   - For **Android**:

     ```bash
     npx react-native run-android
     ```

   - Alternatively, use **Expo** for easier cross-platform testing:

     ```bash
     expo start
     ```

## Folder Structure

```
uber-clone/
├── backend/                 # Backend server files
│   ├── models/              # Database models (e.g., User, Ride)
│   ├── routes/              # API routes (e.g., auth, rides)
│   ├── config/              # Configuration files
│   └── server.js            # Main server file
├── mobile/                  # React Native app files
│   ├── components/          # Reusable components (e.g., Map, RideCard)
│   ├── screens/             # App screens (e.g., Home, Login, RideHistory)
│   ├── navigation/          # React Navigation setup
│   └── App.js               # Main entry point
└── README.md
```

## Future Improvements

- **Driver Interface**: Add a separate interface for drivers to accept and complete ride requests.
- **Push Notifications**: Notify users about driver arrival and ride status.
- **Enhanced Payment System**: Integrate a real payment processor for production use.
- **Better Error Handling**: Improve error feedback and handling throughout the app.

## License

This project is licensed under the MIT License.
