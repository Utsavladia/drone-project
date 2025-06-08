# Drone Mission Control System

A comprehensive system for managing and controlling drone missions with real-time monitoring and simulation capabilities.

## 🚀 Features

- **Mission Planning**

  - Create and manage drone missions
  - Define flight paths with waypoints
  - Configure mission parameters (altitude, overlap, sensors)
  - Multiple flight patterns (perimeter, crosshatch, custom)

- **Real-time Monitoring**

  - Live drone position tracking
  - Battery level monitoring
  - Mission progress updates
  - Status notifications

- **Mission Control**

  - Start/Pause/Resume missions
  - Emergency abort functionality
  - Mission parameter adjustments
  - Real-time mission status

- **Drone Management**
  - Drone status tracking
  - Battery management
  - Location tracking
  - Maintenance scheduling

## 🛠️ Technology Stack

### Frontend

- React
- TypeScript
- Material-UI
- Redux for state management
- Socket.IO for real-time updates
- Leaflet for map visualization

### Backend

- Node.js
- Express
- TypeScript
- MongoDB
- Socket.IO
- Mongoose

## 📋 Prerequisites

- Node.js (v14 or higher)
- MongoDB
- npm or yarn

## 🚀 Installation

1. Clone the repository:

```bash
git clone [repository-url]
cd drone-project
```

2. Install dependencies:

```bash
# Install backend dependencies
cd backend
npm install

# Install frontend dependencies
cd ../frontend
npm install
```

3. Set up environment variables:

```bash
# Backend (.env)
MONGODB_URI=your_mongodb_uri
PORT=5000
NODE_ENV=development

# Frontend (.env)
REACT_APP_API_URL=http://localhost:5000
REACT_APP_SOCKET_URL=http://localhost:5000
```

4. Start the development servers:

```bash
# Start backend server
cd backend
npm run dev

# Start frontend server
cd frontend
npm start
```

## 📁 Project Structure

```
drone-project/
├── frontend/
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/         # Page components
│   │   ├── services/      # API and socket services
│   │   ├── store/         # Redux store
│   │   ├── types/         # TypeScript interfaces
│   │   └── utils/         # Utility functions
│   └── public/            # Static assets
│
└── backend/
    ├── src/
    │   ├── controllers/   # Request handlers
    │   ├── models/        # Database models
    │   ├── routes/        # API routes
    │   ├── services/      # Business logic
    │   ├── socket/        # Socket.IO handlers
    │   └── types/         # TypeScript interfaces
    └── dist/              # Compiled JavaScript
```

## 🔧 Configuration

### Mission Parameters

- Altitude: 50-200 meters
- Overlap: 50-90%
- Frequency: 1-5 Hz
- Sensors: RGB, Thermal, Multispectral

### Drone Status

- Available
- In-mission
- Charging
- Maintenance

## 📝 API Documentation

### Mission Endpoints

- `POST /api/missions` - Create new mission
- `GET /api/missions` - List all missions
- `GET /api/missions/:id` - Get mission details
- `PUT /api/missions/:id` - Update mission
- `DELETE /api/missions/:id` - Delete mission

### Drone Endpoints

- `GET /api/drones` - List all drones
- `GET /api/drones/available` - List available drones
- `PUT /api/drones/:id` - Update drone status

### Mission Run Endpoints

- `POST /api/mission-runs` - Start mission run
- `GET /api/mission-runs` - List mission runs
- `GET /api/mission-runs/:id` - Get mission run details

## 🔐 Security Considerations

- Input validation for all API endpoints
- Authentication and authorization (to be implemented)
- Secure WebSocket connections
- Data encryption for sensitive information
- Rate limiting for API endpoints

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 🔄 Updates

### Version 1.0.0

- Initial release
- Basic mission planning and execution
- Real-time monitoring
- Drone management

### Version 1.1.0 (Planned)

- Advanced mission patterns
- Enhanced simulation capabilities
- Improved error handling
- Additional sensor support
