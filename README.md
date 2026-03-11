# CineBook - Movie Ticket Booking System

CineBook is a modern, responsive web application for booking movie tickets. It allows users to browse movies, search for films using the TMDb API, select seats in various theatres across Kerala, and manage bookings through an admin dashboard.

## 🚀 Features

- **Movie Discovery**: Browse popular movies and detailed information.
- **TMDb Integration**: Search for movies globally; results are cached locally in the database.
- **Theatre Selection**: Book tickets in theatres across all 14 districts of Kerala.
- **Seat Booking**: Interactive seat selection with real-time availability checking.
- **Admin Dashboard**: Secure login for admins to view and manage all bookings.
- **Responsive Design**: Premium UI with glassmorphism aesthetics and smooth transitions.

## 🛠️ Technology Stack

- **Backend**: Python with Flask
- **Database**: SQLite3
- **Frontend**: HTML5, CSS3 (Vanilla), Jinja2 Templating
- **API**: TMDb (The Movie Database) API for movie data
- **Server**: Multi-port support (defaulting to 5001)

## 📋 Database Schema

The system uses an SQLite database (`database.db`) with the following tables:
- `movies`: Stores movie details (title, poster, description, etc.).
- `theatres`: List of theatres and their locations.
- `showtimes`: Links movies to theatres with timing and pricing information.
- `bookings`: Records customer details, selected seats, and payment information.

## 🚦 Getting Started

### Prerequisites
- Python 3.x
- `pip` (Python package installer)

### Installation

1. **Clone the repository**:
   ```bash
   git clone <your-repository-url>
   cd python
   ```

2. **Install dependencies**:
   ```bash
   pip install flask requests
   ```

3. **Set up API Key**:
   Set your TMDb API key as an environment variable (optional, mock data used if not provided):
   ```bash
   set TMDB_API_KEY=your_api_key_here
   ```

4. **Run the application**:
   ```bash
   python movie_app.py
   ```
   The app will be available at `http://localhost:5001`.

## 🔐 Admin Access

- **Login URL**: `/admin/login`
- **Default Username**: `admin`
- **Default Password**: `admin123`

---

*Developed with ❤️ for a seamless movie booking experience.*
