# 🚀 ZapFlow - WhatsApp Business API Platform

<div align="center">

![ZapFlow Logo](https://img.shields.io/badge/⚡-ZapFlow-success?style=for-the-badge&logo=whatsapp&logoColor=white)

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg?style=flat-square&logo=python&logoColor=white)](https://python.org)
[![Node.js](https://img.shields.io/badge/Node.js-16+-green.svg?style=flat-square&logo=node.js&logoColor=white)](https://nodejs.org)
[![Flask](https://img.shields.io/badge/Flask-2.0+-red.svg?style=flat-square&logo=flask&logoColor=white)](https://flask.palletsprojects.com)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Business-25D366?style=flat-square&logo=whatsapp&logoColor=white)](https://business.whatsapp.com)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)

**A powerful, enterprise-grade WhatsApp messaging platform built for businesses**

[🌟 Features](#-features) • [🚀 Quick Start](#-quick-start) • [📚 Documentation](#-documentation) • [🔧 API Reference](#-api-reference) • [🤝 Support](#-support)

---

**Portfolio Project by**

[![THE-GRIT-AGENCIES](https://img.shields.io/badge/THE--GRIT--AGENCIES-Nairobi,%20Kenya-orange?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZD0iTTEyIDJMMTMuMDkgOC4yNkwyMCA5TDEzLjA5IDE1Ljc0TDEyIDIyTDEwLjkxIDE1Ljc0TDQgOUwxMC45MSA4LjI2TDEyIDJaIiBmaWxsPSJ3aGl0ZSIvPgo8L3N2Zz4K)](https://github.com/THE-GRIT-AGENCIES)

*Portfolio showcase demonstrating enterprise-level full-stack development and system architecture*

</div>

---

## 🌟 Features

<div align="center">

| 🔐 **Secure Authentication** | 📱 **WhatsApp Integration** | 🚀 **RESTful API** |
|:---:|:---:|:---:|
| User registration & login | QR code connection | Full API access |
| API key generation | Real-time messaging | Rate limiting |
| Session management | Message history | JSON responses |

| 📊 **Analytics Dashboard** | 📤 **Bulk Messaging** | 📝 **Message Templates** |
|:---:|:---:|:---:|
| Message statistics | CSV import support | Dynamic variables |
| Send/receive history | Broadcast campaigns | Reusable templates |
| User analytics | Contact management | Template editor |

</div>

### ✨ What Makes ZapFlow Special

- ⚡ **Enterprise-Ready**: Built for scale with proper authentication and security
- 🎯 **Developer-Friendly**: Clean RESTful API with comprehensive documentation
- 💼 **Business-Focused**: Template system, bulk messaging, and analytics
- 🌍 **Global Reach**: WhatsApp integration for worldwide communication
- 🛡️ **Secure**: API key authentication and encrypted sessions
- 📊 **Analytics**: Detailed message tracking and delivery reports

---

## 🎯 Project Overview

ZapFlow is a comprehensive WhatsApp Business API platform that I developed to demonstrate full-stack development capabilities. This project showcases enterprise-level architecture, security implementation, and real-world business application development.

### 🏗️ Technical Architecture

**Backend Stack:**
- **Python/Flask** - RESTful API development
- **SQLite/SQLAlchemy** - Database design and ORM implementation
- **Node.js** - WhatsApp Web.js integration bridge
- **Session Management** - Secure authentication system

**Frontend Stack:**
- **HTML5/CSS3** - Modern responsive design
- **JavaScript** - Dynamic user interactions
- **Bootstrap** - Professional UI components
- **Real-time Updates** - WebSocket integration

**Key Integrations:**
- **WhatsApp Web.js** - Real-time messaging capabilities
- **CSV Processing** - Bulk contact management
- **API Security** - Token-based authentication
- **Analytics Dashboard** - Message tracking and reporting

---

## 📚 Documentation

### 🎨 User Interface

![Dashboard Preview](https://img.shields.io/badge/Dashboard-Modern_UI-blue?style=for-the-badge&logo=bootstrap)

The ZapFlow dashboard provides:

- **🏠 Home Dashboard**: Overview of your messaging activity
- **📱 WhatsApp Connection**: Easy QR code scanning interface
- **📤 Send Messages**: Individual and bulk messaging
- **📝 Templates**: Create and manage message templates
- **📊 Analytics**: Track message delivery and engagement
- **🔑 API Keys**: Generate and manage API access

### 🔧 Core Components

#### 1. **User Management**
- Secure registration and authentication
- Phone number verification
- Session management
- API key generation

#### 2. **WhatsApp Integration**
- QR code connection process
- Real-time status monitoring
- Message queue management
- Delivery confirmation

#### 3. **Message System**
- Individual message sending
- Bulk messaging (up to 15 recipients)
- CSV contact import
- Message templates with variables
- Message history and analytics

---

## 🔧 API Architecture

ZapFlow implements a comprehensive RESTful API architecture designed for enterprise-scale messaging operations. The API demonstrates advanced backend development principles including authentication, rate limiting, and structured error handling.

### 🔐 Authentication System

The platform implements a dual-authentication approach:
- **Session-based authentication** for web interface users
- **API key authentication** for programmatic access
- **Rate limiting** to prevent abuse and ensure fair usage

### 📤 API Endpoints Design

**Message Operations:**
- `POST /api/send-message` - Individual message dispatch
- `POST /api/broadcast` - Bulk messaging capabilities
- `GET /api/messages` - Message history and analytics
- `GET /api/templates` - Template management

**User Management:**
- `POST /api/register` - User registration
- `POST /api/login` - Authentication
- `GET /api/profile` - User profile management
- `POST /api/generate-key` - API key generation

**WhatsApp Integration:**
- `GET /api/status` - Connection status monitoring
- `POST /api/connect` - QR code generation
- `GET /api/health` - Service health checks

### 📊 Response Architecture

All API responses follow a consistent structure with proper HTTP status codes, error handling, and detailed response metadata for optimal developer experience.

---

## 🗄️ Database Schema

### 👥 Users Table
| Column | Type | Description |
|--------|------|-------------|
| `id` | Integer | Primary key |
| `name` | String(100) | User's full name |
| `phone` | String(20) | Phone number (unique) |
| `password_hash` | String(128) | Hashed password |
| `api_key` | String(32) | Generated API key |
| `whatsapp_connected` | Boolean | Connection status |
| `created_at` | DateTime | Registration timestamp |

### 💬 Messages Table
| Column | Type | Description |
|--------|------|-------------|
| `id` | Integer | Primary key |
| `user_id` | Integer | Foreign key to users |
| `recipient_phone` | String(20) | Recipient phone number |
| `message_text` | Text | Message content |
| `sent_at` | DateTime | Timestamp |
| `status` | String(20) | Message status |
| `broadcast_id` | String(32) | Broadcast group ID |

### 📝 Templates Table
| Column | Type | Description |
|--------|------|-------------|
| `id` | Integer | Primary key |
| `user_id` | Integer | Foreign key to users |
| `name` | String(100) | Template name |
| `template_text` | Text | Template content |
| `variables` | Text | Template variables |
| `created_at` | DateTime | Creation timestamp |

---

## 🚀 Implementation Highlights

### 🌐 Production-Ready Features

**Environment Management:**
- Configuration management for different deployment stages
- Environment variable handling for sensitive data
- Scalable architecture supporting multiple deployment strategies

**Performance Optimization:**
- Efficient database queries with SQLAlchemy ORM
- Asynchronous message processing
- Connection pooling for database operations
- Caching strategies for frequently accessed data

**Monitoring & Logging:**
- Comprehensive error tracking and logging
- Performance metrics collection
- Health check endpoints for monitoring
- Detailed audit trails for message operations

---

## 🛡️ Security Features

### 🔒 Authentication & Authorization
- Secure password hashing with Werkzeug
- API key-based authentication
- Session management
- Input validation and sanitization

### 🛡️ Security Best Practices
- Rate limiting for API endpoints
- CSRF protection
- SQL injection prevention
- XSS protection
- Secure file uploads

### 🔐 Production Security Checklist
- [ ] Change default secret keys
- [ ] Use HTTPS in production
- [ ] Implement rate limiting
- [ ] Regular security audits
- [ ] Keep dependencies updated
- [ ] Monitor for suspicious activity

---

## 🔍 Development Challenges & Solutions

### 🎯 Technical Challenges Addressed

| Challenge | Solution Implemented |
|-----------|---------------------|
| **Real-time WhatsApp Integration** | Node.js bridge with WebSocket communication for live status updates |
| **Bulk Message Processing** | Asynchronous queue system with progress tracking and error handling |
| **API Rate Limiting** | Custom middleware implementing token bucket algorithm |
| **Database Scalability** | Optimized queries with proper indexing and connection pooling |
| **Security Implementation** | Multi-layer security with authentication, authorization, and input validation |
| **Cross-Platform Compatibility** | Responsive design with progressive enhancement |

### 💡 Innovation Features

- **Dynamic Template System**: Variable replacement engine for personalized messaging
- **CSV Import Processing**: Robust file handling with error detection and validation
- **Real-time Analytics**: Live dashboard updates using WebSocket connections
- **QR Code Integration**: Seamless WhatsApp Web authentication flow
- **Message Queue Management**: Intelligent retry mechanisms and failure handling

---

## 🎯 Portfolio Showcase

### 🛠️ Technologies Demonstrated

- **Backend**: Python, Flask, SQLite
- **Frontend**: HTML5, CSS3, JavaScript, Bootstrap
- **API Integration**: WhatsApp Web.js
- **Runtime**: Node.js for WhatsApp bridge
- **Database**: SQLite with SQLAlchemy ORM
- **Authentication**: Session-based + API key authentication
- **Security**: Password hashing, CSRF protection, input validation

### 🏗️ Architecture Highlights

- **Full-Stack Development**: Complete web application with frontend and backend
- **RESTful API Design**: Clean API endpoints with proper HTTP methods
- **Real-time Communication**: WebSocket integration for live status updates
- **Database Design**: Normalized database schema with relationships
- **Security Implementation**: Production-ready security measures
- **Scalable Architecture**: Modular design for easy maintenance and scaling

### 📈 Key Features Implemented

- User authentication and authorization system
- Real-time WhatsApp integration via QR code
- Bulk messaging capabilities with CSV import
- Message template system with dynamic variables
- Analytics dashboard with message tracking
- API key management system
- Responsive web design for all devices

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2024 THE-GRIT-AGENCIES

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software...
```

---

## 🤝 Support & Contact

<div align="center">

### 💬 Get in Touch

[![Email](https://img.shields.io/badge/Email-Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:support@grit-agencies.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-View_More-4285F4?style=for-the-badge&logo=google-chrome&logoColor=white)](https://portfolio.grit-agencies.com)

### 🌍 Connect with THE-GRIT-AGENCIES

[![Website](https://img.shields.io/badge/Website-Visit_Us-FF6B6B?style=for-the-badge&logo=google-chrome&logoColor=white)](https://grit-agencies.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/company/the-grit-agencies)
[![Twitter](https://img.shields.io/badge/Twitter-Follow-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/grit_agencies)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/THE-GRIT-AGENCIES)

**📍 Location:** Nairobi, Kenya 🇰🇪

---

### 🙏 Acknowledgments

- 🙌 **WhatsApp Web.js** - For the amazing WhatsApp integration
- 🔥 **Flask Community** - For the robust web framework
- 💚 **Node.js Community** - For the excellent runtime environment
- 🎨 **Bootstrap** - For the beautiful UI components
- 🌍 **Open Source Community** - For inspiration and collaboration

---

**Made with ❤️ by THE-GRIT-AGENCIES in Nairobi, Kenya**

*Portfolio project showcasing full-stack development expertise*

</div>

---



<div align="center">

**⭐ This is a portfolio demonstration project showcasing development capabilities**

[![GitHub stars](https://img.shields.io/github/stars/THE-GRIT-AGENCIES/zapflow?style=social)](https://github.com/THE-GRIT-AGENCIES/zapflow/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/THE-GRIT-AGENCIES/zapflow?style=social)](https://github.com/THE-GRIT-AGENCIES/zapflow/network/members)

*Interested in similar projects? Let's connect and discuss your requirements!*

</div>
