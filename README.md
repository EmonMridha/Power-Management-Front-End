## LIVE LINK
Here the live link: https://assignment-05-flax.vercel.app/
# ⚡ GridSync — Smart Electricity & Power Management System

GridSync is a smart electricity management platform designed to improve power distribution management, load-shedding scheduling, and outage response. It connects customers, technicians, and administrators through a centralized system that makes electricity management more transparent, organized, and efficient.

Customers can monitor scheduled power outages in their areas, report unexpected electricity interruptions, and receive updates about restoration progress. Administrators can manage electricity infrastructure, schedule outages, assign technicians, and monitor overall operations.

## 🚀 Key Features

### 👤 Customer
- View scheduled load-shedding and power outage schedules.
- Monitor electricity availability in their respective areas.
- Report unexpected power outages.
- Track reported outage status and restoration progress.
- Receive notifications about scheduled and unexpected outages.
- View previous outage history.

### 🛠️ Technician
- View assigned outage and maintenance requests.
- Accept and manage assigned tasks.
- Update repair and restoration progress.
- Report maintenance activities.
- Update outage status after successful restoration.

### 🔐 Administrator
- Manage customers, technicians, and administrative accounts.
- Manage electricity distribution infrastructure.
- Create and manage load-shedding schedules.
- Monitor scheduled and unexpected outages.
- Assign technicians to reported outages.
- Manage outage priorities and critical areas.
- Monitor electricity distribution activities.
- Access operational analytics and outage history.

## 🏗️ Electricity Infrastructure Hierarchy

GridSync follows a structured electricity distribution hierarchy:


Power Authority
      │
      ▼
Distribution Zone
      │
      ▼
Substation
      │
      ▼
Feeder
      │
      ▼
Area


This hierarchical structure allows administrators to manage electricity distribution and outage schedules at different geographical and operational levels.

## 🔄 Outage Management Workflow

Unexpected outages follow a structured workflow to ensure proper tracking and restoration.


REPORTED
    │
    ▼
ASSIGNED
    │
    ▼
IN_PROGRESS
    │
    ▼
REPAIRING
    │
    ▼
RESTORED


Each stage provides visibility into the outage resolution process, allowing customers and administrators to monitor progress.

## 🧰 Technology Stack

### Backend
- Node.js
- TypeScript
- Express.js
- PostgreSQL
- Prisma ORM
- Zod (Data Validation)
- JWT Authentication

### Additional Integrations
- Redis (Caching)
- Stripe / bKash / SSLCommerz (Payment Integration)
- Google OAuth (Social Authentication)

### Development Tools
- Git & GitHub
- Postman
- VS Code

## 🔒 Security & Architecture

- Role-Based Access Control (RBAC).
- JWT-based authentication.
- Request validation using Zod.
- Centralized error handling.
- Standardized API responses.
- Pagination, filtering, and searching.
- Secure handling of sensitive information.
- Audit logging for important operations.

## 📂 Project Structure


GridSync/
├── src/
│   ├── app/
│   ├── config/
│   ├── middlewares/
│   ├── modules/
│   ├── routes/
│   ├── utils/
│   └── server.ts
├── prisma/
│   └── schema.prisma
├── tests/
├── .env.example
├── .gitignore
├── package.json
└── tsconfig.json


*The directory structure is illustrative and should be adjusted to match the actual repository.*

## ⚙️ Installation & Setup

### 1. Clone the repository

```bash
git clone <YOUR_REPOSITORY_URL>
cd GridSync
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Create a `.env` file in the project root.

```env
PORT=5000
DATABASE_URL="your_postgresql_connection_string"

JWT_SECRET="your_jwt_secret"

REDIS_URL="your_redis_connection_string"
```

Add other credentials required by the integrations you enable.

### 4. Configure the database

```bash
npx prisma generate
npx prisma migrate dev
```

### 5. Start the development server

```bash
npm run dev
```

The API should now be available at:

```text
http://localhost:5000
```


## 🎯 Project Goals

- Improve transparency in electricity distribution.
- Make load-shedding schedules accessible to customers.
- Simplify unexpected outage reporting.
- Improve technician assignment and maintenance coordination.
- Reduce delays in outage resolution.
- Provide administrators with better operational visibility.

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

1. Fork the repository.
2. Create a new feature branch.
3. Commit your changes.
4. Push the branch.
5. Open a Pull Request.

## 📄 License

This project is developed for educational and practical software development purposes.

---

**GridSync — Smarter Electricity Management, Better Power Distribution.** ⚡
