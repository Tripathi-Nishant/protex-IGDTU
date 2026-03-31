<p align="center">
  <img src="assets/banner.png" alt="SafeVoice Banner" width="100%">
</p>

# 🛡️ SafeVoice

**SafeVoice** is a professional-grade anonymous reporting and corporate ethics management platform. It empowers employees to report workplace concerns safely and anonymously, while providing ethics panels and administrators with powerful tools to track, investigate, and resolve issues effectively.

---

## ✨ Key Features

### 👤 For Employees
- **Anonymous Reporting**: File complaints without revealing your identity.
- **Tracking Code**: Receive a unique tracking code to follow the progress of your complaint anonymously.
- **Evidence Uploads**: Securely attach files and documents to support your report.
- **Intuitive Dashboard**: Simple interface to manage and track your submissions.

### ⚖️ For Ethics Panel
- **Voting System**: Collaboratively decide on the resolution of complaints through a secure voting mechanism.
- **Leaderboard**: Track performance metrics such as resolution speed and majority consensus.
- **Ethics Scoring**: Earn points based on accurate and timely participation in ethics reviews.
- **Detailed Analytics**: Visualize voting trends and complaint distribution.

### 🔑 For Administrators
- **Centralized Management**: Full oversight of all complaints and user roles across the organization.
- **Smart Alerts**: Automated detection of patterns like accused thresholds or department-specific clusters.
- **System Monitoring**: Logs for system misuse and audit trails for transparency.
- **Role Management**: Control access for Employees, Ethics Members, and Admins.

---

## 🛠️ Technology Stack

SafeVoice is built with a modern, high-performance stack for scalability and security.

### Frontend
- **React 19**: Utilizing the latest React features for a responsive UI.
- **Vite**: Ultra-fast development environment and build tool.
- **Tailwind CSS 4**: Next-generation utility-first styling.
- **Framer Motion**: Smooth, high-end micro-animations.
- **Recharts**: Data visualization for ethics dashboards.
- **Lucide React**: Clean and professional iconography.

### Backend
- **Node.js & Express**: Scalable and robust API architecture.
- **Prisma ORM**: Type-safe database access and migrations.
- **PostgreSQL**: Enterprise-grade relational database.
- **JWT (JSON Web Tokens)**: Secure, stateless authentication.
- **Multer**: Secure handle for multi-part file uploads.
- **Node-cron**: Automated tasks for deadline tracking and alerts.

---

## 🚀 Getting Started

### Prerequisites
- **Node.js**: v20 or v22 (recommended)
- **PostgreSQL**: Local instance or Docker-based

### 1. Local Development Setup

#### Backend (Server)
1. **Navigate to server**: `cd server`
2. **Install dependencies**: `npm install`
3. **Configure environment**: Create a `server/.env` file and set your `DATABASE_URL`:
   ```env
   DATABASE_URL="postgresql://user:password@localhost:5432/safevoice"
   JWT_SECRET="your_secret_key"
   ```
4. **Initialize database**:
   ```bash
   npm run db:migrate
   npm run db:seed
   ```
5. **Start server**: `npm run dev`

#### Frontend (Client)
1. **Navigate to client**: `cd client`
2. **Install dependencies**: `npm install`
3. **Start Vite server**: `npm run dev`
   *Available at `http://localhost:5173`*

### 2. Docker Setup (Recommended)
If you prefer a containerized environment, you can run everything with a single command:
```bash
docker-compose up --build
```
The application will be available at `http://localhost:8080`.

---

## 🏗️ Architecture & Security

- **Multi-Tenant Ready**: Support for multiple organizations with isolated data.
- **Anonymity Layer**: Complaint-to-User mapping (`AnonMapping`) ensures that even database-level access cannot easily link a report to an identity without explicit permissioning.
- **Role-Based Access Control (RBAC)**: Strict permissioning ensures only authorized personnel can view sensitive complaint details.
- **Audit Logging**: Every action taken on a complaint is tracked for accountability.

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

<p align="center">
  Built with ❤️ for a safer and more ethical workplace.
</p>
