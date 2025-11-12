# EngageOS - Enterprise WhatsApp SaaS Platform

<div align="center">

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![PHP](https://img.shields.io/badge/PHP-8.4+-purple.svg)
![Laravel](https://img.shields.io/badge/Laravel-10.x-red.svg)
![Node.js](https://img.shields.io/badge/Node.js-18.x+-green.svg)
![License](https://img.shields.io/badge/license-Proprietary-orange.svg)

**The Most Comprehensive WhatsApp Messaging Platform for Enterprise**

*Campaign Management • Multi-Tenancy • Real-Time Analytics • GDPR Compliant*

[Features](#-key-features) • [Documentation](#-documentation) • [Quick Start](#-quick-start) • [Deployment](#-deployment-options) • [Tech Stack](#-tech-stack)

</div>

---

## 📖 About EngageOS

**EngageOS** is a production-ready, enterprise-grade WhatsApp SaaS platform that enables businesses, marketing agencies, and service providers to manage sophisticated WhatsApp messaging campaigns at scale. Built with Laravel and Node.js, EngageOS offers complete multi-tenancy, advanced campaign automation, real-time analytics, and comprehensive API integration.

### Why EngageOS?

- ✅ **100+ Features** across 14 major modules
- ✅ **Production-Ready** - Battle-tested in real businesses
- ✅ **Multi-Tenant** - Complete data isolation for multiple users/clients
- ✅ **Enterprise-Grade Security** - GDPR compliant with role-based access control
- ✅ **Modern Tech Stack** - Laravel 10, Node.js 18+, Redis, TailwindCSS
- ✅ **Comprehensive API** - RESTful API for seamless integrations
- ✅ **Real-Time Updates** - WebSocket support for live campaign monitoring
- ✅ **Anti-Ban Protection** - Human-like behavior prevents WhatsApp blocking

### Perfect For

- 🎯 Marketing agencies managing client campaigns
- 💼 Businesses requiring WhatsApp automation
- 🚀 SaaS entrepreneurs entering the messaging market
- 👨‍💻 Developers building custom communication solutions

---

## 🌟 Key Features

### 📊 Campaign Management
- **Advanced Campaign Builder** with scheduling and cloning
- **Smart Recipient Targeting** - Manual, lists, or combined
- **Real-Time Monitoring** - Live status tracking and analytics
- **Campaign States** - Draft, Running, Paused, Completed, Failed
- **Restart Capability** - Rerun campaigns with fresh statistics
- **Multi-User Support** - Track creators and execution history

### 📨 Message & Template System
- **Unlimited Message Templates** with variable substitution
- **Template Categories** - Marketing, Sales, Support, Follow-up
- **Live Preview** - See messages before sending
- **Multi-Provider Support** - WhatsApp (Baileys) + BulkSMS
- **Smart Variables** - {{first_name}}, {{phone}}, {{email}}, custom fields
- **Message Builder Service** - Auto header/footer, opt-out links

### 👥 Contact & List Management
- **Comprehensive Contact Database** with custom fields
- **CSV Import/Export** - Bulk operations with intelligent mapping
- **Static Lists** - Manual grouping and organization
- **Dynamic Lists** - Rule-based segmentation with AND/OR logic
- **Tagging System** - Categorize and filter contacts
- **Multi-User Isolation** - Complete data separation

### 🤖 Automation & Engagement
- **Auto-Reply System** - Keyword-based automated responses
- **Opt-Out Management** - GDPR-compliant subscription handling
- **Preference Center** - Self-service subscription management
- **Keyword Detection** - Auto-detect STOP, UNSUBSCRIBE commands
- **Queue System** - Redis/BullMQ for background processing
- **Anti-Ban Protection** - Random delays, typing indicators

### 👤 Multi-Tenancy & User Management
- **Multi-User System** - Super Admin and User roles
- **Complete Data Isolation** - Per-user contacts, campaigns, lists
- **Invitation System** - Email-based onboarding
- **User Impersonation** - Admin support capabilities
- **Activity Tracking** - Last login, usage statistics
- **Permission Management** - Role-based access control

### 🔌 API & Integrations
- **RESTful API** - Complete CRUD operations
- **API Key Management** - Secure token-based authentication
- **Webhook System** - Real-time event notifications
- **MCP Integration** - AI agent and automation support
- **Comprehensive Documentation** - API reference included
- **Rate Limiting** - Abuse prevention built-in

### 📱 WhatsApp Engine
- **WhatsApp Web Integration** - Baileys 7.x (most stable)
- **QR Code Authentication** - Simple phone scanning
- **Persistent Sessions** - Database-backed (no file storage issues)
- **Multi-Device Support** - Full WhatsApp multi-device support
- **Auto Reconnection** - Handles disconnects gracefully
- **Message Queue** - BullMQ for reliable message processing
- **Media Support** - Images, videos, documents, audio

### 📈 Analytics & Reporting
- **Real-Time Dashboard** - Campaign metrics and KPIs
- **Campaign Analytics** - Delivery, read, reply rates
- **Reply Management** - Centralized response tracking
- **Export Functionality** - CSV export for all data
- **Performance Metrics** - Success rates and engagement tracking
- **Visual Reports** - Chart-ready data structures

### 🎨 Modern UI/UX
- **Dark & Light Mode** - User preference support
- **Mobile Responsive** - Perfect on all devices
- **TailwindCSS Styling** - Modern, clean design
- **Real-Time Updates** - Live data without page refresh
- **Infinite Scroll** - Handle thousands of records smoothly
- **Toast Notifications** - Non-intrusive alerts

### 🔒 Security & Compliance
- **Authentication & Authorization** - Laravel Sanctum
- **Data Encryption** - Passwords, API keys, tokens
- **Rate Limiting** - API and endpoint protection
- **CSRF/XSS Protection** - Security built-in
- **GDPR Compliance** - Opt-out system, data export/deletion
- **Audit Logging** - Track user actions (framework ready)

### 📲 Progressive Web App (PWA)
- **Installable** - Add to home screen
- **Offline Support** - Service worker caching
- **Native Feel** - Standalone app mode
- **Push Notifications** - Browser notification support (ready)
- **App Shortcuts** - Quick actions from home screen

### ⚙️ System Configuration
- **Centralized Settings** - Company info, branding, variables
- **Provider Management** - Configure messaging providers
- **Service Status Dashboard** - Monitor system health (Super Admin)
- **Image Optimization** - Auto WebP/PNG conversion
- **Custom Variables** - Define reusable template variables

### 🛠️ Developer Features
- **Comprehensive Logging** - Laravel + Winston (Node.js)
- **Code Quality Tools** - Laravel Pint, PHPUnit
- **Deployment Automation** - One-command production deployment
- **Environment Validation** - Check requirements
- **Caching Optimization** - Config, route, view caching

---

## 🏗️ Tech Stack

### Backend
- **Laravel 10.x** (PHP 8.4) - Web application framework
- **MySQL 8.0+** / **MariaDB 10.5+** - Relational database
- **Redis 6.0+** - Caching and queue system
- **Laravel Sanctum** - API authentication
- **Livewire 3.x** - Reactive UI components
- **Intervention Image** - Image processing

### Frontend
- **TailwindCSS 3.x** - Utility-first CSS framework
- **Alpine.js 3.x** - Lightweight JavaScript framework
- **Livewire 3.x** - Server-side rendering with SPA experience
- **Socket.IO Client** - Real-time WebSocket communication

### WhatsApp Engine
- **Node.js 18.x+** - JavaScript runtime
- **Baileys 7.x** - WhatsApp Web API integration
- **Express.js** - Web server framework
- **Socket.IO Server** - WebSocket server
- **BullMQ** - Redis-based queue system
- **Winston** - Logging library
- **Axios** - HTTP client

### Infrastructure
- **Nginx** or **Apache 2.4+** - Web server
- **PM2** - Node.js process manager
- **Supervisor** - Laravel queue worker manager
- **Systemd** - Service management
- **Let's Encrypt** - SSL certificate automation

---

## 📚 Documentation

### Deployment Guides
- **[Quick Install - Debian 12](QUICK-INSTALL-DEBIAN12.md)** - ⚡ Fast setup for Debian 12 (15 minutes)
- **[Production Deployment](PRODUCTION-DEPLOYMENT.md)** - Complete guide for VPS/dedicated servers
- **[Apache2 Deployment](DEPLOYMENT-APACHE2.md)** - Quick setup for pre-configured Apache2 servers
- **[cPanel Deployment](DEPLOYMENT-CPANEL.md)** - Deploy to shared hosting with cPanel
- **[Deployment Checklist](DEPLOYMENT-CHECKLIST.md)** - Pre-deployment verification checklist

### Service Management
- **[Systemd Service Setup](SYSTEMD-SERVICE.md)** - WhatsApp Engine as systemd service with web management
- **Installation Scripts**:
  - `install-service.sh` - Install WhatsApp Engine as systemd service
  - `install-supervisor.sh` - Install Supervisor for queue workers

### Feature Documentation
- **[Website Features - English](website-features-en.md)** - Complete feature overview
- **[Website Features - Romanian](website-features-ro.md)** - Prezentare completă funcționalități

### Additional Resources
- **[Debian 12 Notes](DEBIAN12-NOTES.md)** - Debian 12 specific commands and troubleshooting
- **[PWA Setup](PWA_SETUP.md)** - Progressive Web App configuration

---

## ⚡ Quick Start

### Prerequisites

**Production Requirements:**
- PHP 8.4+ with extensions (mysql, redis, mbstring, xml, curl, zip, gd, bcmath, intl)
- Node.js 18.x+
- MySQL 8.0+ or MariaDB 10.5+
- Redis 6.0+
- Nginx 1.18+ or Apache 2.4+
- 4GB RAM minimum (8GB recommended)
- 20GB+ SSD storage

**Development Requirements:**
- PHP 8.4+
- Composer 2.x
- Node.js 18+ and npm
- MySQL/MariaDB database
- Redis (optional for dev, file cache fallback available)
- WhatsApp account for QR code authentication

### Installation Steps

#### 1. Clone Repository
```bash
git clone <repository-url> engageos
cd engageos
```

#### 2. Install Dependencies
```bash
# Backend dependencies
composer install

# Frontend dependencies
npm install
```

#### 3. Environment Configuration
```bash
# Copy environment file
cp .env.example .env

# Generate application key
php artisan key:generate
```

#### 4. Configure Database
Edit `.env` file:
```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=engageos
DB_USERNAME=your_username
DB_PASSWORD=your_password

# Redis Configuration
REDIS_HOST=127.0.0.1
REDIS_PASSWORD=null
REDIS_PORT=6379
```

#### 5. Run Database Migrations
```bash
php artisan migrate
```

#### 6. Build Frontend Assets
```bash
# Development
npm run dev

# Production
npm run build
```

#### 7. Configure WhatsApp Engine
```bash
cd whatsapp-engine

# Install dependencies
npm install

# Create environment file
cp .env.example .env

# Configure WhatsApp Engine
# Edit .env with your settings:
# WHATSAPP_ENGINE_PORT=3000
# APP_URL=http://localhost:8000
# NODE_ENV=development
```

#### 8. Start Services

**Development Mode:**
```bash
# Terminal 1: Laravel Application
php artisan serve

# Terminal 2: Queue Worker
php artisan queue:work

# Terminal 3: WhatsApp Engine
cd whatsapp-engine
npm start
```

**Production Mode:**
```bash
# Use PM2 for WhatsApp Engine
pm2 start whatsapp-engine/ecosystem.config.js --env production

# Use Supervisor for Queue Workers
# See: install-supervisor.sh

# Configure web server (Nginx/Apache)
# See deployment guides
```

#### 9. Access Application
- **Web Interface**: http://localhost:8000
- **WhatsApp Engine Status**: http://localhost:3000/status
- **Login**: Create first user via database or use seeders

#### 10. Connect WhatsApp
1. Visit WhatsApp Connection page in the application
2. Scan QR code with your WhatsApp mobile app
3. Wait for connection confirmation
4. Start sending messages!

---

## 🚀 Deployment Options

### Option 1: Full Production Deployment (Recommended)
**Best for:** VPS, Dedicated Servers, Cloud Instances (AWS, DigitalOcean, Linode, etc.)

Complete automated setup including all services, SSL, security hardening.

```bash
sudo ./deploy-production.sh
```

📖 **Guide:** [PRODUCTION-DEPLOYMENT.md](PRODUCTION-DEPLOYMENT.md)

**Features:**
- Automated Nginx/Apache configuration
- Let's Encrypt SSL certificate
- Systemd service for WhatsApp Engine
- Supervisor for queue workers
- Database setup and migration
- Redis configuration
- Security hardening

---

### Option 2: Quick Install - Debian 12
**Best for:** Fresh Debian 12 servers

Fast setup script that installs everything in ~15 minutes.

```bash
git clone <repository-url> engageos
cd engageos
chmod +x setup-debian12.sh
sudo ./setup-debian12.sh
```

📖 **Guide:** [QUICK-INSTALL-DEBIAN12.md](QUICK-INSTALL-DEBIAN12.md)

---

### Option 3: cPanel Shared Hosting
**Best for:** Shared hosting accounts with cPanel and SSH access

Step-by-step guide for deploying to cPanel environments.

📖 **Guide:** [DEPLOYMENT-CPANEL.md](DEPLOYMENT-CPANEL.md)

**Requirements:**
- cPanel with SSH access
- Node.js support (via Node.js Selector or custom)
- MySQL database
- SSL certificate

---

### Option 4: Pre-Configured Apache2 Server
**Best for:** Servers with Apache2, PHP-FPM, MariaDB, Redis already installed

Quick deployment when infrastructure is already in place.

```bash
# Clone and install
git clone <repository-url> engageos
cd engageos
composer install --no-dev --optimize-autoloader

# Configure .env and database
cp .env.example .env
php artisan key:generate
php artisan migrate

# Configure Apache VirtualHost
# See: DEPLOYMENT-APACHE2.md

# Start WhatsApp Engine
cd whatsapp-engine
npm install
pm2 start ecosystem.config.js --env production
```

📖 **Guide:** [DEPLOYMENT-APACHE2.md](DEPLOYMENT-APACHE2.md)

---

### Option 5: Docker (Coming Soon)
**Best for:** Containerized deployments

Docker Compose configuration for easy deployment.

```bash
# Coming soon
docker-compose up -d
```

---

## 📱 Usage Guide

### Creating Your First Campaign

1. **Navigate to Campaigns**
   - Click on "Campaigns" in the main menu
   - Click "New Campaign" button

2. **Configure Campaign**
   - Enter campaign name and description
   - Choose message type (Text or Template)
   - Write your message or select a template
   - Use variables like {{first_name}}, {{phone}}

3. **Add Recipients**
   - Manual entry: Paste phone numbers (one per line)
   - Select contact list: Choose from static or dynamic lists
   - Combine both: Manual + lists

4. **Schedule or Send**
   - Send immediately or schedule for later
   - Review recipient count
   - Click "Create Campaign"

5. **Monitor Progress**
   - View real-time statistics
   - Track sent, delivered, read status
   - Monitor replies and engagement

### Managing Contacts

**Add Contacts:**
- Manual entry: One at a time
- CSV import: Bulk upload with field mapping
- API integration: Programmatic addition

**Organize Contacts:**
- Create static lists for manual grouping
- Build dynamic lists with rule-based filters
- Tag contacts for easy categorization
- Track subscription status

**Import Contacts:**
1. Prepare CSV file with columns: first_name, last_name, phone, email
2. Go to Contacts → Import CSV
3. Upload file and map columns
4. Review and confirm import
5. Check import statistics

### Setting Up Auto-Replies

1. Navigate to Auto-Replies section
2. Create new auto-reply rule
3. Configure:
   - Keyword trigger (e.g., "INFO", "HELP")
   - Response message
   - Delay time (0-300 seconds)
   - Send once per contact option
4. Activate rule
5. Test by sending keyword to your WhatsApp

### Managing Opt-Outs (GDPR Compliance)

**Automatic Opt-Out:**
- System detects STOP, UNSUBSCRIBE, OPT-OUT keywords
- Automatically adds to opt-out list
- Excludes from future campaigns

**Manual Opt-Out:**
- Admin can opt-out contacts
- Bulk import opt-out lists via CSV
- Track opt-out reason and source

**Preference Center:**
- Contacts receive preference management link
- One-click unsubscribe
- One-click re-subscribe
- No login required

### API Integration

**Generate API Key:**
1. Go to Settings → API Keys
2. Click "Generate New Key"
3. Give it a name
4. Copy the key (shown only once!)
5. Use in API requests as Bearer token

**Example API Call:**
```bash
# Send WhatsApp message
curl -X POST https://your-domain.com/api/messages \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "phone_number": "+1234567890",
    "message": "Hello from EngageOS!"
  }'
```

**Available Endpoints:**
- Contact management (CRUD)
- List management (CRUD)
- Campaign operations (Create, Monitor)
- WhatsApp status check
- Subscription management

📖 **Full API Documentation:** See API docs in the application

---

## 🔧 Configuration

### Environment Variables

**Laravel Application (.env):**
```env
APP_NAME=EngageOS
APP_ENV=production
APP_URL=https://your-domain.com

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_DATABASE=engageos
DB_USERNAME=db_user
DB_PASSWORD=db_password

REDIS_HOST=127.0.0.1
REDIS_PORT=6379

QUEUE_CONNECTION=redis
CACHE_DRIVER=redis
SESSION_DRIVER=redis

WHATSAPP_ENGINE_API_URL=http://localhost:3000
```

**WhatsApp Engine (whatsapp-engine/.env):**
```env
WHATSAPP_ENGINE_PORT=3000
APP_URL=http://localhost:8000
WEBHOOK_URL=http://localhost:8000/webhook/whatsapp
NODE_ENV=production

# Database connection (for session storage)
DB_HOST=localhost
DB_USER=db_user
DB_PASSWORD=db_password
DB_NAME=engageos
```

### System Settings

Configure via web interface:
- **Company Information** - Name, email, phone, address, website
- **Branding** - Logo, favicon (auto-optimized)
- **Message Settings** - Header/footer templates
- **System Variables** - Reusable template variables
- **Provider Settings** - BulkSMS credentials, default provider

---

## 🛡️ Security

### Built-In Security Features

- ✅ **Authentication** - Laravel Sanctum with session management
- ✅ **Authorization** - Role-based access control (RBAC)
- ✅ **Password Hashing** - Bcrypt with cost factor 12
- ✅ **API Security** - Token-based authentication, rate limiting
- ✅ **Data Encryption** - Passwords, API keys, sensitive data
- ✅ **CSRF Protection** - All forms protected
- ✅ **XSS Prevention** - Output escaping throughout
- ✅ **SQL Injection Prevention** - Parameterized queries
- ✅ **Rate Limiting** - API and login attempt limits
- ✅ **Input Validation** - All user input sanitized
- ✅ **Secure Sessions** - HttpOnly, Secure, SameSite cookies

### Security Best Practices

**Production Deployment:**
```bash
# Set strong APP_KEY
php artisan key:generate

# Use HTTPS (SSL certificate)
# Configure web server for HTTPS only

# Set secure session settings in .env
SESSION_SECURE_COOKIE=true
SESSION_HTTP_ONLY=true
SESSION_SAME_SITE=strict

# Enable Redis password
REDIS_PASSWORD=strong_random_password

# Use strong database credentials
DB_PASSWORD=strong_random_password

# Restrict file permissions
chmod -R 755 storage bootstrap/cache
chown -R www-data:www-data storage bootstrap/cache
```

**Firewall Configuration:**
```bash
# Allow only necessary ports
ufw allow 22/tcp   # SSH
ufw allow 80/tcp   # HTTP
ufw allow 443/tcp  # HTTPS
ufw enable
```

---

## 🧪 Testing

### Run Laravel Tests
```bash
# Run all tests
php artisan test

# Run specific test suite
php artisan test --testsuite=Feature

# Run with coverage
php artisan test --coverage
```

### Manual Testing Checklist

- [ ] Create test campaign
- [ ] Add test contacts
- [ ] Connect WhatsApp via QR code
- [ ] Send test messages
- [ ] Verify delivery status updates
- [ ] Reply from phone and check reply tracking
- [ ] Test auto-reply functionality
- [ ] Test opt-out detection
- [ ] Check real-time statistics updates
- [ ] Test CSV import/export
- [ ] Verify API endpoints
- [ ] Test multi-user isolation

---

## 🔄 Maintenance

### Regular Maintenance Tasks

**Daily:**
```bash
# Check queue workers
php artisan queue:work --status

# Check WhatsApp Engine status
pm2 status

# Monitor logs
tail -f storage/logs/laravel.log
```

**Weekly:**
```bash
# Clear old logs
php artisan log:clear

# Optimize application
php artisan optimize:clear
php artisan optimize
```

**Monthly:**
```bash
# Database backup
mysqldump -u user -p engageos > backup_$(date +%Y%m%d).sql

# Update dependencies (carefully)
composer update
npm update
```

### Troubleshooting

**WhatsApp Disconnects:**
1. Check PM2 status: `pm2 status`
2. Check logs: `pm2 logs whatsapp-engine`
3. Restart engine: `pm2 restart whatsapp-engine`
4. Re-scan QR code if needed

**Queue Not Processing:**
1. Check queue worker: `systemctl status laravel-worker`
2. Restart worker: `systemctl restart laravel-worker`
3. Check Redis: `redis-cli ping`
4. Check logs: `tail -f storage/logs/laravel.log`

**Performance Issues:**
1. Enable caching: `php artisan config:cache && php artisan route:cache`
2. Check database indexes
3. Monitor Redis memory: `redis-cli info memory`
4. Check server resources: `htop`

---

## 📊 Performance Optimization

### Laravel Optimization
```bash
# Cache configuration
php artisan config:cache

# Cache routes
php artisan route:cache

# Cache views
php artisan view:cache

# Optimize autoloader
composer install --optimize-autoloader --no-dev
```

### Database Optimization
```sql
-- Add indexes for frequently queried columns
CREATE INDEX idx_campaigns_user_id ON campaigns(user_id);
CREATE INDEX idx_contacts_user_id ON contacts(user_id);
CREATE INDEX idx_messages_campaign_id ON messages(campaign_id);
```

### Redis Optimization
```bash
# Configure Redis max memory
redis-cli CONFIG SET maxmemory 2gb
redis-cli CONFIG SET maxmemory-policy allkeys-lru
```

### Web Server Optimization

**Nginx:**
```nginx
# Enable gzip compression
gzip on;
gzip_vary on;
gzip_min_length 1024;
gzip_types text/plain text/css text/xml text/javascript application/json;

# Browser caching
location ~* \.(jpg|jpeg|png|gif|ico|css|js|svg|woff|woff2)$ {
    expires 365d;
    add_header Cache-Control "public, immutable";
}
```

---

## 🔄 Backup & Recovery

### Automated Backup Script

Create `backup.sh`:
```bash
#!/bin/bash
BACKUP_DIR="/var/backups/engageos"
DATE=$(date +%Y%m%d_%H%M%S)

# Database backup
mysqldump -u user -p'password' engageos > $BACKUP_DIR/db_$DATE.sql

# Files backup
tar -czf $BACKUP_DIR/files_$DATE.tar.gz \
    /var/www/engageos/storage \
    /var/www/engageos/.env \
    /var/www/engageos/public/uploads

# Keep only last 30 days
find $BACKUP_DIR -name "*.sql" -mtime +30 -delete
find $BACKUP_DIR -name "*.tar.gz" -mtime +30 -delete
```

Add to crontab:
```bash
# Daily backup at 2 AM
0 2 * * * /path/to/backup.sh
```

### Restore from Backup
```bash
# Restore database
mysql -u user -p'password' engageos < backup.sql

# Restore files
tar -xzf backup.tar.gz -C /var/www/engageos

# Set permissions
chown -R www-data:www-data /var/www/engageos/storage
```

---

## 📁 Project Structure

```
engageos/
├── app/
│   ├── Http/
│   │   ├── Controllers/        # API & Web controllers
│   │   ├── Middleware/         # Authentication, CORS, etc.
│   │   └── Requests/           # Form request validation
│   ├── Livewire/              # Frontend Livewire components
│   ├── Models/                # Eloquent models
│   ├── Services/              # Business logic layer
│   │   ├── CampaignService.php
│   │   ├── ContactService.php
│   │   ├── WhatsAppService.php
│   │   └── MessageBuilderService.php
│   └── Traits/                # Reusable traits
├── bootstrap/
├── config/                    # Application configuration
├── database/
│   ├── migrations/           # Database schema
│   ├── seeders/             # Database seeders
│   └── factories/           # Model factories
├── public/                   # Web root
│   ├── index.php
│   ├── manifest.json        # PWA manifest
│   └── pwa/                 # PWA assets
├── resources/
│   ├── css/                 # TailwindCSS styles
│   ├── js/                  # Alpine.js, JavaScript
│   └── views/               # Blade templates
│       ├── layouts/
│       ├── livewire/
│       └── auth/
├── routes/
│   ├── web.php             # Web routes
│   ├── api.php             # API routes
│   └── console.php         # Artisan commands
├── storage/
│   ├── app/                # Application files
│   ├── framework/          # Framework cache
│   └── logs/               # Application logs
├── tests/
│   ├── Feature/            # Feature tests
│   └── Unit/               # Unit tests
├── whatsapp-engine/        # Node.js WhatsApp integration
│   ├── index.js            # Main server file
│   ├── routes/             # Express routes
│   ├── services/           # Business logic
│   ├── utils/              # Utilities
│   ├── package.json
│   └── ecosystem.config.js # PM2 configuration
├── .env.example            # Environment template
├── composer.json           # PHP dependencies
├── package.json            # Node dependencies
├── artisan                 # Laravel CLI
└── README.md              # This file
```

---

## 🤝 Support & Community

### Getting Help

- 📧 **Email Support**: support@engageos.com (if applicable)
- 📚 **Documentation**: See `/docs` folder and this README
- 🐛 **Bug Reports**: Use GitHub Issues
- 💬 **Community**: Join our Discord/Slack (if applicable)

### Reporting Issues

When reporting bugs, please include:
1. EngageOS version
2. PHP version
3. Node.js version
4. Operating system
5. Steps to reproduce
6. Error messages and logs
7. Expected vs actual behavior

---

## 📄 License

This project is proprietary software. All rights reserved.

**License Options Available:**
- Single Site License
- Multi-Site License
- Developer License
- White Label Rights

Contact for licensing information.

---

## 🙏 Acknowledgments

EngageOS is built with amazing open-source technologies:

- **[Laravel](https://laravel.com/)** - The PHP framework for web artisans
- **[Baileys](https://github.com/WhiskeySockets/Baileys)** - WhatsApp Web API library
- **[TailwindCSS](https://tailwindcss.com/)** - Utility-first CSS framework
- **[Livewire](https://laravel-livewire.com/)** - Full-stack framework for Laravel
- **[Alpine.js](https://alpinejs.dev/)** - Lightweight JavaScript framework
- **[Redis](https://redis.io/)** - In-memory data structure store
- **[BullMQ](https://docs.bullmq.io/)** - Premium message queue for Node.js
- **[PM2](https://pm2.keymetrics.io/)** - Node.js process manager

Special thanks to the open-source community for making projects like EngageOS possible.

---

## 🚀 What's Next?

### Roadmap (Upcoming Features)

- [ ] **SMS Gateway Integration** - Additional providers (Twilio, Vonage)
- [ ] **Email Campaigns** - Multi-channel support
- [ ] **AI-Powered Analytics** - Predictive insights and recommendations
- [ ] **Advanced Reporting** - Custom reports and dashboards
- [ ] **CRM Integration** - Salesforce, HubSpot connectors
- [ ] **Zapier Integration** - Connect to 5000+ apps
- [ ] **Mobile Apps** - iOS and Android native apps
- [ ] **Voice Campaigns** - WhatsApp voice messages
- [ ] **Video Messages** - Send video campaigns
- [ ] **Chatbot Builder** - Visual flow builder for automated conversations
- [ ] **A/B Testing** - Test message variations
- [ ] **Geolocation** - Location-based campaigns
- [ ] **Multi-Language UI** - Interface translations

---

<div align="center">

**EngageOS** - Enterprise WhatsApp Messaging Platform

Built with ❤️ using Laravel & Node.js by [Cristian Casapu](https://CristianCasapu.ro)

[Get Started](#-quick-start) • [Documentation](#-documentation) • [Support](#-support--community)

---

*Last Updated: November 2025 • Version 1.0.0*

</div>
