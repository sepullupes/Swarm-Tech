# 🔐 SwarmVPN

<div align="center">

![SwarmVPN Banner](https://img.shields.io/badge/SwarmVPN-Corporate%20VPN%20Platform-success?style=for-the-badge)

**Enterprise-Grade Self-Hosted VPN Network Platform**

*Part of Swarm Tech Portfolio by NorthPeak*

[![Status](https://img.shields.io/badge/Status-Beta%20(95%25)-brightgreen?style=flat-square)](README.md)
[![Tech Stack](https://img.shields.io/badge/Stack-Go%20%7C%20React%20%7C%20Tauri%20%7C%20WireGuard-blue?style=flat-square)](README.md)
[![Production Ready](https://img.shields.io/badge/Production-Beta%20Ready-yellow?style=flat-square)](README.md)

[Features](#-core-features) • [Tech Stack](#-technology-stack) • [Setup](#-installation--setup) • [Architecture](#-architecture) • [Deployment](#-deployment)

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Status](#-project-status)
- [Core Features](#-core-features)
- [VPN Capabilities](#-vpn-capabilities)
- [Technology Stack](#-technology-stack)
- [Architecture](#-architecture)
- [Installation & Setup](#-installation--setup)
- [Components](#-components)
- [Database Schema](#-database-schema)
- [API Documentation](#-api-documentation)
- [Desktop Client](#-desktop-client)
- [Deployment](#-deployment)
- [Security Features](#-security-features)
- [Comparison](#-comparison-with-radmin-vpn)
- [Screenshots](#-screenshots)
- [Monitoring](#-monitoring--analytics)
- [Troubleshooting](#-troubleshooting)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🌟 Overview

**SwarmVPN** is an enterprise-grade, self-hosted VPN network platform that combines the power of WireGuard protocol with advanced corporate networking features. Built as a sophisticated alternative to Radmin VPN, SwarmVPN offers user-created networks, unlimited device support, peer-to-peer actions, team collaboration, and comprehensive network management.

### Why SwarmVPN?

- **🛡️ WireGuard Protocol** - Modern, fast, and secure VPN technology
- **🌐 User-Created Networks** - Radmin VPN-style network creation
- **🔌 Unlimited Devices** - No device limitations per user
- **🤝 Peer-to-Peer Actions** - 15+ P2P features (ping, buzz, WoL, file transfer)
- **💬 Built-in Chat** - Team messaging and communication
- **📁 File Sync** - Cross-device file synchronization with versioning
- **👥 Enterprise Features** - RBAC, audit logs, activity monitoring
- **🖥️ Native Client** - Production-ready Windows desktop application (Tauri)
- **📊 Analytics** - Comprehensive monitoring with Prometheus & Grafana
- **🔒 Self-Hosted** - Complete data privacy and control

### Use Cases

- **Corporate Networks** - Secure remote access for distributed teams
- **Development Teams** - Private development environment access
- **Gaming Communities** - Low-latency LAN gaming over the internet
- **Remote Support** - Technical support with remote control features
- **File Sharing** - Secure file transfer between team members
- **Multi-Site Connectivity** - Connect multiple office locations

---

## 📊 Project Status

> ⚠️ **Beta (95% Complete - Production Ready)** - Feature-complete with production installers

| Component | Status | Completion | Production Ready |
|-----------|--------|------------|------------------|
| Backend API (Go) | ✅ Complete | 100% | ✅ Yes |
| Admin Portal (React) | ✅ Complete | 100% | ✅ Yes |
| Desktop Client (Tauri) | ✅ Complete | 95% | ✅ Yes |
| WireGuard Integration | ✅ Complete | 100% | ✅ Yes |
| Database Schema | ✅ Complete | 100% | ✅ Yes |
| WebSocket Features | ✅ Complete | 100% | ✅ Yes |
| File Transfer | ✅ Complete | 90% | ✅ Yes |
| Monitoring Stack | ✅ Complete | 100% | ✅ Yes |
| Windows Installers | ✅ Complete | 100% | ✅ Yes |
| Docker Deployment | ✅ Complete | 100% | ✅ Yes |
| Documentation | ✅ Complete | 95% | ✅ Yes |

**Latest Update:** January 2025
**Total Codebase:** 60,000+ lines across 269+ files
**Backend:** 35,050+ lines of Go code
**API Endpoints:** 85+ RESTful endpoints
**Production Deployments:** Ready for deployment

---

## 🚀 Core Features

### Network Management
- **User-Created Networks** - Users can create and manage their own VPN networks
- **Network Invitations** - Invite users via email or unique join codes
- **Admin Approval Workflow** - Control network member approvals
- **Multi-Network Membership** - Join multiple networks simultaneously
- **Network Discovery** - Find and join public/private networks
- **Network Analytics** - Traffic statistics and connection metrics

### Device Management
- **Unlimited Devices** - Add unlimited devices per user
- **Multi-Platform Support** - Windows (ready), Linux/macOS (planned)
- **Device Profiles** - Custom configurations per device
- **Auto IP Allocation** - Automatic IP address assignment (10.0.0.0/8 range)
- **Device Status** - Real-time online/offline tracking
- **Connection History** - Track device connection patterns

### Peer-to-Peer Actions (15+ Features)
1. **Ping** - Test connectivity between peers
2. **Buzz/Knock** - Send attention notifications
3. **Wake-on-LAN** - Remote device wake-up
4. **Remote Desktop** - VNC/RDP integration
5. **File Transfer** - Direct P2P file sharing
6. **Screen Sharing** - Share screens with peers
7. **Clipboard Sync** - Cross-device clipboard sharing
8. **Message Send** - Direct peer messaging
9. **Network Statistics** - View peer bandwidth usage
10. **Port Forwarding** - Configure port forwarding rules
11. **Traffic Monitoring** - Real-time traffic analysis
12. **Connection Quality** - Latency and packet loss metrics
13. **Custom Commands** - Execute predefined commands
14. **Resource Sharing** - Share folders and printers
15. **Remote Control** - Full remote device control

### Team Collaboration
- **Team Chat** - Built-in messaging system
- **Channel Support** - Public and private channels
- **Direct Messages** - One-on-one conversations
- **File Attachments** - Share files in chat
- **Message History** - Searchable message archives
- **Presence Indicators** - See who's online
- **Typing Indicators** - Real-time typing status
- **Read Receipts** - Message read confirmation

### File Synchronization
- **Cross-Device Sync** - Sync files across all devices
- **Version Control** - File versioning with rollback
- **Conflict Resolution** - Automatic conflict handling
- **Selective Sync** - Choose what to sync
- **Bandwidth Control** - Throttle sync speed
- **Large File Support** - Handle files up to 10GB

### Activity Monitoring (10 Types)
1. **Login Activities** - User authentication events
2. **Network Changes** - Network configuration modifications
3. **Device Changes** - Device additions/removals
4. **File Transfers** - File sharing activities
5. **Connection Events** - VPN connection/disconnection
6. **Admin Actions** - Administrative operations
7. **Security Events** - Security-related activities
8. **P2P Actions** - Peer-to-peer interactions
9. **Chat Activities** - Messaging events
10. **System Events** - System-level operations

### Advanced Security
- **WireGuard Encryption** - ChaCha20-Poly1305 encryption
- **Perfect Forward Secrecy** - Curve25519 key exchange
- **JWT Authentication** - Secure API authentication
- **bcrypt Password Hashing** - Industry-standard password security
- **AES-256 Encryption** - Additional data encryption
- **Audit Logging** - Comprehensive activity logs
- **RBAC** - Role-based access control
- **2FA Support** - Two-factor authentication (planned)
- **IP Whitelisting** - Network-level access control
- **Session Management** - Secure session handling

---

## 🌐 VPN Capabilities

### WireGuard Protocol
- **Modern Cryptography** - State-of-the-art encryption (ChaCha20-Poly1305)
- **High Performance** - 4000+ Mbps throughput
- **Low Latency** - Sub-millisecond overhead
- **Battery Efficient** - Minimal battery drain on mobile devices
- **Simple Configuration** - Easy to set up and maintain
- **Cross-Platform** - Works on all major operating systems

### Network Architecture
- **NAT Traversal** - Connect devices behind NAT/firewalls
- **Relay Server** - Fallback relay for difficult networks
- **Mesh Topology** - Direct peer-to-peer connections
- **Multi-Region Support** - Deploy servers globally
- **Load Balancing** - Distribute traffic across servers
- **Failover** - Automatic failover to backup servers

### Connectivity Features
- **Auto-Reconnect** - Automatic reconnection on network changes
- **Roaming Support** - Seamless network switching
- **Split Tunneling** - Route specific traffic through VPN
- **Kill Switch** - Block internet if VPN disconnects (planned)
- **DNS Management** - Custom DNS server configuration
- **IPv6 Support** - Full IPv6 compatibility

---

## 🛠️ Technology Stack

### Backend (Go 1.23)
- **Gin Framework** - High-performance HTTP web framework
- **GORM** - Elegant ORM for database operations
- **PostgreSQL 15** - Advanced relational database
- **Redis 7** - In-memory caching and session storage
- **WebSocket** - Real-time bidirectional communication
- **WireGuard Tools** - VPN protocol integration
- **JWT-Go** - JSON Web Token implementation
- **bcrypt** - Password hashing library
- **Prometheus Client** - Metrics collection
- **Logrus** - Structured logging

### Desktop Client (Windows)
- **Tauri 2.x** - Rust-based desktop framework
- **React 19** - Modern UI library with hooks
- **TypeScript** - Type-safe JavaScript
- **Ant Design** - Enterprise UI component library
- **Zustand** - Lightweight state management
- **React Query** - Server state management
- **Axios** - HTTP client
- **Socket.io Client** - WebSocket communication
- **MSI Installer** - Windows installer package
- **NSIS** - Alternative installer option

### Admin Portal (React)
- **React 19** - Modern UI framework
- **Vite** - Next-generation build tool
- **TypeScript** - Static type checking
- **TailwindCSS** - Utility-first CSS framework
- **Ant Design** - Component library
- **React Router v6** - Client-side routing
- **Zustand** - State management
- **React Query** - Server state caching
- **Chart.js** - Data visualization
- **Socket.io Client** - Real-time updates

### Database & Cache
- **PostgreSQL 15** - Primary database
  - 25+ tables for network, devices, users
  - Full-text search capabilities
  - JSON field support
  - Advanced indexing
- **Redis 7** - Caching and real-time data
  - Session storage
  - WebSocket presence
  - Rate limiting
  - Job queuing

### Infrastructure
- **Docker** - Containerization
- **Docker Compose** - Multi-container orchestration
- **Nginx** - Reverse proxy (optional)
- **Prometheus** - Metrics collection
- **Grafana** - Monitoring dashboards
- **WireGuard** - VPN protocol
- **SystemD** - Linux service management

### Monitoring & Analytics
- **Prometheus** - Time-series metrics database
- **Grafana** - Visualization and dashboards
- **Custom Metrics** - Application-specific metrics
  - Active connections
  - Network traffic
  - API performance
  - Database queries
  - WebSocket connections

---

## 🏗️ Architecture

### System Architecture

```
┌─────────────────────────────────────────────────────────┐
│                    Clients Layer                        │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐ │
│  │   Windows    │  │  Web Admin   │  │    Mobile    │ │
│  │Desktop Client│  │    Portal    │  │  (Planned)   │ │
│  │   (Tauri)    │  │   (React)    │  │              │ │
│  └──────────────┘  └──────────────┘  └──────────────┘ │
└─────────────────────────────────────────────────────────┘
                         │
                         ▼
┌─────────────────────────────────────────────────────────┐
│              Load Balancer (Optional)                   │
│                    Nginx / HAProxy                      │
└─────────────────────────────────────────────────────────┘
                         │
                         ▼
┌─────────────────────────────────────────────────────────┐
│                 Backend API (Go + Gin)                  │
│                      Port: 8080                         │
│  ┌────────────────────────────────────────────────────┐│
│  │  REST API (85+ endpoints)                          ││
│  │  - Auth API       - Network API                    ││
│  │  - Device API     - User API                       ││
│  │  - Peer API       - Chat API                       ││
│  │  - File API       - Activity API                   ││
│  └────────────────────────────────────────────────────┘│
│  ┌────────────────────────────────────────────────────┐│
│  │  WebSocket Server (Port: 8080/ws)                  ││
│  │  - Real-time Chat      - Presence                  ││
│  │  - Notifications       - P2P Signaling             ││
│  │  - File Progress       - Network Events            ││
│  └────────────────────────────────────────────────────┘│
│  ┌────────────────────────────────────────────────────┐│
│  │  WireGuard Manager                                  ││
│  │  - Config Generation   - Key Management            ││
│  │  - Peer Management     - NAT Traversal             ││
│  └────────────────────────────────────────────────────┘│
└─────────────────────────────────────────────────────────┘
                         │
        ┌────────────────┼────────────────┐
        │                │                │
        ▼                ▼                ▼
┌──────────────┐  ┌──────────────┐  ┌──────────────┐
│  PostgreSQL  │  │    Redis     │  │  WireGuard   │
│  Database    │  │    Cache     │  │  VPN Server  │
│  Port: 5432  │  │  Port: 6379  │  │  Port: 51820 │
│              │  │              │  │   (UDP)      │
│  25+ Tables  │  │  Sessions    │  │              │
│  Users       │  │  Presence    │  │  Encrypted   │
│  Networks    │  │  Rate Limit  │  │  Tunnels     │
│  Devices     │  │  WebSocket   │  │              │
└──────────────┘  └──────────────┘  └──────────────┘

Monitoring Stack:
┌──────────────┐  ┌──────────────┐
│  Prometheus  │  │   Grafana    │
│  Port: 9090  │  │  Port: 3001  │
│  Metrics     │  │  Dashboards  │
└──────────────┘  └──────────────┘
```

### Application Structure

```
SwarmVPN/
├── backend/                      # Go Backend (35,050+ lines)
│   ├── cmd/
│   │   └── server/
│   │       └── main.go          # Application entry point
│   ├── internal/
│   │   ├── api/                 # API handlers
│   │   │   ├── auth/
│   │   │   ├── network/
│   │   │   ├── device/
│   │   │   ├── peer/
│   │   │   ├── chat/
│   │   │   └── file/
│   │   ├── models/              # Database models (25+ tables)
│   │   │   ├── user.go
│   │   │   ├── network.go
│   │   │   ├── device.go
│   │   │   ├── peer_action.go
│   │   │   └── activity.go
│   │   ├── services/            # Business logic
│   │   │   ├── wireguard/
│   │   │   ├── nat_traversal/
│   │   │   └── file_sync/
│   │   ├── websocket/           # WebSocket handlers
│   │   ├── middleware/          # Auth, CORS, logging
│   │   └── config/              # Configuration
│   ├── migrations/              # Database migrations
│   ├── go.mod
│   └── go.sum
│
├── desktop-client/               # Tauri Desktop App
│   ├── src/                     # React frontend
│   │   ├── components/
│   │   │   ├── Dashboard/
│   │   │   ├── Networks/
│   │   │   ├── Devices/
│   │   │   ├── Chat/
│   │   │   └── Settings/
│   │   ├── hooks/
│   │   ├── services/
│   │   ├── store/
│   │   └── utils/
│   ├── src-tauri/               # Rust backend
│   │   ├── src/
│   │   │   ├── main.rs
│   │   │   ├── wireguard.rs
│   │   │   └── system_tray.rs
│   │   ├── Cargo.toml
│   │   └── tauri.conf.json
│   ├── installers/              # Production installers
│   │   ├── SwarmVPN_Setup.msi
│   │   └── SwarmVPN_Setup.exe
│   └── package.json
│
├── admin-portal/                 # React Admin Dashboard
│   ├── src/
│   │   ├── components/
│   │   │   ├── Dashboard/
│   │   │   ├── Users/
│   │   │   ├── Networks/
│   │   │   ├── Analytics/
│   │   │   └── Settings/
│   │   ├── services/
│   │   ├── store/
│   │   └── utils/
│   ├── public/
│   └── package.json
│
├── monitoring/                   # Prometheus & Grafana
│   ├── prometheus/
│   │   ├── prometheus.yml
│   │   └── alerts.yml
│   ├── grafana/
│   │   ├── dashboards/
│   │   │   ├── network-overview.json
│   │   │   ├── api-performance.json
│   │   │   └── vpn-metrics.json
│   │   └── datasources/
│   └── docker-compose.monitoring.yml
│
├── docker-compose.yml            # Production deployment
├── docker-compose.dev.yml        # Development setup
├── .env.example                  # Environment template
├── README.md                     # This file
└── docs/                         # Additional documentation
    ├── API.md
    ├── DEPLOYMENT.md
    ├── DEVELOPMENT.md
    └── ARCHITECTURE.md
```

---

## 📦 Installation & Setup

### Prerequisites

```bash
# Required
Go 1.23+
Node.js v20+ LTS
PostgreSQL 15+
Redis 7+
WireGuard Tools
Docker & Docker Compose (recommended)

# For Desktop Client Development
Rust 1.75+
Tauri CLI
```

### Quick Start with Docker (Recommended)

1. **Navigate to Project Directory**
   ```bash
   cd F:\Docker\SwarmVPN
   ```

2. **Copy Environment Files**
   ```bash
   cp .env.example .env
   ```

3. **Configure Environment Variables**

   Edit `.env`:
   ```env
   # Database
   DB_HOST=postgres
   DB_PORT=5432
   DB_NAME=swarmvpn
   DB_USER=swarmvpn
   DB_PASSWORD=your-secure-password

   # Redis
   REDIS_HOST=redis
   REDIS_PORT=6379
   REDIS_PASSWORD=your-redis-password

   # JWT
   JWT_SECRET=your-super-secret-jwt-key-change-this
   JWT_EXPIRES_IN=24h

   # WireGuard
   WG_INTERFACE=wg0
   WG_PORT=51820
   WG_SERVER_IP=10.0.0.1
   WG_SUBNET=10.0.0.0/8

   # Server
   SERVER_HOST=0.0.0.0
   SERVER_PORT=8080
   PUBLIC_URL=https://vpn.yourdomain.com

   # File Storage
   UPLOAD_DIR=/app/uploads
   MAX_FILE_SIZE=10737418240  # 10GB
   ```

4. **Start All Services**
   ```bash
   docker-compose up -d
   ```

5. **Initialize Database**
   ```bash
   docker-compose exec backend ./swarmvpn migrate
   ```

6. **Create Admin User**
   ```bash
   docker-compose exec backend ./swarmvpn create-admin \
     --email admin@yourdomain.com \
     --password YourSecurePassword123!
   ```

7. **Access Applications**
   - Backend API: http://localhost:8080
   - Admin Portal: http://localhost:3000
   - Prometheus: http://localhost:9090
   - Grafana: http://localhost:3001
   - API Docs: http://localhost:8080/swagger

### Manual Installation

#### Backend Setup

```bash
# Clone repository (or navigate to project)
cd F:\Docker\SwarmVPN\backend

# Install Go dependencies
go mod download

# Install WireGuard tools
# Windows: Download from https://www.wireguard.com/install/
# Linux: sudo apt install wireguard-tools

# Configure PostgreSQL
createdb swarmvpn
psql swarmvpn < migrations/init.sql

# Run migrations
go run cmd/server/main.go migrate

# Start backend
go run cmd/server/main.go serve
```

#### Desktop Client Setup

```bash
cd F:\Docker\SwarmVPN\desktop-client

# Install dependencies
npm install

# Development mode
npm run tauri dev

# Build production installer
npm run tauri build
# Output: src-tauri/target/release/bundle/msi/SwarmVPN_Setup.msi
```

#### Admin Portal Setup

```bash
cd F:\Docker\SwarmVPN\admin-portal

# Install dependencies
npm install

# Development mode
npm run dev

# Build for production
npm run build
```

### Default Admin Credentials

```
Email: admin@swarmvpn.local
Password: [Set during installation wizard]
```

> ⚠️ **Security:** Password must be configured during installation wizard!

---

## 🔧 Components

### 1. Backend API (Go)
- **Language:** Go 1.23
- **Framework:** Gin
- **Lines of Code:** 35,050+
- **Endpoints:** 85+
- **Features:**
  - RESTful API design
  - JWT authentication
  - WebSocket support
  - WireGuard integration
  - File upload/download
  - Real-time notifications
  - Activity logging
  - Prometheus metrics

### 2. Desktop Client (Tauri)
- **Framework:** Tauri 2.x + React 19
- **Platform:** Windows (production-ready)
- **Installer Types:** MSI, NSIS
- **Features:**
  - System tray integration
  - Auto-start on boot
  - Background VPN management
  - Real-time chat
  - File transfer UI
  - Network visualization
  - Notification center
  - Settings management

### 3. Admin Portal (React)
- **Framework:** React 19 + Vite
- **Styling:** TailwindCSS + Ant Design
- **Features:**
  - User management
  - Network oversight
  - Analytics dashboards
  - Activity monitoring
  - System configuration
  - Audit logs
  - Report generation

### 4. Monitoring Stack
- **Prometheus:** Metrics collection
- **Grafana:** Visualization
- **Dashboards:**
  - Network overview
  - API performance
  - VPN metrics
  - Database stats
  - WebSocket connections

---

## 🗄️ Database Schema

### Core Tables (25+)

1. **users** - User accounts and authentication
2. **networks** - VPN network configurations
3. **network_members** - Network membership relations
4. **devices** - User devices and WireGuard configs
5. **peer_actions** - P2P action logs (15 types)
6. **messages** - Chat messages
7. **channels** - Chat channels
8. **files** - File metadata
9. **file_versions** - File version history
10. **activities** - Activity logs (10 types)
11. **invitations** - Network invitation codes
12. **sessions** - User sessions
13. **api_keys** - API authentication keys
14. **roles** - RBAC role definitions
15. **permissions** - Permission definitions
16. **user_roles** - User-role assignments
17. **network_settings** - Network-specific settings
18. **device_stats** - Device statistics
19. **traffic_logs** - Network traffic logs
20. **connection_logs** - VPN connection history
21. **wireguard_peers** - WireGuard peer configurations
22. **nat_mappings** - NAT traversal mappings
23. **relay_servers** - Relay server configurations
24. **notifications** - User notifications
25. **audit_logs** - Security audit trail

---

## 📚 API Documentation

### Authentication

#### Register
```http
POST /api/v1/auth/register
Content-Type: application/json

{
  "email": "user@example.com",
  "password": "SecurePass123!",
  "username": "johndoe"
}
```

#### Login
```http
POST /api/v1/auth/login
Content-Type: application/json

{
  "email": "user@example.com",
  "password": "SecurePass123!"
}

Response:
{
  "token": "eyJhbGciOiJIUzI1NiIs...",
  "user": {...}
}
```

### Networks

#### Create Network
```http
POST /api/v1/networks
Authorization: Bearer {token}
Content-Type: application/json

{
  "name": "My Corporate VPN",
  "description": "Company private network",
  "subnet": "10.0.0.0/24",
  "isPublic": false
}
```

#### List Networks
```http
GET /api/v1/networks?page=1&limit=20
Authorization: Bearer {token}
```

### Devices

#### Add Device
```http
POST /api/v1/devices
Authorization: Bearer {token}
Content-Type: application/json

{
  "name": "Work Laptop",
  "networkId": "network-uuid",
  "os": "Windows",
  "publicKey": "base64-encoded-public-key"
}
```

### Peer Actions

#### Send Ping
```http
POST /api/v1/peers/ping
Authorization: Bearer {token}
Content-Type: application/json

{
  "targetDeviceId": "device-uuid",
  "networkId": "network-uuid"
}
```

#### Wake-on-LAN
```http
POST /api/v1/peers/wake
Authorization: Bearer {token}
Content-Type: application/json

{
  "targetDeviceId": "device-uuid",
  "macAddress": "00:11:22:33:44:55"
}
```

### File Transfer

#### Upload File
```http
POST /api/v1/files/upload
Authorization: Bearer {token}
Content-Type: multipart/form-data

{
  "file": binary-data,
  "networkId": "network-uuid",
  "recipients": ["device-uuid-1", "device-uuid-2"]
}
```

### WebSocket Events (15+ types)

```javascript
// Connect
const ws = new WebSocket('ws://localhost:8080/ws');

// Events
- chat.message
- chat.typing
- peer.online
- peer.offline
- file.progress
- file.complete
- network.update
- device.status
- notification.new
- action.ping
- action.buzz
- action.wol
```

### Full API Documentation

Interactive Swagger docs available at:
```
http://localhost:8080/swagger
```

---

## 🖥️ Desktop Client

### Windows Client Features

- **System Tray Integration** - Minimize to tray, quick actions
- **Auto-Start** - Launch on Windows startup
- **Background Service** - Run VPN in background
- **Connection Manager** - Connect/disconnect networks
- **Device Manager** - Manage all devices
- **Chat Interface** - Built-in messaging
- **File Browser** - Access shared files
- **Peer Actions** - Execute P2P commands
- **Notifications** - Desktop notifications
- **Settings Panel** - Configure client behavior

### Installation

Download the installer from releases:
- **MSI Installer:** `SwarmVPN_Setup.msi` (Recommended)
- **NSIS Installer:** `SwarmVPN_Setup.exe` (Alternative)

### System Requirements

- **OS:** Windows 10/11 (64-bit)
- **RAM:** 2GB minimum, 4GB recommended
- **Disk:** 200MB free space
- **Network:** Internet connection required

### Future Clients

- **Linux** - Planned (AppImage, .deb, .rpm)
- **macOS** - Planned (.dmg, .app)
- **Android** - Planned
- **iOS** - Planned

---

## 🚀 Deployment

### Production Deployment with Docker

```bash
# 1. Clone/navigate to project
cd F:\Docker\SwarmVPN

# 2. Configure environment
cp .env.example .env
nano .env  # Edit configuration

# 3. Build and start services
docker-compose -f docker-compose.yml up -d

# 4. Check service health
docker-compose ps

# 5. View logs
docker-compose logs -f backend

# 6. Initialize database
docker-compose exec backend ./swarmvpn migrate

# 7. Create admin user
docker-compose exec backend ./swarmvpn create-admin
```

### Environment Variables

```env
# Database
DB_HOST=postgres
DB_PORT=5432
DB_NAME=swarmvpn
DB_USER=swarmvpn
DB_PASSWORD=change-this-password

# Redis
REDIS_HOST=redis
REDIS_PORT=6379
REDIS_PASSWORD=change-this-password

# JWT
JWT_SECRET=change-this-to-random-string
JWT_EXPIRES_IN=24h

# WireGuard
WG_INTERFACE=wg0
WG_PORT=51820
WG_SERVER_IP=10.0.0.1
WG_SUBNET=10.0.0.0/8

# Server
SERVER_HOST=0.0.0.0
SERVER_PORT=8080
PUBLIC_URL=https://vpn.yourdomain.com

# Monitoring
PROMETHEUS_ENABLED=true
GRAFANA_ADMIN_PASSWORD=change-this

# File Upload
MAX_FILE_SIZE=10737418240  # 10GB
UPLOAD_DIR=/app/uploads
```

### Nginx Configuration

```nginx
server {
    listen 80;
    server_name vpn.yourdomain.com;
    return 301 https://$server_name$request_uri;
}

server {
    listen 443 ssl http2;
    server_name vpn.yourdomain.com;

    ssl_certificate /etc/nginx/ssl/cert.pem;
    ssl_certificate_key /etc/nginx/ssl/key.pem;

    # Backend API
    location /api {
        proxy_pass http://localhost:8080;
        proxy_http_version 1.1;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection 'upgrade';
        proxy_set_header Host $host;
        proxy_cache_bypass $http_upgrade;
    }

    # WebSocket
    location /ws {
        proxy_pass http://localhost:8080;
        proxy_http_version 1.1;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection "upgrade";
        proxy_set_header Host $host;
    }

    # Admin Portal
    location / {
        proxy_pass http://localhost:3000;
        proxy_set_header Host $host;
    }
}
```

### WireGuard Server Setup

```bash
# 1. Install WireGuard
sudo apt install wireguard

# 2. Generate server keys
wg genkey | tee /etc/wireguard/privatekey | wg pubkey > /etc/wireguard/publickey

# 3. Configure interface
sudo nano /etc/wireguard/wg0.conf

# 4. Enable IP forwarding
echo "net.ipv4.ip_forward=1" | sudo tee -a /etc/sysctl.conf
sudo sysctl -p

# 5. Start WireGuard
sudo systemctl enable wg-quick@wg0
sudo systemctl start wg-quick@wg0
```

### Health Checks

All services include health check endpoints:

```bash
# Backend
curl http://localhost:8080/health

# PostgreSQL
docker-compose exec postgres pg_isready

# Redis
docker-compose exec redis redis-cli ping

# Prometheus
curl http://localhost:9090/-/healthy

# Grafana
curl http://localhost:3001/api/health
```

---

## 🔒 Security Features

### Encryption
- ✅ **WireGuard Protocol** - ChaCha20-Poly1305 encryption
- ✅ **Perfect Forward Secrecy** - Curve25519 key exchange
- ✅ **AES-256 Encryption** - Additional data encryption
- ✅ **TLS/SSL** - HTTPS for all web traffic
- ✅ **bcrypt** - Password hashing (cost factor: 12)

### Authentication & Authorization
- ✅ **JWT Tokens** - Stateless authentication
- ✅ **Refresh Tokens** - Secure token renewal
- ✅ **RBAC** - Role-based access control
- ✅ **API Keys** - Service authentication
- ✅ **Session Management** - Secure session handling
- ✅ **2FA Support** - Two-factor authentication (planned)

### Network Security
- ✅ **IP Whitelisting** - Restrict access by IP
- ✅ **Rate Limiting** - DDoS protection
- ✅ **CORS Configuration** - Cross-origin security
- ✅ **XSS Protection** - Input sanitization
- ✅ **SQL Injection Prevention** - Parameterized queries
- ✅ **CSRF Protection** - Token-based CSRF prevention

### Audit & Compliance
- ✅ **Audit Logs** - Comprehensive activity logging
- ✅ **Activity Monitoring** - 10 activity types tracked
- ✅ **Connection Logs** - VPN connection history
- ✅ **File Access Logs** - File operation tracking
- ✅ **Admin Actions** - Administrative operation logs
- ✅ **GDPR Ready** - Data privacy compliance

---

## 🆚 Comparison with Radmin VPN

| Feature | Radmin VPN | SwarmVPN |
|---------|------------|----------|
| **Protocol** | Proprietary | WireGuard (Open Source) |
| **Speed** | Good (100 Mbps) | Excellent (4000+ Mbps) |
| **User Networks** | ✅ Yes | ✅ Yes |
| **Unlimited Devices** | ✅ Yes | ✅ Yes |
| **Peer Actions** | Limited (5) | ✅ Extensive (15+) |
| **Built-in Chat** | ❌ No | ✅ Yes |
| **File Transfer** | ❌ No | ✅ Yes |
| **File Sync** | ❌ No | ✅ Yes (with versioning) |
| **Web Admin Portal** | ❌ No | ✅ Yes |
| **Activity Logging** | ❌ No | ✅ Yes (10 types) |
| **RBAC** | ❌ No | ✅ Yes |
| **API Access** | ❌ No | ✅ Yes (85+ endpoints) |
| **Monitoring** | ❌ No | ✅ Yes (Prometheus + Grafana) |
| **Self-Hosted** | ❌ Cloud-based | ✅ Yes |
| **Open Source** | ❌ Proprietary | ✅ MIT License |
| **Mobile Apps** | ✅ Yes | ⚠️ Planned |
| **Price** | Free | Free (Self-hosted) |
| **Enterprise Features** | Limited | ✅ Full Suite |
| **Customization** | ❌ No | ✅ Full Control |

### SwarmVPN Advantages

1. **Modern Protocol** - WireGuard is faster, more secure, and battery-efficient
2. **Enterprise Features** - RBAC, audit logs, analytics, monitoring
3. **Collaboration Tools** - Built-in chat, file sync, team features
4. **Self-Hosted** - Complete data privacy and control
5. **Extensible** - Open API for custom integrations
6. **Monitoring** - Comprehensive observability with Prometheus/Grafana
7. **Advanced P2P** - 15+ peer-to-peer actions
8. **Web Portal** - Admin dashboard for centralized management

---

## 📸 Screenshots

Screenshots available at `F:\Docker\SwarmVPN\`:

1. **swarmvpn.png** - Application logo and branding
2. **login-page.png** - User authentication interface
3. **dashboard-page.png** - Main dashboard overview
4. **network-page.png** - Network management interface
5. **devices-page.png** - Device management panel
6. **users-page.png** - User administration
7. **settings-page.png** - Configuration settings
8. **monitoring-page.png** - Grafana monitoring dashboard

---

## 📊 Monitoring & Analytics

### Prometheus Metrics

- **VPN Metrics:**
  - Active connections
  - Bandwidth usage
  - Connection duration
  - Peer latency
  - Packet loss

- **API Metrics:**
  - Request rate
  - Response time
  - Error rate
  - Endpoint performance

- **System Metrics:**
  - CPU usage
  - Memory consumption
  - Disk I/O
  - Network throughput

### Grafana Dashboards

1. **Network Overview**
   - Active users
   - Active networks
   - Total devices
   - Traffic statistics

2. **API Performance**
   - Request/response times
   - Error rates
   - Endpoint usage
   - Rate limiting

3. **VPN Metrics**
   - Connection status
   - Bandwidth graphs
   - Latency monitoring
   - Peer distribution

4. **Database Stats**
   - Query performance
   - Connection pool
   - Table sizes
   - Slow queries

---

## 🔧 Troubleshooting

### Common Issues

#### VPN Connection Failed
```bash
# Check WireGuard status
sudo wg show

# Verify firewall rules
sudo iptables -L

# Check backend logs
docker-compose logs backend

# Test network connectivity
ping 10.0.0.1
```

#### Desktop Client Won't Connect
```bash
# Check backend API
curl http://localhost:8080/health

# Verify WebSocket connection
# Check browser console for errors

# Reinstall client
# Uninstall via Control Panel
# Download latest installer
```

#### Database Connection Issues
```bash
# Check PostgreSQL status
docker-compose exec postgres pg_isready

# Verify credentials
docker-compose exec postgres psql -U swarmvpn -d swarmvpn

# Reset database
docker-compose down -v
docker-compose up -d
docker-compose exec backend ./swarmvpn migrate
```

#### File Upload Failures
```bash
# Check file size limits
cat .env | grep MAX_FILE_SIZE

# Verify upload directory permissions
docker-compose exec backend ls -la /app/uploads

# Check disk space
df -h
```

### Logs

```bash
# All services
docker-compose logs -f

# Backend only
docker-compose logs -f backend

# PostgreSQL
docker-compose logs -f postgres

# Redis
docker-compose logs -f redis
```

For more troubleshooting help, see [Full Documentation](F:\Docker\SwarmVPN\docs\TROUBLESHOOTING.md)

---

## 🤝 Contributing

Contributions welcome! See main [Swarm Tech README](../README.md) for guidelines.

### Development Areas

- **Linux Client** - Tauri Linux application
- **macOS Client** - Tauri macOS application
- **Mobile Apps** - React Native for Android/iOS
- **Additional P2P Actions** - Expand peer-to-peer features
- **Enhanced Monitoring** - More Grafana dashboards
- **Performance Optimization** - Backend and client improvements
- **Documentation** - API docs, tutorials, guides

---

## 📄 License

MIT License - see [LICENSE](../LICENSE)

Copyright (c) 2024-2025 NorthPeak (northpeak.app)

---

## 🔗 Links

- **Main Portfolio:** [Swarm Tech README](../README.md)
- **Company:** [NorthPeak](https://northpeak.app)
- **Project Location:** `F:\Docker\SwarmVPN`
- **Full Documentation:** `F:\Docker\SwarmVPN\docs\`
- **Support:** support@northpeak.app
- **Enterprise Sales:** enterprise@northpeak.app

---

<div align="center">

**Part of Swarm Tech Portfolio by NorthPeak**

[northpeak.app](https://northpeak.app) | [support@northpeak.app](mailto:support@northpeak.app)

Built with ❤️ by the NorthPeak Team

[⬆ Back to Top](#-swarmvpn)

</div>
