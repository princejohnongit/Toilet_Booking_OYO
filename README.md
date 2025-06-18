# ToiletNow 🚽

A full-stack web application for finding and booking nearby toilets, similar to OYO but for public restrooms.

## Features

- 🔍 Find nearby toilets using Google Maps integration
- 📱 User authentication and profile management
- 🎯 Real-time toilet availability checking
- 📅 Booking system with date/time selection
- ⭐ Rating and review system
- 👤 Admin panel for toilet owners

## Tech Stack

### Frontend
- React.js with functional components and hooks
- Tailwind CSS for styling
- Google Maps API integration
- React Router for navigation
- Axios for API calls

### Backend
- Node.js + Express
- MongoDB with Mongoose
- JWT Authentication
- RESTful API architecture

## Project Structure

```
toiletnow/
├── client/                 # Frontend React application
│   ├── public/
│   └── src/
│       ├── components/     # Reusable components
│       ├── pages/         # Page components
│       ├── context/       # React context
│       ├── hooks/         # Custom hooks
│       ├── api/           # API integration
│       └── utils/         # Utility functions
│
└── server/                # Backend Node.js application
    ├── config/           # Configuration files
    ├── controllers/      # Route controllers
    ├── models/          # Mongoose models
    ├── routes/          # API routes
    ├── middleware/      # Custom middleware
    └── utils/           # Utility functions
```

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- MongoDB
- Google Maps API key

### Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/toiletnow.git
cd toiletnow
```

2. Install dependencies
```bash
# Install backend dependencies
cd server
npm install

# Install frontend dependencies
cd ../client
npm install
```

3. Set up environment variables
```bash
# In server directory
cp .env.example .env
# Fill in your environment variables

# In client directory
cp .env.example .env
# Add your Google Maps API key
```

4. Start the development servers
```bash
# Start backend server (from server directory)
npm run dev

# Start frontend server (from client directory)
npm start
```

## Development Plan

1. **Phase 1: Project Setup**
   - Initialize project structure
   - Set up development environment
   - Configure basic dependencies

2. **Phase 2: Backend Development**
   - Set up Express server
   - Create MongoDB schemas
   - Implement authentication
   - Create basic API endpoints

3. **Phase 3: Frontend Development**
   - Set up React application
   - Implement authentication UI
   - Create basic components
   - Integrate Google Maps

4. **Phase 4: Core Features**
   - Implement toilet listing
   - Add booking functionality
   - Create user dashboard
   - Add admin panel

5. **Phase 5: Polish & Testing**
   - Add error handling
   - Implement loading states
   - Add form validation
   - Write tests

## API Endpoints

### Authentication
- POST `/api/auth/register` - Register new user
- POST `/api/auth/login` - User login
- GET `/api/auth/me` - Get current user

### Toilets
- GET `/api/toilets` - List all toilets
- GET `/api/toilets/:id` - Get toilet details
- POST `/api/toilets` - Add new toilet
- PUT `/api/toilets/:id` - Update toilet
- DELETE `/api/toilets/:id` - Delete toilet

### Bookings
- GET `/api/bookings` - List user bookings
- POST `/api/bookings` - Create booking
- PUT `/api/bookings/:id` - Update booking
- DELETE `/api/bookings/:id` - Cancel booking

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details. 
