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
