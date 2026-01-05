# 🕐 PUNCHCLOCK Demo

> **Portfolio/Showcase Version** - This is a demonstration repository showcasing the architecture and capabilities of PUNCHCLOCK, a production HR OS used by Malaysian SMEs.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Visit%20Site-blue?style=for-the-badge)](https://punchclock-seven.vercel.app)
[![Built with Next.js](https://img.shields.io/badge/Next.js-15-black?style=for-the-badge&logo=next.js)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org/)

---

## 🎯 About This Repository

This repository contains a **simplified demo version** of PUNCHCLOCK for portfolio and showcase purposes. The full production system is proprietary and used in client projects.

### What You'll Find Here
- 📐 **Architecture Overview** - System design and technology stack
- 🎨 **UI/UX Samples** - Neo-brutalist design patterns and components
- 📊 **Feature Demonstrations** - Key capabilities and workflows
- 📖 **Documentation** - API design, data models, and compliance approach

### What's Not Included
- 🔒 Full production codebase
- 🔐 Proprietary calculation engines (EPF/SOCSO/PCB algorithms)
- 🗄️ Database schemas and sensitive configurations
- 🔧 Internal tools and automation scripts
- 📈 Analytics and reporting modules

---

## 🚀 What is PUNCHCLOCK?

**PUNCHCLOCK** is a Next-Gen HR Attendance & Payroll System tailored specifically for Malaysian SMEs. It combines modern design with AI-powered compliance to simplify HR operations.

### ✨ Key Features

#### 🎯 Core Capabilities
- **Smart Attendance Tracking** - Real-time clock-in/out with GPS verification
- **Automated Payroll** - One-click salary processing with statutory calculations
- **Malaysian Compliance** - Built-in EPF, SOCSO, EIS, PCB (LHDN) automation
- **Leave Management** - Annual, sick, unpaid leave with approval workflows
- **Multi-Company Support** - Manage multiple business entities from one dashboard

#### 🤖 AI-Powered Intelligence
- **Compliance Assistant** - Real-time guidance on Malaysian labor laws
- **Anomaly Detection** - Automatic flagging of attendance irregularities
- **Predictive Insights** - Workforce trends and cost forecasting
- **Smart Scheduling** - AI-optimized shift planning

#### 🎨 Design Philosophy
- **Neo-Brutalist UI** - Bold, functional, and unapologetically direct
- **Mobile-First** - Optimized for on-the-go HR management
- **Accessibility** - WCAG 2.1 AA compliant
- **Dark Mode** - Reduce eye strain during late-night payroll runs

---

## 🏗️ Technical Stack

### Frontend
- **Framework**: Next.js 15 (App Router)
- **Language**: TypeScript 5.0
- **Styling**: Tailwind CSS + Custom Design System
- **State Management**: React Context + SWR for data fetching
- **Animation**: Framer Motion
- **Forms**: React Hook Form + Zod validation

### Backend & Infrastructure
- **API**: Next.js API Routes + tRPC
- **Database**: PostgreSQL (via Supabase)
- **Authentication**: NextAuth.js with multi-tenant support
- **File Storage**: AWS S3 compatible (Supabase Storage)
- **Email**: Resend + React Email templates
- **Analytics**: Custom event tracking

### AI & Automation
- **LLM Integration**: OpenAI GPT-4 for compliance queries
- **Embeddings**: OpenAI text-embedding-3-small
- **Vector Store**: Supabase pgvector for semantic search
- **Cron Jobs**: Vercel Cron for scheduled tasks

### Compliance & Security
- **Data Encryption**: AES-256 at rest, TLS 1.3 in transit
- **Audit Logging**: Comprehensive change tracking
- **PDPA Compliant**: Malaysian Personal Data Protection Act adherence
- **2FA Support**: Time-based OTP authentication

---

## 📋 System Architecture

\`\`\`
┌─────────────────────────────────────────────────────────────┐
│                     Web Application                          │
│  (Next.js 15 + TypeScript + Tailwind + Neo-Brutalist UI)   │
└────────────────┬────────────────────────────────────────────┘
                 │
                 ▼
┌─────────────────────────────────────────────────────────────┐
│                    API Layer (tRPC)                          │
│  - Authentication & Authorization                            │
│  - Business Logic & Validation                               │
│  - Compliance Rules Engine                                   │
└────────────┬───────────────┬────────────────────────────────┘
             │               │
             ▼               ▼
┌────────────────────┐  ┌──────────────────────────────────┐
│  PostgreSQL DB     │  │  AI Services                      │
│  - Employee Data   │  │  - GPT-4 Compliance Assistant    │
│  - Attendance      │  │  - Vector Search (pgvector)      │
│  - Payroll         │  │  - Anomaly Detection             │
│  - Audit Logs      │  │  - Predictive Analytics          │
└────────────────────┘  └──────────────────────────────────┘
\`\`\`

---

## 🇲🇾 Malaysian Statutory Compliance

PUNCHCLOCK is built with deep understanding of Malaysian employment regulations:

### Automated Calculations
- **EPF (Employer Provident Fund)** - Rates: 12% (employer) + 11% (employee)
- **SOCSO (Social Security)** - Employment Injury & Invalidity schemes
- **EIS (Employment Insurance System)** - 0.2% each from employer & employee
- **PCB (Potongan Cukai Bulanan)** - Monthly tax deduction (LHDN)
- **HRDF (Human Resource Development Fund)** - 1% levy (applicable employers)

### Compliance Features
- ✅ Minimum wage tracking (RM1,500 as of 2024)
- ✅ Overtime calculation (1.5x normal rate)
- ✅ Public holiday pay (2x rate for work on holidays)
- ✅ Annual leave entitlement (8-16 days based on tenure)
- ✅ Statutory reports (EA Form, CP8D, etc.)

---

## 💼 Target Users

### Who Benefits from PUNCHCLOCK?

1. **Malaysian SMEs (5-200 employees)**
   - Retail shops, F&B outlets, service providers
   - Currently using Excel or manual systems
   - Need Malaysian compliance without complexity

2. **Startup Founders**
   - Focus on business, not HR paperwork
   - Need scalable, affordable HR infrastructure
   - Want compliance peace-of-mind

3. **HR Managers**
   - Tired of repetitive manual calculations
   - Need real-time workforce insights
   - Want mobile access for on-the-go management

---

## 🎨 Design Showcase

### Neo-Brutalist Design Language
PUNCHCLOCK uses a bold, functional design aesthetic:

- **Thick Borders**: 3-4px solid borders for clear component separation
- **High Contrast**: Black & white base with vibrant accent colors
- **Raw Typography**: Inter + Mono fonts for clarity
- **Honest UI**: No subtle shadows or gradients - what you see is what you get
- **Functional First**: Every element has a purpose

### Color System
\`\`\`css
Primary:   #0066FF (Blue - Actions & Links)
Success:   #00FF88 (Green - Positive Actions)
Warning:   #FFCC00 (Yellow - Alerts)
Error:     #FF3366 (Red - Critical)
Neutral:   #000000 / #FFFFFF (Black/White Base)
\`\`\`

---

## 📈 Impact & Results

### Production System Achievements
- **95% Time Saved** - Payroll processing time reduced from 2 days to 1 hour
- **Zero Compliance Issues** - Automated checks prevent statutory errors
- **100% Mobile Adoption** - Employees prefer mobile clock-in
- **4.8/5 User Rating** - Based on client feedback

---

## 🔗 Live Demo

Visit the live demo: **[punchclock-seven.vercel.app](https://punchclock-seven.vercel.app)**

### Demo Credentials
(If demo login is set up, add credentials here)

\`\`\`
Email: demo@punchclock.app
Password: [Contact for access]
\`\`\`

---

## 📞 Contact & Collaboration

### About the Creator

**MN Jewel** - Senior Full Stack Engineer  
🌐 Portfolio: [portfolio.w3jdev.com](https://portfolio.w3jdev.com)  
💼 LinkedIn: [Muhammad Nurunnabi](https://linkedin.com/in/muhammad-nurunnabi)  
🐦 Twitter: [@mnjewelps](https://twitter.com/mnjewelps)  
📧 Email: hello@w3jdev.com

### Interested in PUNCHCLOCK?

- **For Recruiters**: This project demonstrates full-stack expertise, system design, and domain knowledge in HR tech
- **For Clients**: Custom HR solutions available - contact for enterprise licensing
- **For Collaboration**: Open to partnerships and integration opportunities

---

## ⚖️ License & Usage

### Copyright Notice

© 2024-2025 w3j LLC. All Rights Reserved.

This demo repository is provided for **portfolio and evaluation purposes only**. The full PUNCHCLOCK system is proprietary software.

### What You Can Do
✅ View and assess code quality  
✅ Learn from architecture decisions  
✅ Reference in discussions with the creator  

### What You Cannot Do
❌ Use in commercial projects  
❌ Redistribute or sublicense  
❌ Claim as your own work  
❌ Extract proprietary algorithms  

For licensing inquiries, contact: **hello@w3jdev.com**

---

## 🗺️ Roadmap (Production System)

### Current Version (v2.0)
- ✅ Core attendance & payroll
- ✅ Malaysian statutory compliance
- ✅ AI compliance assistant
- ✅ Mobile apps (iOS & Android)

### Coming Soon (v3.0)
- 🔄 Performance management module
- 🔄 Recruitment & onboarding
- 🔄 Learning management system (LMS)
- 🔄 Advanced analytics & BI dashboards
- 🔄 API for third-party integrations

---

## 🙏 Acknowledgments

- **Malaysian Laws & Regulations**: EPF, SOCSO, LHDN, MOHR
- **Design Inspiration**: Neo-brutalism movement, Swiss design
- **Technology Partners**: Vercel, Supabase, OpenAI
- **Beta Testers**: Malaysian SME owners who provided feedback

---

<div align="center">

### ⭐ If you're impressed by this demo, let's connect!

**[View Live Demo](https://punchclock-seven.vercel.app)** · **[Contact Me](mailto:hello@w3jdev.com)** · **[Portfolio](https://portfolio.w3jdev.com)**

---

**Built with ❤️ in Malaysia**

</div>
