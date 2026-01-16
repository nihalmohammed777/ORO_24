
## 🛠️ Installation

1. Install dependencies:
  ```bash
  npm install
  # or
  yarn install
  ```

2. Start the server:
  ```bash
  npm run start
  # or
  yarn start
  ```

## 📁 Project Structure

```
/
├── public/              # Static assets
├── src/
│   ├── components/      # Reusable UI components
│   ├── pages/           # Page components
│   ├── styles/          # Global styles and Tailwind configuration
│   ├── App.jsx          # Main application component
│   ├── main.jsx         # Application entry point
│   └── Routes.jsx       # Application routes
├── index.html           # HTML template
├── package.json         # Project dependencies and scripts
├── vite.config.js       # Vite configuration
```

## 🧩 Adding Routes

To add new routes to the application, update the `Routes.jsx` file:

```jsx
import React from 'react';
import { BrowserRouter as Router, Routes, Route } from 'react-router-dom';

// Import page components
import HomePage from "./pages/HomePage";
import AboutPage from "./pages/AboutPage";

const AppRoutes = () => {
  return (
    <Router>
      <Routes>
        <Route path="/" element={<HomePage />} />
        <Route path="/about" element={<AboutPage />} />
      </Routes>
    </Router>
  );
};

export default AppRoutes;
```

## 🎨 Styling

This project uses Tailwind CSS for styling. The configuration includes:

- Utility-first approach for rapid development
- Custom theme configuration
- Responsive design utilities

## 📦 Deployment

Build the application for production:

```bash
npm run build
```

## 🙏 Acknowledgments

- Built with [Rocket.new](https://rocket.new)
- Powered by React and Vite
- Styled with saSS


# ORO24 Mini Web App

A modern React application for ORO24 facilities management services with login, service categories, and service details.

## Features

- 🔐 **Secure Authentication** with token-based login
- 📱 **Fully Responsive** design for all screen sizes
- ⚡ **Optimized Performance** with lazy loading and code splitting
- 🎨 **Modern UI** matching Figma design specifications
- 🛡️ **Error Handling** with error boundaries and user-friendly messages
- 🔄 **Real-time Updates** with context-based state management

## Tech Stack

- **React 18** with Functional Components & Hooks
- **React Router v6** for navigation
- **Context API** for state management
- **Axios** for API requests with interceptors
- **SASS** for styling
- **Class Variance Authority** for variant management
- **React Helmet Async** for SEO

## Project Structure
src/
├── components/
│ ├── common/ # Reusable layout components
│ └── ui/ # Reusable UI components
├── contexts/ # React Context providers
├── hooks/ # Custom React hooks
├── pages/ # Page components
├── services/ # API services
├── styles/ # Global styles
├── utils/ # Utility functions
└── assets/ # Static assets



## Setup & Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd oro24-app

2.install Dependencies
npm install

4.Start the development server
npm start

5.Build for production
npm run build

-----------------------------------------------------------------
API Integration
The application integrates with four main APIs:

Login API - User authentication

Get Categories - Fetch service categories

Get Services - Fetch services by category

Service Details - Get detailed service information

-----------------------------------------------------------------
Demo Credentials
Email: oro_1993@yopmail.com

Password: *123@Abc

----------------------------------------------------------------
Key Implementation Details

Performance Optimizations
Lazy loading of components
Memoization with React.memo and useMemo
Debounced API calls
Image optimization with lazy loading

Security Features
Token-based authentication
Protected routes
Input validation and sanitization
Secure token storage

Code Quality
Proper TypeScript/PropTypes validation
Error boundaries for crash prevention
Comprehensive error handling
Clean, modular code structure

Deployment
The application is deployed on Vercel/Netlify with automatic CI/CD from the main branch.

Live Demo: [https://monumental-moonbeam-5cf416.netlify.app]
