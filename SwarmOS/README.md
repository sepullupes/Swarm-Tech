# 🌐 SwarmOS

<div align="center">

![SwarmOS Banner](https://img.shields.io/badge/SwarmOS-Web%20Desktop%20OS-blue?style=for-the-badge)

**Revolutionary Web-Based Desktop Operating System**

*Part of Swarm Tech Portfolio by NorthPeak*

[![Status](https://img.shields.io/badge/Status-Development%2040%25-yellow?style=flat-square)](README.md)
[![Tech Stack](https://img.shields.io/badge/Stack-Angular%2018%2B-red?style=flat-square)](README.md)
[![License](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)](LICENSE)

[Features](#-core-features) • [Tech Stack](#-technology-stack) • [Setup](#-installation--setup) • [Architecture](#-architecture) • [Roadmap](#-development-roadmap)

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Status](#-project-status)
- [Core Features](#-core-features)
- [Technology Stack](#-technology-stack)
- [Architecture](#-architecture)
- [Installation & Setup](#-installation--setup)
- [Project Structure](#-project-structure)
- [Development Roadmap](#-development-roadmap)
- [Screenshots](#-screenshots)
- [API Documentation](#-api-documentation)
- [Troubleshooting](#-troubleshooting)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🌟 Overview

**SwarmOS** is a revolutionary web-based desktop operating system that brings the familiar desktop experience directly to your browser. Built with modern web technologies, SwarmOS provides a complete desktop environment with window management, application ecosystem, file system, and multi-user capabilities - all accessible from any device with a web browser.

### Why SwarmOS?

- **🌍 Access Anywhere** - Your desktop environment accessible from any device
- **💾 Cloud-Native** - Files and settings automatically synced to the cloud
- **🔒 Secure** - Enterprise-grade security with user authentication and permissions
- **🎨 Customizable** - Themes, widgets, and personalization options
- **📱 Responsive** - Works seamlessly on desktop, tablet, and mobile devices

### Use Cases

- **Remote Work** - Access your work environment from anywhere
- **Education** - Provide students with consistent computing environments
- **Enterprise** - Deploy standardized desktop experiences across organizations
- **Development** - Cloud-based development environments
- **Kiosks** - Public computing terminals with restricted access

---

## 📊 Project Status

> ⚠️ **Work in Progress** - SwarmOS is currently under active development (40% complete)

| Component | Status | Progress |
|-----------|--------|----------|
| Window Management | ✅ Complete | 100% |
| Taskbar | ✅ Complete | 100% |
| Start Menu | ✅ Complete | 100% |
| File System | 🟡 In Progress | 60% |
| App Ecosystem | 🟡 In Progress | 30% |
| User Authentication | 🟡 In Progress | 50% |
| Settings Panel | 🔴 Planned | 10% |
| Theme System | 🟡 In Progress | 40% |
| Multi-User Support | 🔴 Planned | 20% |

**Latest Update:** January 2025
**Expected Beta:** Q2 2025
**Production Release:** Q4 2025

---

## 🚀 Core Features

### Window Management System
- **Multiple Windows** - Open and manage multiple application windows simultaneously
- **Drag & Drop** - Intuitive window positioning and resizing
- **Minimize/Maximize/Close** - Full window controls
- **Focus Management** - Automatic focus handling and z-index management
- **Window Snapping** - Snap windows to screen edges for organized workspace

### Desktop Environment
- **Taskbar** - Windows-style taskbar with running application indicators
- **Start Menu** - Application launcher with search functionality
- **Desktop Icons** - Quick access to frequently used applications
- **System Tray** - System notifications and quick settings
- **Context Menus** - Right-click context menus throughout the system

### Application Ecosystem
- **Built-in Apps** - File Manager, Text Editor, Calculator, Terminal, Browser
- **App Store** (Planned) - Download and install third-party applications
- **Multi-Instance** - Run multiple instances of the same application
- **App Permissions** - Granular permission system for security

### File System
- **Virtual File System** - Complete file and folder hierarchy
- **File Operations** - Create, read, update, delete, copy, move files
- **File Types** - Support for documents, images, videos, and more
- **Cloud Storage** - Files stored in MongoDB GridFS
- **File Sharing** - Share files with other users (planned)

### User Management
- **Multi-User Support** - Multiple user accounts with individual settings
- **Authentication** - Secure login with JWT tokens
- **User Profiles** - Customizable user profiles and avatars
- **Permissions** - Role-based access control (RBAC)
- **Session Management** - Handle multiple concurrent sessions

### Customization
- **Themes** - Light, Dark, and custom theme support
- **Wallpapers** - Custom desktop backgrounds
- **Icon Packs** - Different icon sets for applications
- **Widgets** - Desktop widgets for quick information
- **Layouts** - Save and restore desktop layouts

### Real-time Features
- **Live Updates** - Real-time synchronization using Socket.io
- **Notifications** - System-wide notification system
- **Presence** - See which users are online
- **Collaboration** - Shared workspaces (planned)

---

## 🛠️ Technology Stack

### Frontend
- **Angular 18+** - Modern TypeScript framework for complex applications
- **RxJS** - Reactive programming for async operations
- **Angular Material** - UI component library
- **SCSS** - Advanced styling with variables and mixins
- **TypeScript** - Type-safe JavaScript development

### Backend
- **Node.js** - JavaScript runtime environment
- **Express.js** - Fast, minimalist web framework
- **Socket.io** - Real-time bidirectional event-based communication
- **JWT** - JSON Web Tokens for authentication
- **Multer** - Multipart/form-data file upload handling

### Database
- **MongoDB** - NoSQL database for flexible data models
- **GridFS** - MongoDB file storage system for large files
- **Mongoose** - MongoDB object modeling for Node.js

### Additional Tools
- **Webpack** - Module bundler
- **ESLint** - Code quality and consistency
- **Prettier** - Code formatting
- **Jest** - Unit testing framework
- **Cypress** - End-to-end testing

### Infrastructure
- **Docker** - Containerization for consistent environments
- **Nginx** - Reverse proxy and static file serving
- **PM2** - Production process manager for Node.js

---

## 🏗️ Architecture

### System Architecture

```
┌─────────────────────────────────────────────────────────┐
│                    SwarmOS Frontend                     │
│  ┌──────────────────────────────────────────────────┐  │
│  │  Angular 18+ Application                         │  │
│  │  ┌─────────────┐ ┌─────────────┐ ┌────────────┐ │  │
│  │  │  Window     │ │   Desktop   │ │  Taskbar   │ │  │
│  │  │  Manager    │ │  Controller │ │  Service   │ │  │
│  │  └─────────────┘ └─────────────┘ └────────────┘ │  │
│  │  ┌─────────────┐ ┌─────────────┐ ┌────────────┐ │  │
│  │  │  File       │ │    App      │ │   User     │ │  │
│  │  │  System     │ │  Launcher   │ │   Auth     │ │  │
│  │  └─────────────┘ └─────────────┘ └────────────┘ │  │
│  └──────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────┘
                            │
                            │ HTTP/WebSocket
                            ▼
┌─────────────────────────────────────────────────────────┐
│                    SwarmOS Backend                      │
│  ┌──────────────────────────────────────────────────┐  │
│  │  Express.js + Socket.io Server                   │  │
│  │  ┌─────────────┐ ┌─────────────┐ ┌────────────┐ │  │
│  │  │   Auth      │ │   File      │ │   User     │ │  │
│  │  │   API       │ │   API       │ │   API      │ │  │
│  │  └─────────────┘ └─────────────┘ └────────────┘ │  │
│  │  ┌─────────────┐ ┌─────────────┐ ┌────────────┐ │  │
│  │  │   Socket    │ │  Session    │ │   App      │ │  │
│  │  │  Handlers   │ │  Manager    │ │   Manager  │ │  │
│  │  └─────────────┘ └─────────────┘ └────────────┘ │  │
│  └──────────────────────────────────────────────────┘  │
└─────────────────────────────────────────────────────────┘
                            │
                            ▼
┌─────────────────────────────────────────────────────────┐
│                    Data Layer                           │
│  ┌──────────────────┐      ┌───────────────────────┐   │
│  │   MongoDB        │      │   MongoDB GridFS      │   │
│  │   - Users        │      │   - File Storage      │   │
│  │   - Sessions     │      │   - Large Files       │   │
│  │   - Settings     │      │   - User Files        │   │
│  │   - Apps         │      │                       │   │
│  └──────────────────┘      └───────────────────────┘   │
└─────────────────────────────────────────────────────────┘
```

### Component Hierarchy

```
SwarmOS Root
├── Desktop Environment
│   ├── Taskbar Component
│   │   ├── Start Button
│   │   ├── Running Apps
│   │   └── System Tray
│   ├── Desktop Component
│   │   ├── Desktop Icons
│   │   ├── Context Menu
│   │   └── Wallpaper
│   └── Window Container
│       └── App Windows (Dynamic)
├── Start Menu
│   ├── Search Bar
│   ├── App Grid
│   ├── User Profile
│   └── Power Options
├── File Manager App
├── Settings App
└── Built-in Apps
```

---

## 📦 Installation & Setup

### Prerequisites

Before you begin, ensure you have the following installed:

```bash
# Required
Node.js v18+ LTS
npm v9+ or yarn v1.22+
MongoDB v6+
Git

# Recommended
Docker & Docker Compose (for containerized setup)
VS Code with Angular extension
```

### Method 1: Standard Installation

1. **Navigate to Project Location**
   ```bash
   cd D:\source\AI\SwarmOS
   ```

2. **Install Frontend Dependencies**
   ```bash
   cd frontend
   npm install
   ```

3. **Install Backend Dependencies**
   ```bash
   cd ../backend
   npm install
   ```

4. **Configure Environment Variables**

   Create `.env` file in backend directory:
   ```env
   # Server Configuration
   PORT=3000
   NODE_ENV=development

   # MongoDB Configuration
   MONGODB_URI=mongodb://localhost:27017/swarmos

   # JWT Configuration
   JWT_SECRET=your-super-secret-jwt-key-change-this
   JWT_EXPIRES_IN=7d

   # Socket.io Configuration
   SOCKET_PORT=3001
   CORS_ORIGIN=http://localhost:4200

   # File Upload Configuration
   MAX_FILE_SIZE=10485760  # 10MB in bytes
   UPLOAD_PATH=./uploads
   ```

5. **Start MongoDB**
   ```bash
   # Windows
   net start MongoDB

   # Linux/Mac
   sudo systemctl start mongodb

   # Docker
   docker run -d -p 27017:27017 --name mongodb mongo:latest
   ```

6. **Start Backend Server**
   ```bash
   cd backend
   npm run dev
   ```

7. **Start Frontend Development Server**
   ```bash
   cd frontend
   npm start
   # or
   ng serve
   ```

8. **Access SwarmOS**

   Open your browser and navigate to:
   ```
   http://localhost:4200
   ```

### Method 2: Docker Installation

1. **Navigate to Project Root**
   ```bash
   cd D:\source\AI\SwarmOS
   ```

2. **Build and Start Containers**
   ```bash
   docker-compose up -d
   ```

3. **Access SwarmOS**
   ```
   http://localhost:4200
   ```

### Default Credentials

```
Username: admin
Password: [Set on first login]
```

> ⚠️ **Security Warning:** You will be required to set a secure password on first login!

---

## 📁 Project Structure

```
SwarmOS/
├── frontend/                    # Angular 18+ Frontend Application
│   ├── src/
│   │   ├── app/
│   │   │   ├── core/           # Core services and guards
│   │   │   │   ├── services/
│   │   │   │   │   ├── window.service.ts
│   │   │   │   │   ├── desktop.service.ts
│   │   │   │   │   ├── auth.service.ts
│   │   │   │   │   └── socket.service.ts
│   │   │   │   └── guards/
│   │   │   ├── components/      # Reusable components
│   │   │   │   ├── window/
│   │   │   │   ├── taskbar/
│   │   │   │   ├── start-menu/
│   │   │   │   └── desktop/
│   │   │   ├── apps/            # Built-in applications
│   │   │   │   ├── file-manager/
│   │   │   │   ├── text-editor/
│   │   │   │   ├── calculator/
│   │   │   │   └── settings/
│   │   │   ├── models/          # TypeScript interfaces
│   │   │   └── shared/          # Shared utilities
│   │   ├── assets/              # Static assets
│   │   │   ├── icons/
│   │   │   ├── wallpapers/
│   │   │   └── themes/
│   │   └── environments/        # Environment configs
│   ├── angular.json
│   ├── package.json
│   └── tsconfig.json
│
├── backend/                     # Node.js Backend Server
│   ├── src/
│   │   ├── controllers/         # Route controllers
│   │   │   ├── auth.controller.js
│   │   │   ├── file.controller.js
│   │   │   └── user.controller.js
│   │   ├── models/              # MongoDB models
│   │   │   ├── User.js
│   │   │   ├── File.js
│   │   │   └── Session.js
│   │   ├── middleware/          # Express middleware
│   │   │   ├── auth.middleware.js
│   │   │   └── upload.middleware.js
│   │   ├── routes/              # API routes
│   │   │   ├── auth.routes.js
│   │   │   ├── file.routes.js
│   │   │   └── user.routes.js
│   │   ├── services/            # Business logic
│   │   │   ├── auth.service.js
│   │   │   └── file.service.js
│   │   ├── socket/              # Socket.io handlers
│   │   │   └── handlers.js
│   │   └── utils/               # Utility functions
│   ├── uploads/                 # File upload directory
│   ├── package.json
│   └── server.js
│
├── docker-compose.yml           # Docker composition
├── Dockerfile                   # Docker image definition
├── .env.example                 # Environment template
└── README.md                    # This file
```

---

## 🛣️ Development Roadmap

### Phase 1: Foundation (✅ Completed - 40%)
- [x] Window management system
- [x] Taskbar and start menu
- [x] Basic desktop environment
- [x] User authentication
- [x] File system structure

### Phase 2: Core Features (🟡 In Progress - 30%)
- [x] File manager application
- [ ] Text editor with syntax highlighting
- [ ] Calculator application
- [ ] Terminal emulator
- [ ] Settings panel
- [ ] Theme system completion

### Phase 3: Advanced Features (🔴 Planned - Q2 2025)
- [ ] Multi-user collaboration
- [ ] App store for third-party apps
- [ ] Video and audio players
- [ ] Image editor
- [ ] Email client
- [ ] Calendar and tasks

### Phase 4: Enterprise Features (🔴 Planned - Q3 2025)
- [ ] Role-based access control (RBAC)
- [ ] Active Directory integration
- [ ] SSO (Single Sign-On) support
- [ ] Advanced security features
- [ ] Audit logging
- [ ] Admin dashboard

### Phase 5: Polish & Production (🔴 Planned - Q4 2025)
- [ ] Performance optimization
- [ ] Comprehensive testing
- [ ] Documentation completion
- [ ] Accessibility features
- [ ] Mobile optimization
- [ ] Production deployment

---

## 📸 Screenshots

> 🚧 **Coming Soon** - Screenshots will be added as features are completed

**Planned Screenshots:**
- Desktop Environment with Multiple Windows
- Start Menu and Application Launcher
- File Manager Application
- Settings Panel
- Theme Customization
- Mobile Responsive View

---

## 📚 API Documentation

### Authentication Endpoints

#### POST /api/auth/register
Register a new user account

**Request Body:**
```json
{
  "username": "string",
  "email": "string",
  "password": "string",
  "fullName": "string"
}
```

**Response:**
```json
{
  "success": true,
  "token": "jwt-token",
  "user": {
    "id": "user-id",
    "username": "string",
    "email": "string"
  }
}
```

#### POST /api/auth/login
Authenticate user and receive JWT token

**Request Body:**
```json
{
  "username": "string",
  "password": "string"
}
```

**Response:**
```json
{
  "success": true,
  "token": "jwt-token",
  "user": {
    "id": "user-id",
    "username": "string",
    "settings": {}
  }
}
```

### File System Endpoints

#### GET /api/files
List files and folders

**Query Parameters:**
- `path` - Directory path (default: /)
- `limit` - Number of items per page
- `offset` - Pagination offset

#### POST /api/files/upload
Upload file to user's file system

**Request:** Multipart form data with file

#### DELETE /api/files/:id
Delete file or folder

### Socket.io Events

#### Client → Server
- `window:open` - Open new window
- `window:close` - Close window
- `window:minimize` - Minimize window
- `file:watch` - Watch file for changes

#### Server → Client
- `window:opened` - Window opened confirmation
- `file:changed` - File was modified
- `user:online` - User came online
- `notification` - System notification

---

## 🔧 Troubleshooting

### Common Issues

#### MongoDB Connection Failed
```bash
Error: connect ECONNREFUSED 127.0.0.1:27017
```

**Solution:**
```bash
# Ensure MongoDB is running
# Windows
net start MongoDB

# Linux/Mac
sudo systemctl start mongodb

# Check MongoDB status
mongo --eval "db.stats()"
```

#### Port Already in Use
```bash
Error: listen EADDRINUSE: address already in use :::3000
```

**Solution:**
```bash
# Find process using port
# Windows
netstat -ano | findstr :3000
taskkill /PID <PID> /F

# Linux/Mac
lsof -i :3000
kill -9 <PID>
```

#### Frontend Build Errors
```bash
Error: Cannot find module '@angular/core'
```

**Solution:**
```bash
cd frontend
rm -rf node_modules package-lock.json
npm install
```

#### Socket.io Connection Issues
Check CORS settings in backend `.env`:
```env
CORS_ORIGIN=http://localhost:4200
```

Ensure Socket.io client version matches server version.

### Getting Help

- **Company:** NorthPeak ([northpeak.app](https://northpeak.app))
- 📖 [Full Documentation](D:\source\AI\SwarmOS\docs)
- 🐛 [Report Issues](https://github.com/swarm-tech/SwarmOS/issues)
- 📧 Email: support@northpeak.app
- 🌐 Website: [northpeak.app](https://northpeak.app)

---

## 🤝 Contributing

We welcome contributions to SwarmOS! Here's how you can help:

### Development Setup

1. Fork the repository
2. Clone your fork: `git clone https://github.com/your-username/SwarmOS.git`
3. Create a feature branch: `git checkout -b feature/amazing-feature`
4. Make your changes
5. Commit: `git commit -m "feat: add amazing feature"`
6. Push: `git push origin feature/amazing-feature`
7. Open a Pull Request

### Code Standards

- **TypeScript** - Use strict type checking
- **ESLint** - Follow project ESLint rules
- **Prettier** - Format code before committing
- **Commits** - Use conventional commit messages
- **Tests** - Add tests for new features

### Areas Needing Help

- 🎨 UI/UX improvements
- 📱 Mobile responsiveness
- 🧪 Test coverage
- 📝 Documentation
- 🌐 Internationalization
- ♿ Accessibility features

---

## 📄 License

This project is licensed under the **MIT License**.

```
MIT License

Copyright (c) 2024-2025 NorthPeak (northpeak.app)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

---

## 🔗 Links

- **Main Portfolio:** [Swarm Tech README](../README.md)
- **Company:** [NorthPeak](https://northpeak.app)
- **Project Location:** `D:\source\AI\SwarmOS`
- **Documentation:** [Full Docs](D:\source\AI\SwarmOS\docs)
- **Support:** support@northpeak.app

---

<div align="center">

**Part of Swarm Tech Portfolio by NorthPeak**

[northpeak.app](https://northpeak.app) | [support@northpeak.app](mailto:support@northpeak.app)

Built with ❤️ by the NorthPeak Team

[⬆ Back to Top](#-swarmos)

</div>
