# 🎮 Photo Finder

> **Contact:** muhammed.ali.tuerkmen@gmail.com | [Portfolio](https://tuerkmen.dev)

A competitive real-time multiplayer image guessing game where players race to identify progressively revealed images. Built as a vocational school final project demonstrating full-stack development expertise.

## 🚀 [Live Demo](https://photofinder.tuerkmen.dev/)

---

## 🎯 Project Overview

Photo Finder is a web-based multiplayer game that challenges players to identify images as they're gradually revealed tile-by-tile. Players compete in real-time, submitting guesses through an integrated chat system. The fastest correct answer wins the most points!

### Core Gameplay
- Images are uncovered progressively over 30 seconds (tile-by-tile every 3 seconds)
- Players submit guesses via live chat
- Smart fuzzy matching validates answers (80-100% similarity accepted using Levenshtein distance)
- Points awarded based on speed and accuracy
- Real-time leaderboards and persistent highscore tracking

---

## ✨ Key Features

### 🎲 Game Mechanics
- **Progressive Image Reveal** - Strategic tile-by-tile uncovering system
- **Real-time Multiplayer** - WebSocket-based synchronization for multiple concurrent players
- **Intelligent Answer Validation** - Levenshtein distance algorithm for fuzzy matching
- **Dynamic Scoring System** - Time-based point calculation
- **Live Chat Integration** - Real-time communication and answer submission
- **Persistent Highscores** - All-time leaderboard tracking

### 🔐 Security & Authentication
- **JWT-based Authentication** - Secure stateless session management
- **Role-based Access Control** - Separate permissions for players and administrators
- **Password Encryption** - Industry-standard bcrypt hashing
- **HTTPS/TLS** - Encrypted data transfer
- **Session-based Data Loading** - Optimized security with minimal database queries

### 👨‍💼 Administration Panel
- **User Management** - Create, edit, deactivate, and delete accounts
- **Image Library** - Upload and organize image collections
- **Category Management** - Create themed picture groups
- **Activity Monitoring** - Track user logins and game participation
- **Statistics Dashboard** - Game analytics and user engagement metrics

### 🎨 User Experience
- **Responsive Design** - Optimized for desktop, tablet, and mobile
- **Accessibility** - WCAG-compliant barrier-free design
- **Modern UI/UX** - Clean interface with Bootstrap and PrimeReact components
- **Smooth Animations** - Polished user interactions

---

## 🏗️ Technical Architecture

### Tech Stack

**Frontend**
- React 19.1.1
- TypeScript 5.8.3
- Vite 7.1.2 (Build Tool)
- Bootstrap 5.3.7
- PrimeReact 10.9.7
- Socket.IO Client 4.8.1

**Backend**
- Node.js
- Express 4.18.3
- Socket.IO 4.8.1
- JWT (jsonwebtoken 9.0.2)
- bcrypt 5.1.1

**Database**
- MySQL 8.0

### System Design

Built on the **MVC (Model-View-Controller)** architectural pattern:

- **Model Layer**: TypeScript/JavaScript entity classes (User, Picture, PictureGroup, Highscore)
- **View Layer**: React single-page application with component-based architecture
- **Controller Layer**: RESTful API endpoints and WebSocket event handlers

### Performance Optimizations

- **Session-based Data Loading** - Database information initialized once on login, then dynamically requested per session (reduces database load and improves security)
- **Connection Pooling** - Optimized MySQL connection management (10 concurrent connections)
- **Intelligent Caching** - In-memory caching for frequently accessed data (users, pictures, categories)
- **Efficient Asset Management** - Organized file storage with category-based directory structure
- **Lazy Loading** - Components and assets loaded on-demand

### Database Schema

**Core Tables:**
- `users` - User accounts with authentication credentials and role information
- `pictures` - Image metadata with URLs and category associations
- `picturegroups` - Themed image collections and categories
- `highscores` - Persistent player rankings and scores

**Relationships:**
- User ↔ Highscore (1:1)
- PictureGroup ↔ Picture (1:N)

---

## 🎮 How to Play

1. **Register/Login** - Create an account or sign in with existing credentials
2. **Select Category** - Choose a picture group from the dropdown menu
3. **Join Game** - Click "Play" to enter a game session
4. **Guess Images** - Watch tiles reveal progressively and submit guesses in chat
5. **Compete** - Race against other players for the highest score
6. **View Results** - Check live scoreboard and all-time highscores

---

## 📊 Project Highlights

### Professional Development Practices
- ✅ Comprehensive project documentation (50+ pages)
- ✅ Agile development methodology with sprint planning
- ✅ Version control with Git
- ✅ Code reviews and pair programming
- ✅ Unit and integration testing
- ✅ Security-first architecture
- ✅ Scalable and maintainable codebase

### Technical Achievements
- Real-time bidirectional communication with WebSockets
- Secure authentication and authorization system
- Responsive and accessible user interface
- Optimized database queries and caching strategies
- Production-ready deployment configuration

---


## 📝 License

This project was created as a vocational school examination project in Summer 2025.

---

## 📧 Contact

**Muhammed Ali Türkmen**

- 🌐 Portfolio: [tuerkmen.dev](https://tuerkmen.dev)
- 📧 Email: muhammed.ali.tuerkmen@gmail.com
- 🐙 GitHub: [github.com/muhatrm](https://github.com/muhatrm)

---

**Note:** This application showcases professional software development standards including secure architecture, scalable design patterns, and comprehensive testing procedures. The complete source code is available to potential employers upon request.

