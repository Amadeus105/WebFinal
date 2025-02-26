Made by Shaikenov Aidyn, Khunakhan Astana IT-2305
# Weather, Movies & Quotes Web Application

A full-stack web application that combines weather information, movie searches, and movie quotes with user authentication and admin capabilities.

## Features

### Weather Dashboard
- Real-time weather information using OpenWeather API
- Interactive map display using Leaflet.js
- 14-day weather forecast
- Search weather by city name
- Detailed weather metrics including temperature, humidity, wind, etc.

### Movies Section
- Search movies using RapidAPI Movies Database
- Display movie posters, titles, release years
- Responsive movie card layout
- Real-time search functionality

### Movie Quotes
- Random Breaking Bad quotes
- Dynamic quote display
- One-click quote refresh

### Admin Panel
- User management (Create, Read, Update, Delete)
- Item management with bilingual support (English/Kazakh)
- Admin-only restricted access
- User activity logging

### Default Admin Account
- Username: `yelarys`
- Password: `admin123`

### User Registration
- Anyone can register for a basic user account
- Passwords are securely hashed using bcrypt
- Automatic login after registration

### Dependencies
```json
{
  "axios": "^1.6.2",
  "express": "^4.18.2",
  "mongoose": "^7.0.0",
  "express-session": "^1.17.3",
  "bcrypt": "^5.1.0",
  "ejs": "^3.1.9",
  "nodemon": "^3.1.9"
}
## Setup Instructions

### Prerequisites
- Python 3.9+
- MongoDB instance
- FastAPI & Dependencies (`pip install -r requirements.txt`)
- Docker (optional)

### Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/Amadeus105/WebFinal
   cd digital-camera-store
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Set up environment variables in `.env` file:
   ```sh
   MONGO_URI="mongodb://localhost:27017/render-fincal"
   SECRET_KEY="your_secret_key"
   ```
4. Run the FastAPI application:
   ```sh
   npm start
   uvicorn main:app --reload
   ```

### Running with Docker
1. Build the Docker image:
   ```sh
   docker build -t camera-store-api .
   ```
2. Run the container:
   ```sh
   docker run -p 8000:8000 camera-store-api
   ```

### API Documentation
After starting the server, API documentation can be accessed at:
- Swagger UI: `http://localhost:3000/docs`
- Redoc: `http://localhost:3000/redoc`

### Testing
Use **Postman** or **cURL** to test endpoints. Ensure you authenticate before accessing restricted routes.

### Future Enhancements
- Implementing a payment gateway.
- Adding search and filtering options for products.


