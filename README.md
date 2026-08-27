# All Store – Multi-Vendor E-Commerce Platform

A full-stack multi-vendor e-commerce platform with three separate applications: a customer-facing storefront, a seller/admin dashboard, and a backend API that powers both.

## Overview

All Store supports multiple independent sellers operating on a shared marketplace, with role-based access separating customers, sellers, and admins. The platform handles product listings, cart and checkout, order management, payments, and seller payouts.

## Architecture

The project is split into three independently deployable parts:

- **`backend/`** — Node.js/Express REST API. Handles authentication, product/order/payment logic, and database access.
- **`frontend/`** — React storefront where customers browse products, manage their cart, and check out.
- **`dashboard/`** — React admin/seller dashboard for managing products, orders, and store settings.

## Tech Stack

- **Frontend:** React, Tailwind CSS
- **Backend:** Node.js, Express
- **Database:** MongoDB (Mongoose)
- **Authentication:** JWT-based role-based access control (RBAC), bcrypt password hashing, HTTP-only cookies
- **Payments:** Stripe (including Stripe Connect for seller payouts)
- **Media storage:** Cloudinary
- **AI integration:** Google Gemini API

## My Role

I worked on this project as a **Cybersecurity Developer and Documentation Specialist**, with a focus on:
- Implementing JWT-based authentication and role-based access control across customer, seller, and admin roles
- Applying secure password handling (bcrypt) and HTTP-only cookie session management
- Documenting system architecture and API behavior

## Getting Started

Each of the three folders (`backend`, `frontend`, `dashboard`) is a separate Node project with its own dependencies.

```bash
# Backend
cd backend
npm install
npm start

# Frontend
cd frontend
npm install
npm start

# Dashboard
cd dashboard
npm install
npm start
```

### Environment Variables

Each folder that needs one expects a `.env` file (not included in this repo) with values such as:

```
MONGO_URI=
JWT_SECRET=
STRIPE_SECRET_KEY=
CLOUDINARY_CLOUD_NAME=
CLOUDINARY_API_KEY=
CLOUDINARY_API_SECRET=
GEMINI_API_KEY=
```

## Status

This was built as a university applied project (2025) and is not in active production use.
