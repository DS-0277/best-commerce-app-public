# BestCommerceApp

BestCommerceApp is a learning project for a single-store e-commerce platform with a web storefront, a mobile storefront, and one shared backend API. Customers can browse products, search and filter the catalog, manage a cart, complete checkout with a mock payment flow, and review their orders. Administration is web-only for this MVP.

## Live web demo

[bestcommerce-web.vercel.app](https://bestcommerce-web.vercel.app)

## Phase 1 — Product & Technical Design

Phase 1 defines the product goal, customer and administrator roles, MVP scope, functional and non-functional requirements, feature modules, REST API plan, web/mobile/API/database architecture, local and production environments, coding and security standards, and project risks.

The core design decision is a shared REST API: the web and mobile clients use the same customer accounts, catalog, cart, checkout, order, and address rules. Administrator tools remain in the web application for this MVP.

## Phase 2 — Database Design

Phase 2 covers the MVP entities and relationships, normalized PostgreSQL data design, product categories and variants, inventory, customer accounts, addresses, carts, orders, order-item snapshots, and relational constraints. The deployed backend uses PostgreSQL hosted by Supabase.

## Mobile preview

The mobile app uses React Native, Expo SDK 58, Expo Router, and Expo Secure Store. From the mobile project directory, start the LAN preview with `pnpm start`, then scan the generated QR code in Expo Go.

The checked-in QR image below points to the current LAN preview address. It works only while the development server is running on the same local network; regenerate it if the address changes.

![BestCommerce Expo SDK 58 QR code](./docs/mobile-preview/bestcommerce-expo-sdk58-qr.png)

[Download the mobile preview QR PNG](./docs/mobile-preview/bestcommerce-expo-sdk58-qr.png)

The mobile app is for local Expo Go testing and is not published to the Apple App Store or Google Play.
