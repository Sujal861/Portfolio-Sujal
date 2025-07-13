# Robotics Portfolio Website

## Overview

This is a modern, animated portfolio website for a Robotics Engineer built with React, TypeScript, and Express.js. The application showcases technical skills, projects, and professional experience through an interactive, futuristic-themed interface with smooth animations and responsive design.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript
- **Build Tool**: Vite for development and production builds
- **Styling**: Tailwind CSS with shadcn/ui component library
- **UI Components**: Radix UI primitives for accessibility
- **Animations**: CSS-based animations with custom keyframes
- **State Management**: React Query for server state, React hooks for local state
- **Routing**: Wouter for lightweight client-side routing

### Backend Architecture
- **Runtime**: Node.js with Express.js server
- **Language**: TypeScript with ES modules
- **API Design**: RESTful endpoints for contact form and resume download
- **Development**: Hot module replacement via Vite integration
- **Static Assets**: Served through Express with Vite middleware in development

### Database Layer
- **ORM**: Drizzle ORM with PostgreSQL dialect
- **Database**: PostgreSQL (configured via DATABASE_URL)
- **Schema**: User management with username/password authentication
- **Migrations**: Drizzle Kit for schema migrations
- **Connection**: Neon Database serverless driver

## Key Components

### Portfolio Sections
1. **Hero Section**: Animated introduction with typewriter effect and floating elements
2. **About Section**: Professional summary with profile image and education details
3. **Skills Section**: Interactive skill bars with categorized technical abilities
4. **Projects Section**: Filterable project cards with category-based organization
5. **Experience Section**: Timeline-based work history and certifications
6. **Contact Section**: Form submission with validation and toast notifications

### UI Components
- **Navigation**: Responsive navbar with smooth scrolling
- **Animation System**: Scroll-triggered animations using Intersection Observer
- **Particle Background**: Dynamic particle effects for visual enhancement
- **Responsive Design**: Mobile-first approach with breakpoint-based layouts
- **Toast Notifications**: User feedback system for form submissions

### Technical Features
- **SEO Optimization**: Meta tags, OpenGraph, and Twitter Card support
- **Performance**: Lazy loading, code splitting, and optimized assets
- **Accessibility**: ARIA labels, keyboard navigation, and screen reader support
- **TypeScript**: Full type safety across frontend and backend
- **Custom Hooks**: Reusable logic for mobile detection, scroll animations, and toasts

## Data Flow

1. **Static Content**: Portfolio data stored in TypeScript configuration files
2. **Client Rendering**: React components consume data and render UI
3. **User Interactions**: Form submissions and navigation handled client-side
4. **API Communication**: Contact form data sent to Express backend
5. **Server Processing**: Form validation and response generation
6. **Database Operations**: User management through Drizzle ORM (prepared for future use)

## External Dependencies

### Frontend Libraries
- React ecosystem (React, React DOM, React Query)
- UI components (Radix UI, shadcn/ui)
- Styling (Tailwind CSS, class-variance-authority)
- Utilities (clsx, date-fns, lucide-react icons)

### Backend Dependencies
- Express.js server framework
- Database (Drizzle ORM, Neon Database driver)
- Development tools (tsx, esbuild)
- Session management (connect-pg-simple)

### Build Tools
- Vite for frontend bundling and development
- TypeScript compiler for type checking
- PostCSS for CSS processing
- ESBuild for server-side bundling

## Deployment Strategy

### Development Environment
- Vite development server with HMR
- Express server with middleware integration
- Database migrations via Drizzle Kit
- Replit-specific development tools and banners

### Production Build
1. **Frontend**: Vite builds client assets to `dist/public`
2. **Backend**: ESBuild bundles server code to `dist/index.js`
3. **Database**: Schema pushed to production database
4. **Deployment**: Single Node.js process serving static files and API

### Environment Configuration
- Database connection via `DATABASE_URL` environment variable
- Production detection through `NODE_ENV` variable
- Replit-specific features enabled in development mode
- Build and start scripts for different deployment scenarios

The application follows a modern full-stack architecture with separation of concerns, type safety, and developer experience optimizations while maintaining performance and accessibility standards.