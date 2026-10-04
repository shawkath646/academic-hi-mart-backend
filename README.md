<!-- HEADER SECTION -->
<div align="center">

# HiMart — Backend REST API

**Scalable e-commerce RESTful API service built with Node.js, Express.js, Firebase Firestore, and JWT.**

<!-- BADGES -->
[![Platform](https://img.shields.io/badge/Platform-Cloud%20%26%20Microservices-0A66C2?style=flat-square)](#)
[![Author](https://img.shields.io/badge/Author-Shawkat%20Hossain%20Maruf-black?style=flat-square)](https://shawkath646.dev)
[![Ecosystem](https://img.shields.io/badge/Ecosystem-clouburstlab-2563EB?style=flat-square)](https://clouburstlab.com)
[![Course](https://img.shields.io/badge/Course-Web%20Programming-orange?style=flat-square)](#)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](#-license)
[![Node.js](https://img.shields.io/badge/Node.js-18%2B-339933?style=flat-square&logo=node.js&logoColor=white)](#)

</div>

---

### 📋 Project Overview

| Property | Details |
| :--- | :--- |
| **Author** | [Shawkat Hossain Maruf](https://shawkath646.dev) |
| **Course** | Web Programming |
| **Platform** | REST API / Node.js Backend Service |
| **Period / Timeline** | Spring 2025 (Mar 2025 – May 2025) |
| **Status** | Completed / Academic Project |
| **Primary Stack** | Node.js, Express.js, Firebase Admin (Firestore), JWT, CORS |

---

> [!IMPORTANT]
> **Academic Coursework Notice**  
> This repository houses the server-side REST API for the **HiMart** e-commerce ecosystem, developed as comprehensive coursework for the **Web Programming** course. It provides database access, security middleware, and business logic for the [`academic-hi-mart-frontend`](https://github.com/shawkath646/academic-hi-mart-frontend) client application.

---

## 🎯 Purpose & Problem Statement

### Why It Exists
Modern web applications require stateless, secure backends capable of validating requests, enforcing role-based permissions, and persisting transaction records securely. HiMart Backend provides a clean, modular REST interface that powers product catalogs, authenticated carts, and merchant administration.

### What It Solves
- **Role-Based Authentication:** Protects sensitive routes (such as product creation and seller dashboards) using JSON Web Tokens (JWT).
- **Persistent NoSQL Document Storage:** Leverages Google Firebase Firestore for flexible, high-availability document storage.
- **Cart & Order Isolation:** Guarantees user session isolation so that each customer's cart and order history remain strictly private.

---

## 💡 Key Insights & Architecture

- **Modular Express Routing:** Route endpoints are cleanly separated into dedicated modules (`routes/products.js`, `routes/cart.js`, `routes/seller.js`).
- **Middleware Authentication (`libs/auth.js`):** Intercepts incoming requests, verifies Bearer JWT tokens, and attaches authenticated user profiles to the request context.
- **Firebase Admin Integration (`libs/firebase.js`):** Centralizes Firestore database initialization and document manipulation queries.
- **Cross-Origin Security (CORS):** Fully configured CORS middleware allowing authorized cross-origin requests from the client frontend.

---

## 🛠️ Tech Stack & Dependencies

- **Runtime:** Node.js 18+
- **Web Framework:** Express.js 5.1
- **Database & Storage:** Google Firebase Admin SDK (Firestore & Cloud Storage)
- **Security & Auth:** JSON Web Tokens (`jsonwebtoken`), bcrypt
- **Development Tools:** Nodemon, Dotenv, CORS

---

## 🚀 Getting Started

### Prerequisites
- `Node.js >= 18.x` installed locally.
- A Firebase project with Firestore database enabled.

### Installation & Configuration

```bash
# 1. Clone the repository
git clone https://github.com/shawkath646/academic-hi-mart-backend.git
cd academic-hi-mart-backend

# 2. Install dependencies
npm install

# 3. Environment configuration
# Create a .env file from the provided sample:
cp .env.example .env
```

Define the required environment variables:
```env
PORT=5000
JWT_SECRET="your-secure-jwt-secret-key"
FIREBASE_PROJECT_ID="your-firebase-project-id"
FIREBASE_CLIENT_EMAIL="your-service-account-email"
FIREBASE_PRIVATE_KEY="your-firebase-private-key"
```

```bash
# 4. Start the server in development mode
npm run dev

# 5. Start for production
npm start
```

---

## 🤝 Contributing & Support

Because this repository contains personal university coursework, pull requests adding unrelated code will not be accepted. Issues and discussions are welcome via the [Issue Tracker](https://github.com/shawkath646/academic-hi-mart-backend/issues).

---

## 📄 License

Distributed under the [MIT License](LICENSE). See `LICENSE` for more information.

---

<!-- BRANDING FOOTER -->
<div align="center">
  <sub>Engineered by</sub><br/>
  <strong><a href="https://shawkath646.dev">Shawkat Hossain Maruf</a></strong>
  <br/><br/>
  <sub>A product of</sub><br/>
  <a href="https://clouburstlab.com" target="_blank" rel="noopener noreferrer">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://assets.clouburstlab.com/branding/icon_dark.png">
      <source media="(prefers-color-scheme: light)" srcset="https://assets.clouburstlab.com/branding/icon_light.png">
      <img alt="clouburstlab" src="https://assets.clouburstlab.com/branding/icon_light.png" width="230">
    </picture>
  </a>
</div>
