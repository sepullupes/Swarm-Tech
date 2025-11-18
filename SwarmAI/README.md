# 🤖 SwarmAI

<div align="center">

![SwarmAI Banner](https://img.shields.io/badge/SwarmAI-ChatGPT%20for%20n8n-ff69b4?style=for-the-badge)

**AI-Powered Workflow Automation Assistant**

*Part of Swarm Tech Portfolio by NorthPeak*

[![Status](https://img.shields.io/badge/Status-Beta%2099%25-orange?style=flat-square)](README.md)
[![Security](https://img.shields.io/badge/Security-Fixes%20Required-red?style=flat-square)](README.md)
[![Test Coverage](https://img.shields.io/badge/Coverage-80%25%2B-success?style=flat-square)](README.md)

[Features](#-core-features) • [Tech Stack](#-technology-stack) • [Setup](#-installation--setup) • [Workflows](#-workflow-types) • [Security](#-security-warnings)

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Project Status](#-project-status)
- [Core Features](#-core-features)
- [Technology Stack](#-technology-stack)
- [Workflow Types](#-workflow-types)
- [Architecture](#-architecture)
- [Installation & Setup](#-installation--setup)
- [AI Providers](#-ai-providers)
- [Security Warnings](#-security-warnings)
- [API Documentation](#-api-documentation)
- [Usage Examples](#-usage-examples)
- [Troubleshooting](#-troubleshooting)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🌟 Overview

**SwarmAI** is an intelligent workflow automation assistant that brings ChatGPT-like natural language capabilities to n8n workflow automation. Simply describe what you want to automate in plain English, and SwarmAI generates, manages, and executes complex n8n workflows automatically.

### Why SwarmAI?

- **💬 Natural Language** - Describe workflows in plain English
- **🔄 26+ Workflow Types** - Pre-built automation templates
- **🤖 Dual AI Providers** - OLLAMA (local) + OpenRouter (cloud)
- **⚡ Instant Execution** - Generate and run workflows immediately
- **🔧 Auto-Optimization** - AI improves workflows over time
- **📊 Smart Analytics** - Track workflow performance
- **🔒 Local & Cloud** - Choose between privacy and power

### Use Cases

- **Email Automation** - Auto-respond, filter, and organize emails
- **Data Processing** - ETL workflows with AI enhancement
- **Social Media** - Auto-posting and engagement monitoring
- **Notifications** - Smart alerting and notification routing
- **API Integration** - Connect services with natural language
- **Report Generation** - Automated data reports
- **Task Automation** - Repetitive task elimination

---

## 📊 Project Status

> ⚠️ **Beta - Security Fixes Required** - 99% complete, critical security patches needed before production

| Component | Status | Progress | Production Ready |
|-----------|--------|----------|------------------|
| Core AI Engine | ✅ Complete | 100% | ⚠️ Security Fixes |
| Workflow Generator | ✅ Complete | 100% | ⚠️ Security Fixes |
| n8n Integration | ✅ Complete | 100% | ⚠️ Security Fixes |
| OLLAMA Provider | ✅ Complete | 100% | ✅ Yes |
| OpenRouter Provider | ✅ Complete | 100% | ⚠️ Security Fixes |
| User Interface | ✅ Complete | 95% | ⚠️ Security Fixes |
| API Layer | ✅ Complete | 100% | ⚠️ Security Fixes |
| Test Coverage | ✅ Complete | 80%+ | ✅ Yes |
| Security Hardening | 🔴 Critical | 60% | ❌ No |

**Latest Update:** January 2025
**Expected Production:** Q2 2025 (after security fixes)

> ⚠️ **SECURITY WARNING - DO NOT DEPLOY TO PRODUCTION**
>
> This project contains known security vulnerabilities that must be fixed before deployment.
> This documentation is for portfolio purposes only.

### Critical Security Issues

1. **API Key Exposure** - Sensitive keys not properly encrypted
2. **SQL Injection** - Some inputs need better sanitization
3. **Rate Limiting** - Missing rate limits on AI endpoints
4. **Authentication** - JWT refresh token vulnerabilities
5. **CORS Configuration** - Overly permissive CORS settings

> ⚠️ **DO NOT DEPLOY TO PRODUCTION** until security patches are applied!

---

## 🚀 Core Features

### Natural Language Workflow Creation

Simply describe what you want in natural language:

```
"Send me a Slack notification every day at 9 AM with yesterday's sales data from Stripe"
```

SwarmAI automatically:
1. Understands the intent
2. Generates n8n workflow JSON
3. Configures all nodes and connections
4. Sets up schedules and triggers
5. Deploys and activates workflow

### 26+ Pre-Built Workflow Types

#### Communication & Notifications
1. **Email Automation** - Auto-respond, filter, forward
2. **Slack Integration** - Notifications, bots, alerts
3. **SMS Alerts** - Twilio SMS automation
4. **Discord Bots** - Auto-moderation, notifications
5. **Telegram Bots** - Message automation

#### Data & Analytics
6. **Database Sync** - PostgreSQL, MongoDB, MySQL sync
7. **CSV Processing** - Import, transform, export
8. **Report Generation** - Automated PDF/Excel reports
9. **Data Cleaning** - AI-powered data normalization
10. **API Polling** - Regular API data fetching

#### Social Media
11. **Twitter/X Automation** - Auto-posting, engagement
12. **LinkedIn Posts** - Schedule and publish content
13. **Instagram Management** - Post scheduling
14. **Facebook Automation** - Page management

#### E-commerce
15. **Order Processing** - WooCommerce, Shopify automation
16. **Inventory Sync** - Multi-platform inventory updates
17. **Price Monitoring** - Competitor price tracking
18. **Customer Notifications** - Order status updates

#### DevOps & Monitoring
19. **Server Monitoring** - Health checks and alerts
20. **GitHub Automation** - Issue management, PR automation
21. **Deployment Pipelines** - CI/CD workflow triggers
22. **Error Tracking** - Sentry, Bugsnag integration

#### Business Automation
23. **CRM Sync** - Salesforce, HubSpot integration
24. **Invoice Generation** - Automated billing
25. **Meeting Scheduling** - Calendar integration
26. **Lead Nurturing** - Automated follow-ups

### AI-Powered Features

- **Workflow Optimization** - AI suggests improvements
- **Error Resolution** - Auto-fix common workflow errors
- **Smart Scheduling** - Optimal execution timing
- **Data Transformation** - AI-assisted data mapping
- **Natural Language Queries** - Query workflow data conversationally
- **Predictive Analytics** - Forecast workflow outcomes

### Workflow Management

- **Visual Editor** - n8n's drag-and-drop interface
- **Version Control** - Track workflow changes
- **Templates** - Save and reuse custom workflows
- **Cloning** - Duplicate and modify workflows
- **Import/Export** - Share workflows as JSON
- **Testing** - Dry-run before activation

### Multi-Provider AI

#### OLLAMA (Local AI)
- **Privacy First** - All data stays local
- **No API Costs** - Free to run
- **Fast Response** - Low latency
- **Offline Capable** - Works without internet
- **Supported Models:**
  - Llama 2 (7B, 13B, 70B)
  - Mistral (7B)
  - CodeLlama
  - Vicuna
  - And 20+ more

#### OpenRouter (Cloud AI)
- **Multiple Models** - Access to 50+ AI models
- **High Quality** - GPT-4, Claude, PaLM 2
- **Scalability** - Handle high workloads
- **Latest Models** - Always up-to-date
- **Supported Models:**
  - GPT-4, GPT-3.5 Turbo
  - Claude 2, Claude Instant
  - PaLM 2
  - Llama 2 (via cloud)

---

## 🛠️ Technology Stack

### Backend
- **Node.js 18+** - JavaScript runtime
- **Express.js** - Web framework
- **TypeScript** - Type-safe development
- **PostgreSQL 14+** - Primary database
- **Redis** - Caching and session management

### AI & Automation
- **n8n** - Workflow automation platform
- **OLLAMA** - Local LLM deployment
- **OpenRouter** - Multi-model AI router
- **LangChain** - LLM orchestration framework
- **tiktoken** - Token counting for LLMs

### API & Integration
- **Axios** - HTTP client
- **Bull** - Queue management
- **Node-cron** - Job scheduling
- **Socket.io** - Real-time updates

### Authentication & Security
- **JWT** - Authentication tokens
- **bcrypt** - Password hashing
- **Helmet** - Security headers
- **Rate Limiting** - API protection (needs fixes)

### Testing
- **Jest** - Unit and integration testing
- **Supertest** - API endpoint testing
- **Mock Service Worker** - API mocking
- **Test Coverage:** 80%+

### Monitoring
- **Winston** - Logging
- **Morgan** - HTTP request logging
- **PM2** - Process management

---

## 🔄 Workflow Types

### 1. Email Automation

**Example Request:**
```
"Forward all emails from billing@company.com to accounting@company.com"
```

**Generated Workflow:**
- Email Trigger (IMAP)
- Filter Node (sender = billing@company.com)
- Email Node (forward to accounting@company.com)

### 2. Slack Notifications

**Example Request:**
```
"Send me a Slack message when a new row is added to my PostgreSQL users table"
```

**Generated Workflow:**
- PostgreSQL Trigger (watch for new rows)
- Transform Data Node
- Slack Node (send message)

### 3. Data Processing

**Example Request:**
```
"Import CSV from Google Drive, clean the data, and save to PostgreSQL"
```

**Generated Workflow:**
- Google Drive Trigger
- CSV Parser Node
- Data Cleaning Node (AI)
- PostgreSQL Insert Node

### 4. Social Media Posting

**Example Request:**
```
"Post to Twitter and LinkedIn every Monday at 10 AM with content from my blog RSS feed"
```

**Generated Workflow:**
- Schedule Trigger (Cron: 0 10 * * 1)
- RSS Feed Node
- Content Formatter Node
- Twitter Node
- LinkedIn Node

### 5. API Integration

**Example Request:**
```
"Fetch new orders from Shopify every hour and create invoices in QuickBooks"
```

**Generated Workflow:**
- Schedule Trigger (hourly)
- Shopify Node (get new orders)
- Transform Data Node
- QuickBooks Node (create invoice)
- Slack Notification Node (confirmation)

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────┐
│                SwarmAI Frontend (React)                 │
│  ┌───────────────────────────────────────────────────┐ │
│  │  Chat Interface  │  Workflow List  │  Settings   │ │
│  └───────────────────────────────────────────────────┘ │
└─────────────────────────────────────────────────────────┘
                         │
                         ▼ (HTTP/WebSocket)
┌─────────────────────────────────────────────────────────┐
│             SwarmAI Backend (Node.js/Express)           │
│  ┌───────────────────────────────────────────────────┐ │
│  │  REST API                                         │ │
│  │  - Chat Endpoint    - Workflow CRUD               │ │
│  │  - Execution        - Analytics                   │ │
│  └───────────────────────────────────────────────────┘ │
│  ┌───────────────────────────────────────────────────┐ │
│  │  AI Orchestration Layer                           │ │
│  │  - Intent Recognition                             │ │
│  │  - Workflow Generation                            │ │
│  │  - n8n JSON Builder                               │ │
│  └───────────────────────────────────────────────────┘ │
└─────────────────────────────────────────────────────────┘
                         │
        ┌────────────────┼────────────────┐
        │                │                │
        ▼                ▼                ▼
┌──────────────┐  ┌──────────────┐  ┌──────────────┐
│   OLLAMA     │  │  OpenRouter  │  │     n8n      │
│   (Local)    │  │   (Cloud)    │  │  Automation  │
│              │  │              │  │              │
│  - Llama 2   │  │  - GPT-4     │  │  - Execute   │
│  - Mistral   │  │  - Claude    │  │  - Monitor   │
│  - CodeLlama │  │  - PaLM 2    │  │  - Schedule  │
└──────────────┘  └──────────────┘  └──────────────┘
        │                │                │
        └────────────────┼────────────────┘
                         │
        ┌────────────────┼────────────────┐
        │                │                │
        ▼                ▼                ▼
┌──────────────┐  ┌──────────────┐  ┌──────────────┐
│  PostgreSQL  │  │    Redis     │  │   Storage    │
│              │  │              │  │              │
│  - Users     │  │  - Sessions  │  │  - Workflows │
│  - Workflows │  │  - Cache     │  │  - Logs      │
│  - Executions│  │  - Queue     │  │  - Analytics │
└──────────────┘  └──────────────┘  └──────────────┘
```

---

## 📦 Installation & Setup

### Prerequisites

```bash
# Required
Node.js v18+ LTS
npm v9+
PostgreSQL 14+
Redis 7+
n8n (latest version)

# AI Provider (choose one or both)
OLLAMA (for local AI)
OpenRouter API Key (for cloud AI)
```

### Method 1: Quick Start with OLLAMA (Local)

1. **Install OLLAMA**
   ```bash
   # Linux/Mac
   curl https://ollama.ai/install.sh | sh

   # Windows
   # Download from https://ollama.ai/download
   ```

2. **Pull AI Model**
   ```bash
   ollama pull llama2
   # or
   ollama pull mistral
   ```

3. **Navigate to Project**
   ```bash
   cd D:\source\AI\SwarmAI
   ```

4. **Install Dependencies**
   ```bash
   npm install
   ```

5. **Configure Environment**

   Create `.env` file:
   ```env
   NODE_ENV=development
   PORT=3000

   # PostgreSQL
   DATABASE_URL=postgresql://username:password@localhost:5432/swarm_ai

   # Redis
   REDIS_HOST=localhost
   REDIS_PORT=6379

   # JWT
   JWT_SECRET=your-super-secret-key-change-this
   JWT_EXPIRES_IN=7d

   # AI Provider - OLLAMA
   AI_PROVIDER=ollama
   OLLAMA_URL=http://localhost:11434
   OLLAMA_MODEL=llama2

   # n8n Integration
   N8N_URL=http://localhost:5678
   N8N_API_KEY=your-n8n-api-key

   # Optional: OpenRouter (for cloud AI)
   # OPENROUTER_API_KEY=sk-or-v1-xxxxxxxxxxxxxxxx (Get from OpenRouter)
   # OPENROUTER_MODEL=openai/gpt-4
   ```

6. **Setup Database**
   ```bash
   npm run migrate
   npm run seed
   ```

7. **Install & Start n8n**
   ```bash
   # Install n8n globally
   npm install -g n8n

   # Start n8n
   n8n start
   ```

8. **Start SwarmAI**
   ```bash
   npm run dev
   ```

9. **Access SwarmAI**
   - SwarmAI: http://localhost:3000
   - n8n: http://localhost:5678

### Method 2: OpenRouter (Cloud AI)

1. **Get OpenRouter API Key**
   - Visit https://openrouter.ai
   - Sign up and get API key

2. **Configure .env**
   ```env
   AI_PROVIDER=openrouter
   OPENROUTER_API_KEY=sk-or-xxxxx
   OPENROUTER_MODEL=openai/gpt-4
   ```

3. **Follow steps 3-9 from Method 1**

### Method 3: Hybrid (Both Local & Cloud)

Use OLLAMA for testing, OpenRouter for production:

```env
AI_PROVIDER=hybrid
OLLAMA_URL=http://localhost:11434
OLLAMA_MODEL=llama2
OPENROUTER_API_KEY=sk-or-xxxxx
OPENROUTER_MODEL=openai/gpt-4
AI_FALLBACK=openrouter  # Fallback if OLLAMA fails
```

### Default Credentials

```
Email: admin@swarm.ai
Password: [Must be set during installation]
```

---

## 🤖 AI Providers

### OLLAMA (Recommended for Development)

**Advantages:**
- ✅ Free and open source
- ✅ Privacy-focused (all local)
- ✅ No API costs
- ✅ Fast response times
- ✅ Offline capable

**Disadvantages:**
- ❌ Requires powerful hardware (8GB+ RAM)
- ❌ Limited model capabilities vs GPT-4
- ❌ Setup complexity

**Recommended Models:**
```bash
# Balanced (7B parameters)
ollama pull llama2
ollama pull mistral

# Code-focused
ollama pull codellama

# Larger (better quality, more resources)
ollama pull llama2:13b
ollama pull llama2:70b
```

### OpenRouter (Recommended for Production)

**Advantages:**
- ✅ Access to GPT-4, Claude, etc.
- ✅ Best AI quality
- ✅ No hardware requirements
- ✅ Simple setup
- ✅ Multiple model options

**Disadvantages:**
- ❌ Costs money per request
- ❌ Requires internet
- ❌ Privacy concerns (data sent to cloud)

**Pricing (approximate):**
- GPT-3.5 Turbo: $0.002 per 1K tokens
- GPT-4: $0.03 per 1K tokens
- Claude 2: $0.008 per 1K tokens

**Popular Models:**
```env
# Fast and cheap
OPENROUTER_MODEL=openai/gpt-3.5-turbo

# Best quality
OPENROUTER_MODEL=openai/gpt-4

# Anthropic Claude
OPENROUTER_MODEL=anthropic/claude-2

# Google PaLM
OPENROUTER_MODEL=google/palm-2-chat
```

---

## ⚠️ Security Warnings

### Critical Issues (Must Fix Before Production)

#### 1. API Key Exposure
**Issue:** Sensitive API keys stored in plain text in database

**Fix Required:**
```javascript
// Before (vulnerable)
await db.query('INSERT INTO api_keys VALUES ($1)', [apiKey]);

// After (secure)
const encrypted = await encrypt(apiKey, process.env.ENCRYPTION_KEY);
await db.query('INSERT INTO api_keys VALUES ($1)', [encrypted]);
```

#### 2. SQL Injection Vulnerability
**Issue:** User input not properly sanitized in workflow queries

**Fix Required:**
```javascript
// Before (vulnerable)
const query = `SELECT * FROM workflows WHERE name = '${userInput}'`;

// After (secure)
const query = 'SELECT * FROM workflows WHERE name = $1';
await db.query(query, [userInput]);
```

#### 3. Missing Rate Limiting
**Issue:** AI endpoints can be abused

**Fix Required:**
```javascript
const rateLimit = require('express-rate-limit');

const aiLimiter = rateLimit({
  windowMs: 15 * 60 * 1000, // 15 minutes
  max: 100 // limit each IP to 100 requests per windowMs
});

app.use('/api/ai', aiLimiter);
```

#### 4. JWT Refresh Token Issues
**Issue:** Refresh tokens not properly rotated

**Fix Required:**
- Implement token rotation
- Add token blacklisting
- Set shorter expiration times

#### 5. CORS Misconfiguration
**Issue:** CORS allows all origins

**Fix Required:**
```javascript
// Before (vulnerable)
app.use(cors({ origin: '*' }));

// After (secure)
app.use(cors({
  origin: process.env.ALLOWED_ORIGINS.split(','),
  credentials: true
}));
```

### Security Checklist

- [ ] Encrypt all API keys in database
- [ ] Sanitize all user inputs
- [ ] Implement rate limiting
- [ ] Fix JWT refresh token rotation
- [ ] Configure CORS properly
- [ ] Add input validation middleware
- [ ] Enable HTTPS in production
- [ ] Implement CSP headers
- [ ] Add audit logging
- [ ] Regular security audits

---

## 📚 API Documentation

### Generate Workflow from Natural Language

```http
POST /api/ai/generate-workflow
Authorization: Bearer {token}
Content-Type: application/json

{
  "prompt": "Send me an email every morning at 8 AM with yesterday's GitHub commits",
  "provider": "ollama",
  "model": "llama2"
}
```

**Response:**
```json
{
  "success": true,
  "workflow": {
    "id": "workflow-uuid",
    "name": "Daily GitHub Commits Email",
    "n8nWorkflow": {
      "nodes": [...],
      "connections": {...}
    },
    "deployed": true,
    "active": true
  }
}
```

### List Workflows

```http
GET /api/workflows?page=1&limit=20
Authorization: Bearer {token}
```

### Execute Workflow

```http
POST /api/workflows/:id/execute
Authorization: Bearer {token}
```

### Full API Documentation

Swagger docs: http://localhost:3000/api-docs

---

## 💡 Usage Examples

### Example 1: Email to Slack

**User Input:**
```
"When I receive an email with 'urgent' in the subject, send it to #urgent channel in Slack"
```

**SwarmAI Response:**
```
I've created a workflow called "Urgent Email to Slack" with:
1. Email trigger monitoring your inbox
2. Filter for emails containing 'urgent' in subject
3. Slack notification to #urgent channel

The workflow is now active!
```

### Example 2: Database Backup

**User Input:**
```
"Backup my PostgreSQL database every night at 2 AM and upload to Google Drive"
```

**SwarmAI Response:**
```
Created "Nightly Database Backup" workflow:
1. Cron trigger (2 AM daily)
2. PostgreSQL dump command
3. Compress to ZIP
4. Upload to Google Drive /backups folder

Scheduled successfully!
```

### Example 3: Social Media Automation

**User Input:**
```
"Post my latest blog article to Twitter, LinkedIn, and Facebook when I publish on WordPress"
```

**SwarmAI Response:**
```
Built "Blog Auto-Poster" workflow:
1. WordPress webhook trigger
2. Extract article title, excerpt, link
3. Twitter post with hashtags
4. LinkedIn post with professional tone
5. Facebook page post

Workflow activated and ready!
```

---

## 🔧 Troubleshooting

### OLLAMA Connection Failed

```bash
# Check if OLLAMA is running
curl http://localhost:11434/api/tags

# Restart OLLAMA
# Linux/Mac
sudo systemctl restart ollama

# Windows
# Restart from Task Manager or Services
```

### n8n Integration Not Working

```bash
# Get n8n API key
# Login to n8n → Settings → API

# Test connection
curl http://localhost:5678/api/v1/workflows \
  -H "X-N8N-API-KEY: your-api-key"
```

### PostgreSQL Connection Issues

```bash
# Test connection
psql -h localhost -U swarm -d swarm_ai

# Reset database
npm run migrate:reset
npm run seed
```

---

## 🤝 Contributing

**Priority Areas:**
- 🔒 Security fixes (CRITICAL)
- 🧪 Test coverage improvements
- 📝 Documentation
- 🎨 UI/UX enhancements
- 🤖 More workflow templates

See [main portfolio](../README.md) for guidelines.

---

## 📄 License

MIT License - see [LICENSE](../LICENSE)

Copyright (c) 2024-2025 NorthPeak (northpeak.app)

---

## 🔗 Links

- **Main Portfolio:** [Swarm Tech README](../README.md)
- **Company:** [NorthPeak](https://northpeak.app)
- **Project Location:** `D:\source\AI\SwarmAI`
- **n8n Documentation:** https://docs.n8n.io
- **OLLAMA:** https://ollama.ai
- **OpenRouter:** https://openrouter.ai
- **Support:** support@northpeak.app

---

<div align="center">

**⚠️ SECURITY NOTICE: DO NOT USE IN PRODUCTION UNTIL SECURITY FIXES ARE APPLIED ⚠️**

---

**Part of Swarm Tech Portfolio by NorthPeak**

[northpeak.app](https://northpeak.app) | [support@northpeak.app](mailto:support@northpeak.app)

Built with ❤️ by the NorthPeak Team

[⬆ Back to Top](#-swarmai)

</div>
