# EngageOS - Enterprise WhatsApp SaaS Platform

<div align="center">

![Version](https://img.shields.io/badge/version-2.0.0-blue.svg)
![PHP](https://img.shields.io/badge/PHP-8.4+-purple.svg)
![Laravel](https://img.shields.io/badge/Laravel-10.x-red.svg)
![OpenWA](https://img.shields.io/badge/OpenWA-Gateway-green.svg)
![License](https://img.shields.io/badge/license-Proprietary-orange.svg)

**The Most Comprehensive WhatsApp Messaging Platform for Enterprise**

*Campaign Management • Multi-Tenancy • Real-Time Analytics • GDPR Compliant*

[Features](#-key-features) • [Documentation](#-documentation) • [Quick Start](#-quick-start) • [Deployment](#-deployment-options) • [Tech Stack](#-tech-stack)

</div>

---

## 📖 About EngageOS

**EngageOS** is a production-ready, enterprise-grade WhatsApp SaaS platform that enables businesses, marketing agencies, and service providers to manage sophisticated WhatsApp messaging campaigns at scale. Built on Laravel and powered by the self-hosted **[OpenWA](https://github.com/CristianCasapu/OpenWA)** WhatsApp gateway, EngageOS offers complete multi-tenancy, advanced campaign automation, real-time analytics, and comprehensive API integration.

### Why EngageOS?

- ✅ **100+ Features** across 14 major modules
- ✅ **Production-Ready** - Battle-tested in real businesses
- ✅ **Multi-Tenant** - Complete data isolation for multiple users/clients
- ✅ **Enterprise-Grade Security** - GDPR compliant with role-based access control
- ✅ **Modern Tech Stack** - Laravel 10, OpenWA gateway, Redis, TailwindCSS
- ✅ **Comprehensive API** - RESTful API for seamless integrations
- ✅ **Real-Time Updates** - WebSocket support (Laravel Reverb) for live campaign monitoring
- ✅ **Anti-Ban Protection** - Paced, human-like sending prevents WhatsApp blocking

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
- **WhatsApp Delivery** - All messaging flows through the self-hosted OpenWA gateway
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
- **Queue System** - Redis-backed Laravel queues for background processing
- **Anti-Ban Protection** - ~3s spacing with random jitter between messages, plus OpenWA's own anti-ban pacing

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

### 📱 WhatsApp Gateway (OpenWA)
- **Self-Hosted Gateway** - [OpenWA](https://github.com/CristianCasapu/OpenWA), a NestJS WhatsApp API gateway run as a Docker service
- **Engine Choice** - whatsapp-web.js by default, Baileys optional (configured in OpenWA via `ENGINE_TYPE`)
- **QR Code Authentication** - Pair by scanning a QR code straight from the EngageOS UI
- **Server-Side REST Integration** - Laravel talks to the gateway with an `X-API-Key`; nothing is exposed to the browser
- **Signed Webhooks** - Message sent/received/ack/failed and session status/QR events, verified with HMAC-SHA256
- **Delivery & Read Receipts** - Ack events update campaign statistics in real time
- **Built-In Dashboard** - OpenWA ships its own React dashboard for sessions, keys, and logs

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
- **Service Status Dashboard** - Monitor system health (Super Admin)
- **Image Optimization** - Auto WebP/PNG conversion
- **Custom Variables** - Define reusable template variables

### 🛠️ Developer Features
- **Comprehensive Logging** - Laravel logs plus OpenWA container logs
- **Code Quality Tools** - Laravel Pint, PHPUnit
- **One-Command Updates** - `update.sh` handles the full 8-step update
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
- **Laravel Echo + Reverb** - Real-time WebSocket updates

### WhatsApp Gateway (OpenWA)
- **[OpenWA](https://github.com/CristianCasapu/OpenWA)** - Self-hosted NestJS WhatsApp API gateway
- **Docker Compose** - Runs as a container via `docker-compose.openwa.yml`, bound to `127.0.0.1:2785`
- **whatsapp-web.js / Baileys** - Selectable engine (`ENGINE_TYPE`, OpenWA-side setting)
- **REST API + Webhooks** - `X-API-Key` auth outbound, HMAC-SHA256 signed events inbound
- **React Dashboard** - Session, API key, and log management on the same port

### Infrastructure
- **Nginx** or **Apache 2.4+** - Web server
- **Docker + Docker Compose** - OpenWA gateway runtime
- **Supervisor** - Laravel queue worker manager
- **Systemd** - Service management (Reverb, workers)
- **Let's Encrypt** - SSL certificate automation

---

## 📚 Documentation

### Deployment & Operations
- **`docker-compose.openwa.yml`** - OpenWA gateway service; the file header documents setup, logs, and update commands
- **`update.sh`** - 8-step production update script (pull, dependencies, assets, caches, migrations, Apache reload, service restarts)
- **[Continuous Campaigns Deployment](deployment/CONTINUOUS_CAMPAIGNS_DEPLOYMENT.md)** - Running the continuous campaigns daemon

### Helper Scripts
- `scripts/create-admin.php` - Create the first admin user
- `scripts/reset-admin-password.php` - Reset an admin password

> OpenWA has its own documentation in the [OpenWA repository](https://github.com/CristianCasapu/OpenWA), covering the dashboard, API keys, engines, and anti-ban settings.

---

## ⚡ Quick Start

### Prerequisites

**Production Requirements:**
- PHP 8.4+ with extensions (mysql, redis, mbstring, xml, curl, zip, gd, bcmath, intl)
- Node.js 18.x+ (frontend asset builds)
- Docker + Docker Compose (OpenWA gateway)
- MySQL 8.0+ or MariaDB 10.5+
- Redis 6.0+
- Nginx 1.18+ or Apache 2.4+
- 4GB RAM minimum (8GB recommended)
- 20GB+ SSD storage

**Development Requirements:**
- PHP 8.4+
- Composer 2.x
- Node.js 18+ and npm
- Docker + Docker Compose
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

#### 7. Set Up the OpenWA Gateway
```bash
# Clone OpenWA next to this repo (the compose file builds from ../OpenWA)
git clone https://github.com/CristianCasapu/OpenWA ../OpenWA

# Build and start the gateway (bound to 127.0.0.1:2785)
docker compose -f docker-compose.openwa.yml up -d --build

# Read the bootstrap admin API key written on first boot
docker compose -f docker-compose.openwa.yml exec openwa cat /app/data/.api-key
```

Add the OpenWA settings to the Laravel `.env`:
```env
OPENWA_BASE_URL=http://127.0.0.1:2785
OPENWA_API_KEY=<key from the command above>
OPENWA_SESSION_NAME=engageos
OPENWA_WEBHOOK_SECRET=<random shared secret>
```

Then provision the session and register the webhook (idempotent, safe to re-run):
```bash
php artisan openwa:setup
```

#### 8. Start Services

**Development Mode:**
```bash
# Terminal 1: Laravel Application
php artisan serve

# Terminal 2: Queue Worker
php artisan queue:work

# Terminal 3: Reverb (real-time updates)
php artisan reverb:start
```
The OpenWA gateway is already running in Docker from step 7.

**Production Mode:**
```bash
# Supervisor for Queue Workers, systemd for Reverb
# Configure web server (Nginx/Apache)

# OpenWA runs under Docker with restart: unless-stopped
docker compose -f docker-compose.openwa.yml up -d
```

#### 9. Access Application
- **Web Interface**: http://localhost:8000
- **OpenWA Dashboard**: http://127.0.0.1:2785 (local access only)
- **Login**: Create first user via `scripts/create-admin.php` or seeders

#### 10. Connect WhatsApp
1. Visit the WhatsApp Connection page in the application
2. The page polls Laravel, which fetches the current QR code from OpenWA
3. Scan the QR code with your WhatsApp mobile app
4. Wait for connection confirmation and start sending messages!

---

## 🚀 Deployment Options

### Option 1: Production VPS / Dedicated Server (Recommended)
**Best for:** VPS, Dedicated Servers, Cloud Instances (AWS, DigitalOcean, Linode, etc.)

```bash
# Clone and install
git clone <repository-url> engageos
cd engageos
composer install --no-dev --optimize-autoloader
npm install && npm run build

# Configure .env and database
cp .env.example .env
php artisan key:generate
php artisan migrate

# Configure Apache/Nginx VirtualHost for the Laravel app
# Supervisor for queue workers, systemd for Reverb

# Start the OpenWA gateway
git clone https://github.com/CristianCasapu/OpenWA ../OpenWA
docker compose -f docker-compose.openwa.yml up -d --build
docker compose -f docker-compose.openwa.yml exec openwa cat /app/data/.api-key
# Set OPENWA_* in .env, then:
php artisan openwa:setup
```

**Notes:**
- OpenWA is bound to `127.0.0.1:2785` — it is never exposed publicly, and no web server proxy rules are needed for it
- Laravel and OpenWA communicate server-side only (REST + signed webhooks)

---

### Option 2: Updating an Existing Installation

```bash
sudo ./update.sh
```

The script runs 8 steps: git pull, Composer dependencies, npm dependencies, asset build, Laravel optimizations, migrations, Apache reload, and service restarts.

OpenWA is updated independently of the app:
```bash
git -C ../OpenWA pull
docker compose -f docker-compose.openwa.yml up -d --build
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
   - Track sent, delivered, read status (via OpenWA ack webhooks)
   - Monitor replies and engagement

Messages are sent one at a time through the OpenWA gateway with roughly 3 seconds plus random jitter between sends (`OPENWA_SEND_DELAY_MS`), keeping the pace human-like.

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

Inbound messages arrive through the OpenWA webhook (`message.received`), so auto-replies and keyword detection work without any extra setup.

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

# OpenWA gateway (see config/openwa.php)
OPENWA_BASE_URL=http://127.0.0.1:2785
OPENWA_API_KEY=your-openwa-api-key
OPENWA_SESSION_NAME=engageos
OPENWA_WEBHOOK_SECRET=your-shared-webhook-secret
OPENWA_TIMEOUT=30
OPENWA_SEND_DELAY_MS=3000
```

**How the integration works:**
- Laravel calls OpenWA server-side via `app/Services/OpenWA/OpenWAClient.php`, authenticating with `X-API-Key`
- OpenWA posts events to `POST /webhook/openwa`, signed with HMAC-SHA256 (`X-OpenWA-Signature`, verified against `OPENWA_WEBHOOK_SECRET`)
- Handled events: `message.received`, `message.sent`, `message.ack` (delivered/read/failed), `message.failed`, `session.status`, `session.qr`
- `php artisan openwa:setup` provisions the session and registers the webhook — idempotent, safe to re-run after config changes
- Gateway-side options (engine choice via `ENGINE_TYPE`, anti-ban pacing, storage) are configured in OpenWA itself, not in EngageOS

### System Settings

Configure via web interface:
- **Company Information** - Name, email, phone, address, website
- **Branding** - Logo, favicon (auto-optimized)
- **Message Settings** - Header/footer templates
- **System Variables** - Reusable template variables

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
- ✅ **Signed Webhooks** - OpenWA events verified with HMAC-SHA256
- ✅ **Localhost-Only Gateway** - OpenWA bound to 127.0.0.1, never internet-facing

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

# Set a strong OpenWA webhook secret
OPENWA_WEBHOOK_SECRET=strong_random_secret

# Restrict file permissions
chmod -R 755 storage bootstrap/cache
chown -R www-data:www-data storage bootstrap/cache
```

**Firewall Configuration:**
```bash
# Allow only necessary ports (OpenWA's 2785 stays localhost-only)
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
- [ ] Verify delivery status updates (ack webhooks)
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

# Check OpenWA gateway status
docker compose -f docker-compose.openwa.yml ps

# Monitor logs
tail -f storage/logs/laravel.log
docker compose -f docker-compose.openwa.yml logs -f
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

# Update OpenWA
git -C ../OpenWA pull
docker compose -f docker-compose.openwa.yml up -d --build
```

### Troubleshooting

**WhatsApp Disconnects:**
1. Check the container: `docker compose -f docker-compose.openwa.yml ps`
2. Check logs: `docker compose -f docker-compose.openwa.yml logs -f openwa`
3. Inspect the session in the OpenWA dashboard: http://127.0.0.1:2785
4. Restart the gateway: `docker compose -f docker-compose.openwa.yml restart`
5. Re-scan the QR code from the WhatsApp Connection page if needed

**Webhooks Not Arriving (no receipts / no inbound replies):**
1. Verify `OPENWA_WEBHOOK_SECRET` matches the registered webhook
2. Re-run `php artisan openwa:setup` (idempotent) to re-register the webhook
3. Make sure `APP_URL` is reachable from inside the OpenWA container
4. Check Laravel logs for signature verification failures

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

> The OpenWA session lives in the `openwa-data` Docker volume — include it in backups if you want to avoid re-pairing after a full restore.

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
│   │   ├── Controllers/        # API & Web controllers (incl. OpenWA webhook)
│   │   ├── Middleware/         # Authentication, CORS, etc.
│   │   └── Requests/           # Form request validation
│   ├── Livewire/              # Frontend Livewire components
│   ├── Models/                # Eloquent models
│   ├── Services/              # Business logic layer
│   │   ├── CampaignService.php
│   │   ├── ContactService.php
│   │   ├── WhatsAppService.php
│   │   ├── MessageBuilderService.php
│   │   └── OpenWA/
│   │       └── OpenWAClient.php  # REST client for the OpenWA gateway
│   └── Traits/                # Reusable traits
├── bootstrap/
├── config/                    # Application configuration
│   └── openwa.php            # OpenWA gateway settings
├── database/
│   ├── migrations/           # Database schema
│   ├── seeders/             # Database seeders
│   └── factories/           # Model factories
├── deployment/               # Continuous campaigns daemon setup
├── public/                   # Web root
│   ├── index.php
│   ├── manifest.json        # PWA manifest
│   └── pwa/                 # PWA assets
├── resources/
│   ├── css/                 # TailwindCSS styles
│   ├── js/                  # Alpine.js, Echo/Reverb
│   └── views/               # Blade templates
│       ├── layouts/
│       ├── livewire/
│       └── auth/
├── routes/
│   ├── web.php             # Web routes (incl. /webhook/openwa)
│   ├── api.php             # API routes
│   └── console.php         # Artisan commands
├── scripts/                 # Admin helper scripts
├── storage/
│   ├── app/                # Application files
│   ├── framework/          # Framework cache
│   └── logs/               # Application logs
├── tests/
│   ├── Feature/            # Feature tests
│   └── Unit/               # Unit tests
├── docker-compose.openwa.yml  # OpenWA gateway service (built from ../OpenWA)
├── update.sh               # 8-step production update script
├── .env.example            # Environment template
├── composer.json           # PHP dependencies
├── package.json            # Node dependencies (frontend build)
├── artisan                 # Laravel CLI
└── README.md              # This file
```

The OpenWA gateway itself lives in a sibling checkout (`../OpenWA`) and is built into a Docker image by `docker-compose.openwa.yml`.

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
3. OpenWA version / engine (`ENGINE_TYPE`)
4. Operating system
5. Steps to reproduce
6. Error messages and logs (Laravel + OpenWA container)
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
- **[OpenWA](https://github.com/CristianCasapu/OpenWA)** - Self-hosted WhatsApp API gateway powering all messaging
- **[TailwindCSS](https://tailwindcss.com/)** - Utility-first CSS framework
- **[Livewire](https://laravel-livewire.com/)** - Full-stack framework for Laravel
- **[Alpine.js](https://alpinejs.dev/)** - Lightweight JavaScript framework
- **[Redis](https://redis.io/)** - In-memory data structure store

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

Built with ❤️ using Laravel & OpenWA by [Cristian Casapu](https://CristianCasapu.ro)

[Get Started](#-quick-start) • [Documentation](#-documentation) • [Support](#-support--community)

---

*Last Updated: August 2026 • Version 2.0.0*

</div>
