[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=19922161&assignment_repo_type=AssignmentRepo)
# Deployment and DevOps for MERN Applications

This assignment focuses on deploying a full MERN stack application to production, implementing CI/CD pipelines, and setting up monitoring for your application.

## Assignment Overview

You will:
1. Prepare your MERN application for production deployment
2. Deploy the backend to a cloud platform
3. Deploy the frontend to a static hosting service
4. Set up CI/CD pipelines with GitHub Actions
5. Implement monitoring and maintenance strategies

## Getting Started

1. Accept the GitHub Classroom assignment invitation
2. Clone your personal repository that was created by GitHub Classroom
3. Follow the setup instructions in the `Week7-Assignment.md` file
4. Use the provided templates and configuration files as a starting point

## Files Included

- `Week7-Assignment.md`: Detailed assignment instructions
- `.github/workflows/`: GitHub Actions workflow templates
- `deployment/`: Deployment configuration files and scripts
- `.env.example`: Example environment variable templates
- `monitoring/`: Monitoring configuration examples

## Requirements

- A completed MERN stack application from previous weeks
- Accounts on the following services:
  - GitHub
  - MongoDB Atlas
  - Render, Railway, or Heroku (for backend)
  - Vercel, Netlify, or GitHub Pages (for frontend)
- Basic understanding of CI/CD concepts

## Deployment Platforms

### Backend Deployment Options
- **Render**: Easy to use, free tier available
- **Railway**: Developer-friendly, generous free tier
- **Heroku**: Well-established, extensive documentation

### Frontend Deployment Options
- **Vercel**: Optimized for React apps, easy integration
- **Netlify**: Great for static sites, good CI/CD
- **GitHub Pages**: Free, integrated with GitHub

## CI/CD Pipeline

The assignment includes templates for setting up GitHub Actions workflows:
- `frontend-ci.yml`: Tests and builds the React application
- `backend-ci.yml`: Tests the Express.js backend
- `frontend-cd.yml`: Deploys the frontend to your chosen platform
- `backend-cd.yml`: Deploys the backend to your chosen platform

## Submission

Your work will be automatically submitted when you push to your GitHub Classroom repository. Make sure to:

1. Complete all deployment tasks
2. Set up CI/CD pipelines with GitHub Actions
3. Deploy both frontend and backend to production
4. Document your deployment process in the README.md
5. Include screenshots of your CI/CD pipeline in action
6. Add URLs to your deployed applications

## Resources

- [GitHub Actions Documentation](https://docs.github.com/en/actions)
- [MongoDB Atlas Documentation](https://docs.atlas.mongodb.com/)
- [Render Documentation](https://render.com/docs)
- [Railway Documentation](https://docs.railway.app/)
- [Vercel Documentation](https://vercel.com/docs)
- [Netlify Documentation](https://docs.netlify.com/)
- 


# 🚀 MERN Deployment & DevOps Essentials – Bug Tracker

This project demonstrates how to deploy a full MERN stack application with CI/CD, monitoring, and proper DevOps practices.

---

## 📦 Setup & Run Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/mern-bug-tracker.git
cd mern-bug-tracker
```

### 2. Install Dependencies

#### Backend
```bash
cd backend
npm install
```

#### Frontend
```bash
cd ../frontend
npm install
```

### 3. Environment Variables

Create `.env` files based on the provided `.env.example`.

#### Example for Backend:
```
MONGO_URI=your_mongodb_atlas_connection_string
NODE_ENV=production
```

### 4. Run Locally

#### Backend
```bash
cd backend
node server.js
```

#### Frontend
```bash
cd frontend
npm run dev
```

---

## 🧪 Running & Monitoring Tests

### Backend Tests (Jest + Supertest)
```bash
cd backend
npm test
```

### Frontend Tests (React Testing Library + Jest)
```bash
cd frontend
npm test
```

Use tools like **coverage reports** or GitHub Actions logs to monitor test results.

---

## ⚙️ CI/CD Pipeline Setup

This project uses **GitHub Actions** for continuous integration and deployment.

- `.github/workflows/ci-cd.yml` handles build, test, and deployment.
- Automatic deployment to:
  - **Render** (backend)
  - **Vercel** (frontend)

### ✅ Example Workflow
![CI/CD Pipeline](./screenshots/ci-cd.png)

---

## 🌐 Deployment URLs

- **Frontend (Vercel):** [https://mern-bug-tracker-frontend.vercel.app](https://mern-bug-tracker-frontend.vercel.app)
- **Backend (Render):** [https://mern-bug-tracker-backend.onrender.com](https://mern-bug-tracker-backend.onrender.com)

---

## 🔍 Monitoring & Error Tracking

- **Health Check Endpoint:** `/api/health`
- **Error Tracking:** [Sentry](https://sentry.io)
- **Uptime Monitoring:** [UptimeRobot](https://uptimerobot.com)
- **Performance Monitoring:** Chrome DevTools, Render Metrics Dashboard

---

## 🔄 Rollback & Maintenance Plan

### Rollback Strategy
- Revert to previous commit and redeploy via GitHub
- Render retains deploy history for easy rollback

### Maintenance Tasks
- Weekly dependency updates using `npm outdated`
- Monthly database backups from MongoDB Atlas
- Monitor logs and metrics on Render dashboard

---

## 📁 Folder Structure
```
mern-bug-tracker/
├── backend/
│   ├── server.js
│   ├── app.js
│   ├── routes/
│   └── middleware/
├── frontend/
│   ├── src/
│   ├── App.jsx
│   └── main.jsx
├── .github/workflows/
│   └── ci-cd.yml
└── README.md
```

---

Happy deploying! 💻🚀
