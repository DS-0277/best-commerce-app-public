# BestCommerceApp

BestCommerceApp is a learning project for a single-store e-commerce platform with a web storefront, a mobile storefront, and a shared backend API.

## 1. MVP Scope & Features

- Customers can create an account, sign in, browse products, view product details, and manage a shopping cart.
- Customers can complete checkout with a mock payment flow, manage account information and saved addresses, and review order history.
- Administrators can manage products, categories, inventory, and order operations through protected administration tools.
- The platform is designed around one shared API so web and mobile clients use consistent customer, catalog, cart, checkout, and order behavior.

## 2. Technology & Deployment

- Backend/API: Node.js, Express.js, TypeScript, REST APIs, and JWT-based authentication.
- Database: PostgreSQL hosted by Supabase.
- Hosting: Vercel for the web frontend, Render for the backend/API, and Supabase for PostgreSQL.
- Web frontend: React, TypeScript, Vite, React Router, and Tailwind CSS.
- Mobile frontend: React Native, Expo SDK 58, Expo Router, and Expo Secure Store.

### Access

#### Live web demo

[bestcommerce-web.vercel.app](https://bestcommerce-web.vercel.app)

#### Mobile preview

Start the mobile project with `pnpm start`, then scan the generated LAN QR code in Expo Go. The checked-in image below is valid only while the development server is running at the matching local-network address; regenerate it if that address changes.

![BestCommerce Expo SDK 58 QR code](./docs/mobile-preview/bestcommerce-expo-sdk58-qr.png)

[Download the mobile preview QR PNG](./docs/mobile-preview/bestcommerce-expo-sdk58-qr.png)

The mobile app is for local Expo Go testing and is not published to the Apple App Store or Google Play.

## Project Status

| Phase | Status |
|---|---|
| Phase 0 - Project Management & Setup | Complete |
| Phase 1 - Product & Technical Design | Complete |
| Phase 2 - Database Design | Complete |
| Phase 3 - Backend Foundation | Complete |
| Phase 4 - Catalog Features with REST APIs | Complete |
| Phase 5 - Cart & Inventory Features with REST APIs | Complete |
| Phase 6 - Checkout, Orders & Payments with REST APIs | Complete |
| Phase 7 - Customer Account & Order History with REST APIs | Complete |
| Phase 8 - Administrator Operations & Authorization | Complete |
| Phase 9 - Web Storefront | Complete |
| Phase 10 - Mobile Storefront | Complete |
| Phase 11 - Quality, Security & Release Testing | Complete |
| Phase 12 - Deployment & Operations | Complete |

# Phase 0 - Project Management & Setup

Main topics:

Skipped (assumed complete):

- Non-Disclosure Agreement
- User Research
- User Personas
- Project Proposal
- Service Agreement
- Project Charter
- Project Plan

Completed setup topics:

- Visual Studio Code installation
- Node.js installation and NVM configuration
- pnpm installation
- Git installation and repository initialization
- PostgreSQL installation
- Expo Go installation
- Monorepo workspace and root-file setup
- ESLint and Prettier installation

# Phase 1 - Product & Technical Design

Main topics:

- Product goal
- Customer and administrator roles
- MVP scope and deferred features
- Functional requirements
- Non-functional requirements
- Feature modules
- REST API plan
- Web, mobile, API, and database architecture
- Local, staging, and production environments
- Coding, security, testing, and Git standards
- Technical decisions and project risks

# Phase 2 - Database Design

Main topics:

- MVP entities
- Entity responsibilities
- Relationships and cardinality
- Attributes and PostgreSQL data types
- Primary and foreign keys
- Unique, value, and relational constraints
- Referential actions
- Database normalization
- Historical order snapshots
- Entity relationship diagram
- Data dictionary

# Phase 3 - Backend Foundation

Main topics:

- API workspace package initialization
- TypeScript configuration and strict checking
- HTTP, REST, JSON, and status codes
- Express server and health endpoint
- Environment variables and secret handling
- Backend folder structure and request flow
- Middleware order
- Request validation with Zod
- Consistent errors and safe logging
- CORS configuration
- PostgreSQL connection and Prisma integration
- Schema, migrations, generated client, and seed data
- Password hashing
- JWT authentication
- Customer registration, login, and current-user endpoint
- Basic authorization
- Type-checking and API verification
- Phase boundary and definition of done

# Phase 4 - Catalog Features with REST APIs

Main topics:

- Public catalog API design
- Complete feature-module structure
- Category listing
- Development catalog seed data
- Product listing, filtering, and pagination metadata
- Product details by slug
- Product variants, images, and available stock
- Multi-option variants for relevant products
- Safe public response shapes
- Catalog endpoint verification
- Postman collection and endpoint verification

# Phase 5 - Cart & Inventory Features with REST APIs

Main topics:

- Customer cart endpoints
- Cart items and quantities
- Inventory availability checks
- Cart ownership checks
- Stock reduction deferred to checkout
- Cart and inventory endpoint verification

# Phase 6 - Checkout, Orders & Payments with REST APIs

Main topics:

- Checkout validation
- Checkout shipping address
- Database transactions
- Order and order-item creation
- Mock payment flow
- Stock reduction after successful checkout
- Checkout and order endpoint verification

# Phase 7 - Customer Account & Order History with REST APIs

Main topics:

- Customer profile endpoint
- Saved addresses
- Customer order history and order details
- Ownership checks for customer data
- Customer endpoint verification

# Phase 8 - Administrator Operations & Authorization

Main topics:

- Role-based authorization
- Administrator-only route protection
- Category and product management
- Inventory management
- Order management
- Administrator endpoint verification

# Phase 9 - Web Storefront

Main topics:

- Web application setup
- API integration
- Public catalog, search suggestions, category filtering, pagination, and product pages
- Warm lifestyle market visual design
- Shared API-served category and product imagery
- Authentication and customer account screens
- Cart, checkout, and saved-address selection
- Administrator screens

# Phase 10 - Mobile Storefront

Main topics:

- Expo mobile application setup
- Shared API integration
- Mobile catalog pagination, authentication, cart, checkout, and saved-address selection
- Warm lifestyle market mobile design, branded navigation, and shared imagery
- Customer order screens
- Mobile testing on Expo Go

# Phase 11 - Quality, Security & Release Testing

Main topics:

- Quality and security test planning
- Build and dependency health
- API, authorization, validation, and checkout testing
- Web and mobile customer-flow testing
- Accessibility, regression, and release-readiness checks

# Phase 12 - Deployment & Operations

Main topics:

- Production environment configuration
- Database migration and backup strategy
- Production catalog data import
- API, web, database, and mobile release deployment
- Production domains, CORS, monitoring, and logs
- Operations and release checklist
