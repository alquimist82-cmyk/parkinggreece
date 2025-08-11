# ParkGreece - Parking Location Finder

## Overview

ParkGreece is a mobile-first web application designed to help users find available parking spots across Greece. The application provides real-time parking availability, pricing information, and navigation assistance for major Greek cities including Athens, Thessaloniki, Patras, and more. Built as a full-stack TypeScript application, it features a React frontend with a Node.js/Express backend and PostgreSQL database for persistent data storage.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
The client is built using **React 18** with **TypeScript** and follows a component-based architecture. Key architectural decisions include:

- **Vite** as the build tool for fast development and optimized production builds
- **Wouter** for lightweight client-side routing instead of React Router
- **TanStack Query** for server state management, caching, and data synchronization
- **Tailwind CSS** with **shadcn/ui** components for consistent, accessible UI design
- **Mobile-first responsive design** optimized for smartphone usage
- **Recharts** for analytics visualization and business intelligence dashboards

The frontend features comprehensive user interfaces including:
- Real-time notifications system with badge indicators
- Multi-language support (English/Greek) with language switcher
- Advanced admin panel with analytics dashboard and location management
- Secure payment processing with Stripe integration
- Interactive user settings with privacy controls

### Backend Architecture  
The server follows a **REST API** pattern built with:

- **Express.js** as the web framework
- **TypeScript** for type safety across the entire stack
- **PostgreSQL database** with Drizzle ORM for production-ready data persistence
- **Comprehensive API endpoints** for bookings, payments, notifications, and administration
- **Shared schema definitions** between client and server using Drizzle ORM types

The backend implements enterprise-level features:
- Booking system with payment processing integration
- Review and rating system for parking locations
- Price alert system with user notifications
- Administrative controls for real-time availability updates
- Email notification system integration ready

### Data Storage Solutions
The application uses **PostgreSQL** as the primary database with:

- **Drizzle ORM** for type-safe database operations and migrations
- **Neon Database** serverless PostgreSQL for cloud hosting
- **Comprehensive relational schema** including users, cities, parking locations, bookings, reviews, price alerts, and notifications
- **UUID-based primary keys** for all entities
- **Database initialization** with Greek city data and parking locations

### Enterprise Features
Production-ready features include:

- **Database-backed storage** replacing in-memory storage for scalability
- **Notification system** with real-time updates and read/unread states
- **Payment processing** simulation ready for Stripe integration
- **Admin dashboard** with analytics, location management, and system controls
- **Multi-language support** targeting Greek market with English fallback

### External Service Integrations
The application integrates with:

- **Leaflet maps** for interactive parking location visualization
- **Font Awesome** icons for consistent UI iconography
- **Google Fonts** (Inter) for typography
- **Replit development tools** for cloud-based development environment

## External Dependencies

### Core Framework Dependencies
- **React 18** with TypeScript for the frontend application
- **Express.js** with TypeScript for the REST API backend
- **Node.js** runtime environment for server execution

### Database and ORM
- **PostgreSQL** database (configured for Neon Database serverless)
- **Drizzle ORM** for type-safe database operations and migrations
- **@neondatabase/serverless** for cloud database connectivity

### Frontend Libraries
- **@tanstack/react-query** for server state management and caching
- **wouter** for lightweight client-side routing
- **@radix-ui** component primitives for accessible UI components
- **tailwindcss** for utility-first CSS framework
- **date-fns** for date manipulation and formatting

### UI and Styling
- **shadcn/ui** component library built on Radix UI primitives
- **class-variance-authority** for component variant management
- **clsx** and **tailwind-merge** for conditional CSS class handling
- **Leaflet** for interactive map visualization

### Development and Build Tools  
- **Vite** for fast development server and optimized production builds
- **TypeScript** compiler for type checking and compilation
- **ESBuild** for server-side bundling in production
- **PostCSS** with **Autoprefixer** for CSS processing

### Cloud Services and Hosting
- **Neon Database** for serverless PostgreSQL hosting
- **Replit** development environment with integrated deployment
- **Environment-based configuration** for database connections and API keys