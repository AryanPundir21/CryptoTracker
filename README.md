# 🪙 CryptoTracker

A full-stack cryptocurrency tracking application that allows users to explore cryptocurrency data, monitor prices, and visualize market trends through an interactive dashboard.

## 🚀 Overview

**CryptoTracker** is a full-stack web application built with React and TypeScript on the frontend and Node.js/Express on the backend.

The application provides an interactive interface for tracking cryptocurrency information and visualizing price-related data using charts and a responsive dashboard.

## ✨ Features

* 📈 Cryptocurrency price tracking
* 📊 Interactive charts and data visualization
* 🔍 Browse and explore cryptocurrency data
* 💻 Responsive and modern user interface
* 🔐 User authentication and session management
* ⚡ REST API powered by Express
* 🗄️ PostgreSQL database integration
* 🧩 Type-safe database operations using Drizzle ORM
* 🎨 Tailwind CSS based UI
* 📱 Responsive dashboard

## 🛠️ Tech Stack

### Frontend

* React
* TypeScript
* Vite
* Tailwind CSS
* React Router
* TanStack React Query
* Recharts
* Framer Motion
* Radix UI
* Lucide React

### Backend

* Node.js
* Express.js
* TypeScript
* WebSockets
* Passport.js
* Express Session

### Database

* PostgreSQL
* Neon Serverless PostgreSQL
* Drizzle ORM
* Drizzle Kit

## 📁 Project Structure

```text
CryptoTracker/
│
├── client/                 # React frontend
│   ├── public/
│   └── src/
│
├── server/                 # Express backend
│   └── index.ts
│
├── shared/                 # Shared types and schemas
│
├── migrations/             # Database migrations
│
├── package.json
├── drizzle.config.ts
├── vite.config.ts
├── tailwind.config.ts
└── tsconfig.json
```

## ⚙️ Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/akshaydagar21/CryptoTracker.git
cd CryptoTracker
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Create a `.env` file in the project root and add the required configuration.

Example:

```env
DATABASE_URL=your_postgresql_connection_string
SESSION_SECRET=your_session_secret
```

> Add any additional environment variables required by your deployment configuration.

### 4. Set up the database

Push the database schema using Drizzle:

```bash
npm run db:push
```

### 5. Start the development server

```bash
npm run dev
```

The development server will start the application in development mode.

## 📦 Available Scripts

```bash
npm run dev       # Start development server
npm run build     # Build the application
npm run start     # Start production server
npm run check     # TypeScript type checking
npm run db:push   # Push database schema
```

## 🧠 Architecture

```text
                    ┌────────────────────┐
                    │    React Client    │
                    │   TypeScript/Vite  │
                    └──────────┬─────────┘
                               │
                               │ HTTP / API
                               ▼
                    ┌────────────────────┐
                    │   Express Server   │
                    │    TypeScript      │
                    └──────────┬─────────┘
                               │
                    ┌──────────┴──────────┐
                    │                     │
                    ▼                     ▼
             ┌──────────────┐      ┌──────────────┐
             │  PostgreSQL  │      │   Sessions   │
             │ + Drizzle    │      │ + Passport   │
             └──────────────┘      └──────────────┘
```

## 📊 Data Visualization

The application uses **Recharts** to present cryptocurrency-related information through interactive charts and visual components.

This makes it easier to understand price movements and market trends rather than relying only on raw numerical data.

## 🔐 Authentication

User authentication and session management are handled on the backend using Passport.js and Express sessions.

Protected application functionality can therefore be associated with authenticated users and persistent sessions.

## 🗄️ Database

The project uses **PostgreSQL** for persistent data storage and **Drizzle ORM** for type-safe database interaction.

Database schema changes can be managed using Drizzle Kit.

## 🔮 Future Improvements

* Real-time cryptocurrency price updates
* Cryptocurrency watchlists
* Portfolio tracking
* Price alerts and notifications
* Historical price analysis
* Advanced technical indicators
* Multiple currency support
* Improved mobile experience
* Production deployment

## 👨‍💻 Author

**Akshay Dagar**

GitHub: [@akshaydagar21](https://github.com/akshaydagar21)

---

⭐ If you find this project useful, consider giving it a star!
