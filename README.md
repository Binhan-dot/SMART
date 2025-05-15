# Device Control App with Firebase

This is a React Native application that allows you to control devices through Firebase Realtime Database.

## Prerequisites

- Node.js (v14 or newer)
- npm or yarn
- React Native development environment set up
- Firebase account

## Setup

1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

3. Configure Firebase:
   - Create a new Firebase project at https://console.firebase.google.com/
   - Enable Realtime Database
   - Get your Firebase configuration
   - Replace the Firebase configuration in `src/config/firebase.js` with your own

4. Start the application:
   ```bash
   # For iOS
   npm run ios
   # or
   yarn ios

   # For Android
   npm run android
   # or
   yarn android
   ```

## Firebase Database Structure

The app expects the following structure in your Firebase Realtime Database:

```json
{
  "devices": {
    "device1": {
      "name": "Living Room Light",
      "status": false,
      "lastUpdated": "2024-01-01T00:00:00.000Z"
    },
    "device2": {
      "name": "Kitchen Light",
      "status": true,
      "lastUpdated": "2024-01-01T00:00:00.000Z"
    }
  }
}
```

## Features

- Real-time device status updates
- Toggle device state (ON/OFF)
- Clean and modern UI
- Responsive design

## Contributing

Feel free to submit issues and enhancement requests. 