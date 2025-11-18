# 🕷️ ScrutNest

<div align="center">

![ScrutNest Banner](https://img.shields.io/badge/ScrutNest-Web%20Scraping%20Platform-purple?style=for-the-badge)

**AI-Powered Web Scraping & Data Extraction Platform**

*Part of Swarm Tech Portfolio by NorthPeak*

[![Status](https://img.shields.io/badge/Status-Foundation%2030%25-yellow?style=flat-square)](README.md)
[![Tech Stack](https://img.shields.io/badge/Stack-React%20%7C%20Node.js%20%7C%20PostgreSQL-blue?style=flat-square)](README.md)
[![Test Coverage](https://img.shields.io/badge/Coverage-10%25-red?style=flat-square)](README.md)

[Features](#-core-features) • [Tech Stack](#-technology-stack) • [Setup](#-installation--setup) • [Scrapers](#-scraper-types) • [Roadmap](#-development-roadmap)

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Project Status](#-project-status)
- [Core Features](#-core-features)
- [Technology Stack](#-technology-stack)
- [Scraper Types](#-scraper-types)
- [Architecture](#-architecture)
- [Installation & Setup](#-installation--setup)
- [AI Capabilities](#-ai-capabilities)
- [Data Visualization](#-data-visualization)
- [Use Cases](#-use-cases)
- [Development Roadmap](#-development-roadmap)
- [API Documentation](#-api-documentation)
- [Troubleshooting](#-troubleshooting)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🌟 Overview

**ScrutNest** is an intelligent web scraping and data extraction platform that combines traditional scraping techniques with AI-powered enhancement. Built for data scientists, researchers, and businesses, ScrutNest provides a visual workflow builder, multi-source scraping capabilities, and advanced data processing pipelines.

### Why ScrutNest?

- **🤖 AI-Powered Selectors** - Automatically identify data patterns
- **🎨 Visual Workflow Builder** - Drag-and-drop scraping workflows
- **📊 Real-time Visualization** - D3.js powered data dashboards
- **🔄 Multi-Source Scraping** - Extract from 8+ different sources
- **⚡ High Performance** - Concurrent scraping with rate limiting
- **🛡️ Anti-Detection** - Proxy rotation and browser fingerprinting
- **💾 Data Pipeline** - ETL workflows for data processing

### Use Cases

- **Market Research** - Competitor pricing and product monitoring
- **Lead Generation** - Business contact information extraction
- **Price Monitoring** - E-commerce price tracking and alerts
- **News Aggregation** - Real-time news and content collection
- **Social Media** - Social media data extraction and analysis
- **Academic Research** - Large-scale data collection for research
- **SEO Analysis** - SERP tracking and keyword monitoring
- **Real Estate** - Property listing aggregation

---

## 📊 Project Status

> ⚠️ **Work in Progress** - ScrutNest is in early development (30% complete)

| Component | Status | Progress | Production Ready |
|-----------|--------|----------|------------------|
| Core Scraping Engine | 🟡 In Progress | 60% | ❌ No |
| Visual Workflow Builder | 🟡 In Progress | 40% | ❌ No |
| AI Selector Engine | 🔴 Planned | 20% | ❌ No |
| Data Pipeline | 🟡 In Progress | 50% | ❌ No |
| Dashboard & UI | 🟡 In Progress | 35% | ❌ No |
| API Layer | 🟡 In Progress | 45% | ❌ No |
| Proxy Management | 🔴 Planned | 15% | ❌ No |
| Scheduling System | 🔴 Planned | 10% | ❌ No |
| Data Visualization | 🟡 In Progress | 30% | ❌ No |

**Latest Update:** January 2025
**Expected Beta:** Q4 2025
**Production Release:** Q1 2026

---

## 🚀 Core Features

### Scraping Capabilities

#### Multi-Source Scraping (8+ Types)
1. **Static HTML Scraping** - Traditional DOM parsing
2. **Dynamic JavaScript Sites** - Puppeteer/Playwright rendering
3. **API Scraping** - REST API data extraction
4. **Social Media** - Facebook, Twitter, LinkedIn, Instagram
5. **E-commerce** - Amazon, eBay, Shopify stores
6. **News Sites** - Article extraction with NLP
7. **Search Engines** - Google, Bing SERP scraping
8. **Custom Sources** - User-defined scrapers

#### Advanced Features
- **Pagination Handling** - Auto-detect and navigate pagination
- **Infinite Scroll** - Handle infinite scroll pages
- **Login & Authentication** - Scrape authenticated content
- **CAPTCHA Solving** - Integration with solving services
- **Rate Limiting** - Respect robots.txt and custom limits
- **Error Handling** - Retry logic and fallback strategies

### AI-Powered Enhancement

- **Smart Selectors** - AI identifies optimal CSS/XPath selectors
- **Data Pattern Recognition** - Automatically detect data structures
- **Content Classification** - Categorize extracted content
- **Data Validation** - AI-powered data quality checks
- **Anomaly Detection** - Identify unusual patterns in data
- **Auto-Repair** - Fix broken selectors automatically

### Visual Workflow Builder

- **Drag-and-Drop Interface** - No-code scraping workflow creation
- **Node-Based System** - Connect scraping steps visually
- **Template Library** - Pre-built workflow templates
- **Live Preview** - Real-time scraping preview
- **Version Control** - Track workflow changes
- **Import/Export** - Share workflows with team

### Data Processing Pipeline

- **Data Cleaning** - Remove duplicates, normalize formats
- **Transformation** - Apply custom data transformations
- **Enrichment** - Enhance data with additional sources
- **Validation** - Schema validation and quality checks
- **Storage** - PostgreSQL, MongoDB, CSV, JSON exports
- **API Export** - Webhook delivery to external systems

### Scheduling & Automation

- **Cron Scheduling** - Schedule scraping jobs
- **Event-Driven** - Trigger on data changes or webhooks
- **Monitoring** - Real-time job monitoring and alerts
- **Retry Logic** - Automatic retry on failures
- **Resource Management** - CPU and memory optimization
- **Queue System** - Bull queue for job management

### Data Visualization

- **Interactive Dashboards** - D3.js powered visualizations
- **Custom Charts** - Line, bar, pie, scatter plots
- **Trend Analysis** - Historical data visualization
- **Comparison Tools** - Compare data across sources
- **Export Options** - PNG, SVG, PDF exports
- **Real-time Updates** - Live data visualization

---

## 🛠️ Technology Stack

### Frontend
- **React 18** - Modern UI framework
- **Redux Toolkit** - State management
- **D3.js** - Data visualization library
- **React Flow** - Workflow diagram builder
- **Material-UI** - Component library
- **Monaco Editor** - Code editor for selectors
- **Recharts** - Additional charting library

### Backend
- **Node.js 18+** - JavaScript runtime
- **Express.js** - Web framework
- **TypeScript** - Type-safe development
- **Bull** - Queue management for jobs
- **Node-cron** - Job scheduling

### Scraping Technologies
- **Puppeteer** - Headless Chrome automation
- **Playwright** - Cross-browser automation
- **Cheerio** - Fast HTML parsing
- **Axios** - HTTP client for API scraping
- **jsdom** - JavaScript DOM implementation

### Databases
- **PostgreSQL 14+** - Primary relational database
  - User data, workflows, jobs
  - Scraped data storage
  - Analytics and metrics
- **Redis 7+** - Caching and queue management
  - Job queues
  - Rate limiting
  - Session caching
  - Real-time data

### AI & ML (Planned)
- **TensorFlow.js** - ML models in browser/Node.js
- **Natural** - NLP for content extraction
- **Brain.js** - Neural networks for pattern recognition
- **OpenAI API** - GPT integration for smart parsing

### Proxy & Anti-Detection
- **Proxy Rotation** - Rotate through proxy pools
- **User-Agent Rotation** - Randomize browser signatures
- **Cookie Management** - Session persistence
- **Browser Fingerprinting** - Mimic real browsers

### Data Processing
- **Papa Parse** - CSV parsing and generation
- **json2csv** - JSON to CSV conversion
- **Lodash** - Data manipulation utilities
- **Joi** - Data validation

### Monitoring & Logging
- **Winston** - Logging framework
- **Prometheus** - Metrics collection (planned)
- **Grafana** - Metrics visualization (planned)
- **Sentry** - Error tracking

---

## 🕷️ Scraper Types

### 1. Static HTML Scraper
**Status:** ✅ Complete (60%)

Extract data from traditional server-rendered HTML pages.

**Features:**
- CSS and XPath selectors
- Multi-element extraction
- Attribute extraction
- Text content and HTML extraction

**Example:**
```javascript
{
  "type": "static",
  "url": "https://example.com",
  "selectors": {
    "title": "h1.product-title",
    "price": "span.price",
    "description": "div.description"
  }
}
```

### 2. Dynamic JavaScript Scraper
**Status:** 🟡 In Progress (40%)

Scrape JavaScript-heavy single-page applications.

**Features:**
- Full browser automation
- Wait for dynamic content
- Scroll and pagination handling
- Screenshot capture

**Technologies:**
- Puppeteer
- Playwright

### 3. API Scraper
**Status:** 🟡 In Progress (50%)

Extract data from REST APIs and GraphQL endpoints.

**Features:**
- Authentication handling (Bearer, API keys)
- Request/response transformation
- Rate limiting
- Pagination support

### 4. Social Media Scrapers
**Status:** 🔴 Planned (10%)

Extract data from social media platforms.

**Supported Platforms:**
- Facebook (posts, profiles, groups)
- Twitter/X (tweets, profiles, hashtags)
- LinkedIn (profiles, jobs, companies)
- Instagram (posts, profiles, hashtags)

### 5. E-commerce Scrapers
**Status:** 🔴 Planned (15%)

Specialized scrapers for e-commerce platforms.

**Supported Platforms:**
- Amazon (products, reviews, prices)
- eBay (listings, sold items)
- Shopify stores
- WooCommerce sites

### 6. News & Content Scrapers
**Status:** 🟡 In Progress (30%)

Extract articles and news content with NLP.

**Features:**
- Article content extraction
- Author and date detection
- Category classification
- Related articles extraction

### 7. Search Engine Scrapers
**Status:** 🔴 Planned (5%)

SERP (Search Engine Results Page) scraping.

**Supported Engines:**
- Google Search
- Bing Search
- DuckDuckGo

### 8. Custom Scrapers
**Status:** 🟡 In Progress (35%)

User-defined custom scraping logic.

**Features:**
- JavaScript code editor
- Custom transformation functions
- Import npm packages
- Test and debug mode

---

## 🏗️ Architecture

### System Architecture

```
┌────────────────────────────────────────────────────────┐
│              ScrutNest Frontend (React)                │
│  ┌──────────────────────────────────────────────────┐ │
│  │  Workflow Builder    │   Dashboard   │   Jobs   │ │
│  └──────────────────────────────────────────────────┘ │
└────────────────────────────────────────────────────────┘
                         │
                         ▼ (HTTP/WebSocket)
┌────────────────────────────────────────────────────────┐
│              Backend API (Node.js/Express)             │
│  ┌──────────────────────────────────────────────────┐ │
│  │  REST API                                        │ │
│  │  - Workflow Management   - Job Control          │ │
│  │  - Data Export           - User Management      │ │
│  └──────────────────────────────────────────────────┘ │
└────────────────────────────────────────────────────────┘
                         │
        ┌────────────────┼────────────────┐
        │                │                │
        ▼                ▼                ▼
┌──────────────┐  ┌──────────────┐  ┌──────────────┐
│   Scraping   │  │    Data      │  │   Scheduler  │
│    Engine    │  │  Pipeline    │  │   Service    │
│              │  │              │  │              │
│  - Puppeteer │  │  - Clean     │  │  - Cron Jobs │
│  - Cheerio   │  │  - Transform │  │  - Queue Mgmt│
│  - Axios     │  │  - Validate  │  │  - Bull      │
└──────────────┘  └──────────────┘  └──────────────┘
        │                │                │
        └────────────────┼────────────────┘
                         │
        ┌────────────────┼────────────────┐
        │                │                │
        ▼                ▼                ▼
┌──────────────┐  ┌──────────────┐  ┌──────────────┐
│  PostgreSQL  │  │    Redis     │  │  AI Service  │
│              │  │              │  │  (Planned)   │
│  - Workflows │  │  - Queues    │  │              │
│  - Jobs      │  │  - Cache     │  │  - Selectors │
│  - Data      │  │  - Sessions  │  │  - Patterns  │
└──────────────┘  └──────────────┘  └──────────────┘
```

---

## 📦 Installation & Setup

### Prerequisites

```bash
# Required
Node.js v18+ LTS
npm v9+ or yarn
PostgreSQL 14+
Redis 7+
Git

# Recommended
Docker & Docker Compose
Chrome/Chromium (for Puppeteer)
```

### Quick Start with Docker

1. **Navigate to Project Directory**
   ```bash
   cd D:\source\AI\ScrutNest
   ```

2. **Configure Environment**
   ```bash
   cp .env.example .env
   ```

3. **Start Services**
   ```bash
   docker-compose up -d
   ```

4. **Initialize Database**
   ```bash
   docker-compose exec api npm run migrate
   docker-compose exec api npm run seed
   ```

5. **Access ScrutNest**
   - Frontend: http://localhost:3000
   - API: http://localhost:5000
   - API Docs: http://localhost:5000/api-docs

### Manual Installation

1. **Install Dependencies**

   ```bash
   # Backend
   cd backend
   npm install

   # Frontend
   cd ../frontend
   npm install
   ```

2. **Setup PostgreSQL**

   ```sql
   CREATE DATABASE scrutnest;
   CREATE USER scrutnest WITH PASSWORD 'your_password';
   GRANT ALL PRIVILEGES ON DATABASE scrutnest TO scrutnest;
   ```

3. **Setup Redis**

   ```bash
   # Start Redis server
   redis-server
   ```

4. **Configure Environment**

   **backend/.env**
   ```env
   NODE_ENV=development
   PORT=5000

   # PostgreSQL
   DATABASE_URL=postgresql://scrutnest:password@localhost:5432/scrutnest

   # Redis
   REDIS_HOST=localhost
   REDIS_PORT=6379

   # JWT
   JWT_SECRET=your-super-secret-key
   JWT_EXPIRES_IN=7d

   # Puppeteer
   PUPPETEER_EXECUTABLE_PATH=/usr/bin/chromium-browser

   # Rate Limiting
   RATE_LIMIT_WINDOW_MS=60000
   RATE_LIMIT_MAX_REQUESTS=100

   # Proxy (Optional)
   PROXY_URL=http://proxy.example.com:8080
   PROXY_USERNAME=username
   PROXY_PASSWORD=password
   ```

5. **Run Migrations**
   ```bash
   cd backend
   npm run migrate
   npm run seed
   ```

6. **Start Services**

   ```bash
   # Terminal 1 - Backend
   cd backend
   npm run dev

   # Terminal 2 - Frontend
   cd frontend
   npm start
   ```

### Default Credentials

```
Email: admin@scrutnest.com
Password: [Set on first login]
```

---

## 🤖 AI Capabilities

### Smart Selector Generation (Planned)

AI analyzes page structure and suggests optimal selectors:

```javascript
// Traditional approach
const selector = 'div.container > ul > li.item > h3.title';

// AI-powered approach
const aiSelector = await ai.generateSelector({
  url: 'https://example.com',
  targetText: 'Product Title',
  context: 'e-commerce product listing'
});
// Returns: Robust selector that works even if HTML changes
```

### Pattern Recognition

Automatically detect data patterns:

- **Tables** - Detect and extract tabular data
- **Lists** - Identify list structures
- **Cards** - Recognize card-based layouts
- **Forms** - Extract form data

### Data Enhancement

- **Entity Recognition** - Identify people, places, organizations
- **Sentiment Analysis** - Analyze text sentiment
- **Language Detection** - Auto-detect content language
- **Content Summarization** - Generate summaries

---

## 📊 Data Visualization

### Available Visualizations

1. **Time Series Charts** - Track data changes over time
2. **Comparison Charts** - Compare data across sources
3. **Geospatial Maps** - Visualize location-based data
4. **Network Graphs** - Relationship visualization
5. **Heatmaps** - Intensity visualization
6. **Word Clouds** - Text data visualization

### Custom Dashboards

Build custom dashboards with drag-and-drop widgets:

- Real-time data updates
- Interactive filters
- Export to PDF/PNG
- Share with team members

---

## 💼 Use Cases

### E-commerce Price Monitoring

Monitor competitor prices across multiple stores:

```javascript
{
  "workflow": "price-monitor",
  "sources": [
    "https://amazon.com/product/123",
    "https://ebay.com/itm/456",
    "https://walmart.com/ip/789"
  ],
  "schedule": "0 */6 * * *", // Every 6 hours
  "alerts": {
    "priceChange": true,
    "threshold": 5 // 5% change triggers alert
  }
}
```

### Lead Generation

Extract business contact information:

```javascript
{
  "workflow": "lead-generation",
  "source": "https://directory.com",
  "extract": [
    "company_name",
    "email",
    "phone",
    "address",
    "website"
  ],
  "filters": {
    "industry": "Technology",
    "location": "San Francisco"
  }
}
```

---

## 🛣️ Development Roadmap

### Phase 1: Foundation (🟡 30% Complete)
- [x] Basic scraping engine (Cheerio + Puppeteer)
- [x] PostgreSQL database setup
- [x] REST API foundation
- [ ] Visual workflow builder (40%)
- [ ] Job queue system (50%)
- [ ] User authentication

### Phase 2: Core Features (🔴 Q2 2025)
- [ ] Complete workflow builder
- [ ] 8 scraper types implementation
- [ ] Data pipeline (clean, transform, validate)
- [ ] Dashboard and analytics
- [ ] API documentation
- [ ] Proxy management

### Phase 3: AI Integration (🔴 Q3 2025)
- [ ] AI selector generation
- [ ] Pattern recognition
- [ ] Auto-repair broken scrapers
- [ ] Data classification
- [ ] Anomaly detection

### Phase 4: Advanced Features (🔴 Q4 2025)
- [ ] CAPTCHA solving integration
- [ ] Advanced scheduling
- [ ] Team collaboration features
- [ ] API marketplace
- [ ] Mobile app (React Native)

### Phase 5: Production (🔴 Q1 2026)
- [ ] Performance optimization
- [ ] Security hardening
- [ ] Comprehensive testing
- [ ] Documentation completion
- [ ] Production deployment

---

## 📚 API Documentation

### Create Scraping Job

```http
POST /api/jobs
Authorization: Bearer {token}
Content-Type: application/json

{
  "name": "Amazon Price Scraper",
  "type": "ecommerce",
  "config": {
    "url": "https://amazon.com/product/123",
    "selectors": {
      "price": "span.price",
      "title": "h1#title"
    }
  },
  "schedule": "0 */2 * * *"
}
```

### Get Job Results

```http
GET /api/jobs/:jobId/results?page=1&limit=50
Authorization: Bearer {token}
```

### Full API Documentation

Available at: http://localhost:5000/api-docs (when running)

---

## 🔧 Troubleshooting

### Puppeteer Issues

```bash
# Install Chromium dependencies (Linux)
sudo apt-get install -y chromium-browser

# Windows - Use bundled Chromium
# No additional setup needed
```

### Memory Issues

Adjust Node.js memory limit:
```bash
NODE_OPTIONS="--max-old-space-size=4096" npm run dev
```

---

## 🤝 Contributing

We need help! Priority areas:

- 🎨 UI/UX design for workflow builder
- 🕷️ New scraper implementations
- 🤖 AI/ML integration
- 📝 Documentation
- 🧪 Testing

See [main portfolio](../README.md) for contribution guidelines.

---

## 📄 License

MIT License - see [LICENSE](../LICENSE)

Copyright (c) 2024-2025 NorthPeak (northpeak.app)

---

## 🔗 Links

- **Main Portfolio:** [Swarm Tech README](../README.md)
- **Company:** [NorthPeak](https://northpeak.app)
- **Project Location:** `D:\source\AI\ScrutNest`
- **Documentation:** [Full Docs](D:\source\AI\ScrutNest\docs)
- **Support:** support@northpeak.app

---

<div align="center">

**Part of Swarm Tech Portfolio by NorthPeak**

[northpeak.app](https://northpeak.app) | [support@northpeak.app](mailto:support@northpeak.app)

Built with ❤️ by the NorthPeak Team

[⬆ Back to Top](#-scrutnest)

</div>
