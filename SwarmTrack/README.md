# ⏱️ SwarmTrack

<div align="center">

![SwarmTrack Banner](https://img.shields.io/badge/SwarmTrack-Workforce%20Management-brightgreen?style=for-the-badge)

**Enterprise Time Tracking & Workforce Management Platform**

*Part of Swarm Tech Portfolio by NorthPeak*

[![Status](https://img.shields.io/badge/Status-Beta-green?style=flat-square)](README.md)
[![Tech Stack](https://img.shields.io/badge/Stack-NestJS%20%7C%20PostgreSQL-red?style=flat-square)](README.md)
[![License](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](LICENSE)

[Features](#-core-features) • [Tech Stack](#-technology-stack) • [Setup](#-installation--setup) • [API](#-api-documentation) • [Microservices](#-microservices-architecture)

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Status](#-project-status)
- [Core Features](#-core-features)
- [Technology Stack](#-technology-stack)
- [Microservices Architecture](#-microservices-architecture)
- [Installation & Setup](#-installation--setup)
- [API Documentation](#-api-documentation)
- [Database Schema](#-database-schema)
- [Configuration](#-configuration)
- [Deployment](#-deployment)
- [Troubleshooting](#-troubleshooting)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🌟 Overview

**SwarmTrack** is a comprehensive enterprise-grade time tracking and workforce management solution designed for modern businesses. It combines GPS tracking, facial recognition, automated timesheets, and advanced analytics to provide complete visibility into workforce productivity and attendance.

### Why SwarmTrack?

- **📍 GPS Tracking** - Real-time location tracking for field workers
- **👤 Facial Recognition** - Biometric authentication for clock-in/out
- **⏰ Automated Timesheets** - Eliminate manual timesheet entry
- **💰 Payroll Integration** - Seamless integration with payroll systems
- **📊 Advanced Analytics** - Insights into workforce productivity
- **🔒 Enterprise Security** - Role-based access control and data encryption

### Use Cases

- **Field Service Management** - Track mobile workforce in real-time
- **Construction** - Monitor site attendance and project hours
- **Healthcare** - Manage shift schedules for medical staff
- **Retail** - Track store employee hours and breaks
- **Remote Teams** - Monitor distributed workforce productivity
- **Consulting** - Accurate billable hours tracking

---

## 📊 Project Status

> ✅ **Beta Release** - Auth service production-ready, core features in active development

| Service | Status | Progress | Production Ready |
|---------|--------|----------|------------------|
| Auth Service | ✅ Complete | 100% | ✅ Yes |
| User Service | 🟡 Beta | 85% | ⚠️ Soon |
| Time Tracking Service | 🟡 In Progress | 70% | ❌ No |
| GPS Service | 🟡 In Progress | 60% | ❌ No |
| Facial Recognition | 🔴 Planned | 30% | ❌ No |
| Reporting Service | 🔴 Planned | 20% | ❌ No |
| Payroll Integration | 🔴 Planned | 10% | ❌ No |
| Admin Dashboard | 🟡 In Progress | 50% | ❌ No |

**Latest Update:** January 2025
**Expected Production:** Q3 2025

---

## 🚀 Core Features

### Time Tracking
- **Clock In/Out** - Simple one-tap time tracking
- **Break Management** - Automatic break time calculation
- **Overtime Tracking** - Real-time overtime monitoring
- **Shift Scheduling** - Advanced shift planning and management
- **Multiple Projects** - Track time across different projects
- **Manual Adjustments** - Manager approval for time corrections

### GPS & Location Services
- **Real-time GPS Tracking** - Live location updates
- **Geofencing** - Define virtual boundaries for work sites
- **Route Tracking** - Track employee movement throughout the day
- **Location History** - Historical location playback
- **Offline Mode** - Queue location updates when offline
- **Battery Optimization** - Smart tracking to preserve battery life

### Facial Recognition (Planned)
- **Biometric Authentication** - Prevent buddy punching
- **Liveness Detection** - Ensure authentic user presence
- **Photo Verification** - Capture photo with each clock-in
- **Privacy Compliant** - GDPR and privacy law compliance
- **Mask Detection** - COVID-19 safety compliance

### Automated Timesheets
- **Auto-Generation** - Timesheets created automatically
- **Manager Approval** - Multi-level approval workflows
- **Export Formats** - CSV, Excel, PDF exports
- **Custom Fields** - Add project codes, cost centers, etc.
- **Exception Handling** - Flag anomalies for review

### Reporting & Analytics
- **Real-time Dashboards** - Live workforce metrics
- **Custom Reports** - Build reports with drag-and-drop
- **Productivity Analytics** - Time utilization analysis
- **Cost Analytics** - Labor cost tracking
- **Compliance Reports** - Labor law compliance reporting
- **Export & Scheduling** - Automated report delivery

### Payroll Integration
- **Multiple Providers** - ADP, Gusto, QuickBooks, etc.
- **Automated Sync** - Real-time payroll data synchronization
- **Rate Management** - Multiple pay rates per employee
- **Deductions** - Tax and benefit deductions
- **Direct Deposit** - Bank account integration

### Mobile Applications
- **iOS & Android** - Native mobile apps
- **Offline Support** - Work without internet connection
- **Push Notifications** - Shift reminders and alerts
- **Camera Integration** - Photo capture for verification
- **Biometric Support** - Touch ID / Face ID login

---

## 🛠️ Technology Stack

### Backend Framework
- **NestJS** - Progressive Node.js framework for scalable applications
- **TypeScript** - Type-safe development
- **Express** - Underlying HTTP server
- **Class Validator** - Request validation
- **TypeORM** - Database ORM with TypeScript support

### Databases
- **PostgreSQL 14+** - Primary relational database
  - User data, time entries, schedules
  - ACID compliance for critical data
  - Advanced indexing for performance
- **MongoDB** - Document storage
  - GPS location history
  - Activity logs
  - Unstructured data
- **Redis** - Caching and session management
  - Session storage
  - Real-time data caching
  - Message queuing

### Microservices Communication
- **gRPC** - High-performance RPC framework
- **Redis Pub/Sub** - Event-driven messaging
- **Message Queue** - Bull for background jobs

### Authentication & Security
- **JWT** - JSON Web Tokens for stateless auth
- **Passport.js** - Authentication middleware
- **bcrypt** - Password hashing
- **Helmet** - Security headers
- **Rate Limiting** - API rate limiting

### GPS & Location
- **Google Maps API** - Mapping and geocoding
- **Geofencing Libraries** - Virtual boundary detection
- **GeoJSON** - Location data format

### Monitoring & Logging
- **Winston** - Structured logging
- **Morgan** - HTTP request logging
- **Prometheus** - Metrics collection
- **Grafana** - Metrics visualization

### Development Tools
- **Jest** - Unit and integration testing
- **Supertest** - API endpoint testing
- **ESLint** - Code quality
- **Prettier** - Code formatting
- **Husky** - Git hooks

---

## 🏗️ Microservices Architecture

SwarmTrack follows a microservices architecture for scalability and maintainability.

```
┌─────────────────────────────────────────────────────────────┐
│                     API Gateway (NestJS)                    │
│                    Port: 3000 (HTTP/REST)                   │
└─────────────────────────────────────────────────────────────┘
                            │
        ┌───────────────────┼───────────────────┐
        │                   │                   │
        ▼                   ▼                   ▼
┌───────────────┐   ┌───────────────┐   ┌───────────────┐
│  Auth Service │   │  User Service │   │  Time Service │
│  Port: 3001   │   │  Port: 3002   │   │  Port: 3003   │
│  ✅ Production│   │  🟡 Beta      │   │  🟡 Progress  │
└───────────────┘   └───────────────┘   └───────────────┘
        │                   │                   │
        └───────────────────┼───────────────────┘
                            │
                ┌───────────┼───────────┐
                │           │           │
                ▼           ▼           ▼
        ┌───────────┐ ┌─────────┐ ┌─────────┐
        │PostgreSQL │ │ MongoDB │ │  Redis  │
        │  Port:    │ │ Port:   │ │ Port:   │
        │  5432     │ │ 27017   │ │ 6379    │
        └───────────┘ └─────────┘ └─────────┘

Additional Services (Planned):
┌───────────────┐   ┌───────────────┐   ┌───────────────┐
│  GPS Service  │   │  Face Recog   │   │Report Service │
│  Port: 3004   │   │  Port: 3005   │   │  Port: 3006   │
│  🟡 Progress  │   │  🔴 Planned   │   │  🔴 Planned   │
└───────────────┘   └───────────────┘   └───────────────┘
```

### Service Breakdown

#### 1. Auth Service (✅ Production-Ready)
**Responsibilities:**
- User authentication and authorization
- JWT token generation and validation
- Password management
- Session management
- OAuth integration (Google, Microsoft)

**Endpoints:**
- `POST /auth/register` - User registration
- `POST /auth/login` - User login
- `POST /auth/logout` - User logout
- `POST /auth/refresh` - Token refresh
- `POST /auth/forgot-password` - Password reset

#### 2. User Service (🟡 Beta)
**Responsibilities:**
- User profile management
- Role and permission management
- Organization/company management
- Employee onboarding
- User settings

**Endpoints:**
- `GET /users` - List users
- `GET /users/:id` - Get user details
- `PUT /users/:id` - Update user
- `DELETE /users/:id` - Deactivate user
- `GET /users/:id/permissions` - Get user permissions

#### 3. Time Tracking Service (🟡 In Progress)
**Responsibilities:**
- Clock in/out management
- Time entry CRUD operations
- Break time tracking
- Overtime calculation
- Timesheet generation

**Endpoints:**
- `POST /time/clock-in` - Clock in
- `POST /time/clock-out` - Clock out
- `GET /time/entries` - Get time entries
- `PUT /time/entries/:id` - Update time entry
- `GET /time/timesheets` - Generate timesheet

#### 4. GPS Service (🟡 In Progress)
**Responsibilities:**
- Real-time location tracking
- Geofencing management
- Route tracking
- Location history
- Distance calculation

**Endpoints:**
- `POST /gps/location` - Update location
- `GET /gps/location/:userId` - Get current location
- `GET /gps/history/:userId` - Location history
- `POST /gps/geofence` - Create geofence
- `GET /gps/geofence/:id/status` - Check geofence status

#### 5. Facial Recognition Service (🔴 Planned)
**Responsibilities:**
- Face enrollment
- Face verification
- Liveness detection
- Photo storage
- Anti-spoofing

#### 6. Reporting Service (🔴 Planned)
**Responsibilities:**
- Report generation
- Analytics dashboards
- Data aggregation
- Export functionality
- Scheduled reports

---

## 📦 Installation & Setup

### Prerequisites

```bash
# Required
Node.js v18+ LTS
npm v9+ or yarn v1.22+
PostgreSQL 14+
MongoDB 6+
Redis 7+
Git

# Recommended
Docker & Docker Compose
Postman or similar API testing tool
```

### Method 1: Docker Compose (Recommended)

1. **Navigate to Project Directory**
   ```bash
   cd D:\source\AI\SwarmTrack
   ```

2. **Configure Environment Variables**
   ```bash
   cp .env.example .env
   # Edit .env file with your configuration
   ```

3. **Start All Services**
   ```bash
   docker-compose up -d
   ```

4. **Run Database Migrations**
   ```bash
   docker-compose exec api npm run migration:run
   ```

5. **Seed Initial Data (Optional)**
   ```bash
   docker-compose exec api npm run seed
   ```

6. **Access Services**
   - API Gateway: http://localhost:3000
   - Auth Service: http://localhost:3001
   - User Service: http://localhost:3002
   - Swagger Docs: http://localhost:3000/api/docs

### Method 2: Manual Installation

1. **Clone Repository**
   ```bash
   cd D:\source\AI\SwarmTrack
   ```

2. **Install Dependencies for Each Service**

   ```bash
   # API Gateway
   cd apps/api-gateway
   npm install

   # Auth Service
   cd ../auth-service
   npm install

   # User Service
   cd ../user-service
   npm install

   # Time Service
   cd ../time-service
   npm install
   ```

3. **Setup Databases**

   ```sql
   -- PostgreSQL
   CREATE DATABASE swarmtrack_auth;
   CREATE DATABASE swarmtrack_users;
   CREATE DATABASE swarmtrack_time;

   -- Create database user
   CREATE USER swarmtrack WITH PASSWORD 'your_password';
   GRANT ALL PRIVILEGES ON DATABASE swarmtrack_auth TO swarmtrack;
   GRANT ALL PRIVILEGES ON DATABASE swarmtrack_users TO swarmtrack;
   GRANT ALL PRIVILEGES ON DATABASE swarmtrack_time TO swarmtrack;
   ```

   ```bash
   # MongoDB
   mongo
   use swarmtrack_gps
   db.createUser({
     user: "swarmtrack",
     pwd: "your_password",
     roles: ["readWrite"]
   })
   ```

4. **Configure Environment Variables**

   Create `.env` files in each service directory:

   ```env
   # apps/auth-service/.env
   PORT=3001
   NODE_ENV=development
   DATABASE_URL=postgresql://swarmtrack:password@localhost:5432/swarmtrack_auth
   REDIS_URL=redis://localhost:6379
   JWT_SECRET=your-super-secret-key
   JWT_EXPIRES_IN=7d
   ```

5. **Run Database Migrations**
   ```bash
   cd apps/auth-service
   npm run migration:run

   cd ../user-service
   npm run migration:run

   cd ../time-service
   npm run migration:run
   ```

6. **Start Services**

   ```bash
   # Terminal 1 - Auth Service
   cd apps/auth-service
   npm run start:dev

   # Terminal 2 - User Service
   cd apps/user-service
   npm run start:dev

   # Terminal 3 - Time Service
   cd apps/time-service
   npm run start:dev

   # Terminal 4 - API Gateway
   cd apps/api-gateway
   npm run start:dev
   ```

### Default Credentials

```
Admin User:
Email: admin@swarmtrack.com
Password: [Set during installation]

Manager User:
Email: manager@swarmtrack.com
Password: [Set during installation]

Employee User:
Email: employee@swarmtrack.com
Password: [Set during installation]
```

> ⚠️ **Security Warning:** All passwords must be set during installation process!

---

## 📚 API Documentation

### Authentication

#### Register New User
```http
POST /api/auth/register
Content-Type: application/json

{
  "email": "user@example.com",
  "password": "SecurePass123!",
  "firstName": "John",
  "lastName": "Doe",
  "role": "employee"
}
```

**Response:**
```json
{
  "success": true,
  "data": {
    "user": {
      "id": "uuid",
      "email": "user@example.com",
      "firstName": "John",
      "lastName": "Doe",
      "role": "employee"
    },
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9..."
  }
}
```

#### Login
```http
POST /api/auth/login
Content-Type: application/json

{
  "email": "user@example.com",
  "password": "SecurePass123!"
}
```

### Time Tracking

#### Clock In
```http
POST /api/time/clock-in
Authorization: Bearer {token}
Content-Type: application/json

{
  "location": {
    "latitude": 40.7128,
    "longitude": -74.0060
  },
  "projectId": "project-uuid",
  "notes": "Starting morning shift"
}
```

#### Clock Out
```http
POST /api/time/clock-out
Authorization: Bearer {token}
Content-Type: application/json

{
  "location": {
    "latitude": 40.7128,
    "longitude": -74.0060
  },
  "notes": "Completed tasks"
}
```

#### Get Time Entries
```http
GET /api/time/entries?startDate=2025-01-01&endDate=2025-01-31
Authorization: Bearer {token}
```

### User Management

#### Get All Users (Admin Only)
```http
GET /api/users?page=1&limit=20&role=employee
Authorization: Bearer {token}
```

#### Update User
```http
PUT /api/users/{userId}
Authorization: Bearer {token}
Content-Type: application/json

{
  "firstName": "Jane",
  "phoneNumber": "+1234567890",
  "department": "Engineering"
}
```

### Complete API Documentation

Access interactive Swagger documentation at:
```
http://localhost:3000/api/docs
```

---

## 🗄️ Database Schema

### PostgreSQL Schema (Auth Service)

```sql
-- Users Table
CREATE TABLE users (
  id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
  email VARCHAR(255) UNIQUE NOT NULL,
  password_hash VARCHAR(255) NOT NULL,
  first_name VARCHAR(100) NOT NULL,
  last_name VARCHAR(100) NOT NULL,
  role VARCHAR(50) NOT NULL,
  is_active BOOLEAN DEFAULT true,
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
  updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-- Time Entries Table
CREATE TABLE time_entries (
  id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
  user_id UUID REFERENCES users(id),
  clock_in TIMESTAMP NOT NULL,
  clock_out TIMESTAMP,
  break_duration INTEGER DEFAULT 0,
  total_hours DECIMAL(5,2),
  project_id UUID,
  status VARCHAR(20) DEFAULT 'active',
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-- Geofences Table
CREATE TABLE geofences (
  id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
  name VARCHAR(255) NOT NULL,
  latitude DECIMAL(10,8) NOT NULL,
  longitude DECIMAL(11,8) NOT NULL,
  radius INTEGER NOT NULL,
  organization_id UUID NOT NULL,
  is_active BOOLEAN DEFAULT true
);
```

---

## ⚙️ Configuration

### Environment Variables

```env
# Application
NODE_ENV=production
PORT=3000
API_PREFIX=api

# Database - PostgreSQL
DATABASE_HOST=localhost
DATABASE_PORT=5432
DATABASE_NAME=swarmtrack
DATABASE_USER=swarmtrack
DATABASE_PASSWORD=secure_password

# Database - MongoDB
MONGODB_URI=mongodb://localhost:27017/swarmtrack

# Redis
REDIS_HOST=localhost
REDIS_PORT=6379
REDIS_PASSWORD=

# JWT
JWT_SECRET=your-256-bit-secret
JWT_EXPIRES_IN=7d
JWT_REFRESH_EXPIRES_IN=30d

# Google Maps
GOOGLE_MAPS_API_KEY=your-api-key

# Email (SendGrid)
SENDGRID_API_KEY=SG.xxxxx_xxxxx (Get from SendGrid Dashboard)
FROM_EMAIL=noreply@swarmtrack.com

# AWS S3 (for photo storage)
AWS_ACCESS_KEY_ID=AKIA... (Get from AWS Console)
AWS_SECRET_ACCESS_KEY=wJalrXU... (Get from AWS Console)
AWS_S3_BUCKET=swarmtrack-photos
AWS_REGION=us-east-1
```

---

## 🚀 Deployment

### Docker Production Deployment

```bash
# Build production images
docker-compose -f docker-compose.prod.yml build

# Start services
docker-compose -f docker-compose.prod.yml up -d

# Run migrations
docker-compose exec api npm run migration:run
```

### Traditional VPS Deployment

```bash
# Build applications
npm run build

# Start with PM2
pm2 start ecosystem.config.js

# Save PM2 configuration
pm2 save
pm2 startup
```

---

## 🔧 Troubleshooting

### Database Connection Issues

```bash
# Test PostgreSQL connection
psql -h localhost -U swarmtrack -d swarmtrack_auth

# Test MongoDB connection
mongo mongodb://localhost:27017/swarmtrack_gps
```

### Redis Connection Failed

```bash
# Test Redis
redis-cli ping
# Should return: PONG
```

---

## 🤝 Contributing

Contributions welcome! See [main portfolio README](../README.md) for guidelines.

---

## 📄 License

MIT License - see [LICENSE](../LICENSE) file

Copyright (c) 2024-2025 NorthPeak (northpeak.app)

---

## 🔗 Links

- **Main Portfolio:** [Swarm Tech README](../README.md)
- **Company:** [NorthPeak](https://northpeak.app)
- **Project Location:** `D:\source\AI\SwarmTrack`
- **API Docs:** http://localhost:3000/api/docs
- **Support:** support@northpeak.app

---

<div align="center">

**Part of Swarm Tech Portfolio by NorthPeak**

[northpeak.app](https://northpeak.app) | [support@northpeak.app](mailto:support@northpeak.app)

Built with ❤️ by the NorthPeak Team

[⬆ Back to Top](#-swarmtrack)

</div>
