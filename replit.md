# Azure Palace Hotel Management System

## Overview

Azure Palace Hotel Management System is a full-stack web application for managing hotel operations. It provides a public-facing booking interface for guests and a comprehensive admin dashboard for hotel staff. The system handles room management, guest bookings, analytics, and reporting with support for both English and Arabic languages.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React with TypeScript running on Vite for fast development and builds
- **UI Components**: Shadcn/ui component library built on Radix UI primitives for accessibility
- **Styling**: Tailwind CSS with custom CSS variables for theming
- **State Management**: TanStack Query (React Query) for server state and caching
- **Routing**: Wouter for lightweight client-side routing
- **Internationalization**: Custom language provider supporting English and Arabic with RTL layout

### Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Language**: TypeScript with ES modules
- **Database ORM**: Drizzle ORM for type-safe database operations
- **Authentication**: JWT-based authentication with bcrypt for password hashing
- **API Design**: RESTful API structure with separate admin and public endpoints

### Database Design
- **Database**: PostgreSQL with Neon serverless driver
- **Schema**: Structured with proper relationships between users, rooms, guests, and bookings
- **Types**: Strongly typed with enum constraints for room types, statuses, and booking states
- **Migration**: Drizzle Kit for schema management and migrations

### Key Features
- **Room Management**: CRUD operations for room inventory with status tracking
- **Booking System**: Complete booking workflow from search to confirmation
- **Guest Management**: Guest profiles with booking history and preferences
- **Analytics Dashboard**: Revenue tracking, occupancy rates, and booking statistics
- **Multi-language Support**: English and Arabic with proper RTL layout handling

### Authentication & Authorization
- **Admin Authentication**: JWT tokens for admin dashboard access
- **Password Security**: Bcrypt hashing for secure password storage
- **Role-based Access**: Admin role verification for protected endpoints

### Development & Deployment
- **Build System**: Vite for frontend, esbuild for backend bundling
- **Development**: Hot module replacement and runtime error overlay
- **Environment**: Configured for Replit with specific plugins and cartographer support

## External Dependencies

### Database
- **Neon Database**: Serverless PostgreSQL database with connection pooling
- **Environment**: Requires `DATABASE_URL` environment variable

### Authentication
- **JWT Secret**: Requires `JWT_SECRET` environment variable for token signing

### Frontend Libraries
- **UI Framework**: Radix UI primitives for accessible components
- **Form Handling**: React Hook Form with Zod validation
- **Date Handling**: date-fns for date manipulation
- **Icons**: Lucide React for consistent iconography

### Backend Libraries
- **Database**: @neondatabase/serverless for database connectivity
- **Validation**: Zod for runtime type checking and validation
- **Security**: bcrypt for password hashing, jsonwebtoken for authentication

### Development Tools
- **TypeScript**: Full type safety across the stack
- **ESLint & Prettier**: Code quality and formatting
- **Tailwind CSS**: Utility-first styling with custom design system