

```markdown
# 🌾 AgriTech AI - Smart Farming Assistant
deployed link-- https://bfb-hack.vercel.app/




## 📋 Table of Contents
- [Overview](#-overview)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Prerequisites](#-prerequisites)
- [Installation Guide](#-installation-guide)
- [Environment Variables](#-environment-variables) 
- [Deployment](#-deployment)
- [Contributing](#-contributing)
- [License](#-license)
- [Contact](#-contact)

## 🌱 Overview

**AgriTech AI** is a comprehensive smart farming platform that leverages artificial intelligence to empower farmers with cutting-edge technology. The platform integrates multilingual support, disease detection, personalized crop advisory, and weather alert systems to create an all-in-one agricultural assistant.

### 🎯 Key Benefits
- 👨‍🌾 **For Farmers**: Instant access to agricultural expertise
- 🌍 **Multilingual**: Breaking language barriers in farming communities
- 📱 **Accessible**: Web-based platform accessible from any device
- ⚡ **Real-time**: Live weather updates and alerts

## ✨ Features

### 1. 🤖 AI Multilingual Chatbot
- **Powered by Google Gemini AI**
- Supports multiple Indian and international languages
- Context-aware agricultural conversations
- 24/7 availability for farmer queries

### 2. 🍃 Leaf Disease Detector
- **Deep Learning-based detection**
- Instant disease identification from leaf images
- Treatment recommendations and preventive measures
- Support for multiple crop types

### 3. 🌾 AI-Powered Crop Advisory
- **Soil analysis-based recommendations**
- Personalized crop planning
- Fertilizer and irrigation scheduling
- Weather-integrated suggestions

### 4. ⚡ Weather Alert System
- **Real-time weather monitoring**
- Automated email alerts for severe conditions
- Location-based weather tracking
- Preventive action recommendations

## 🛠️ Tech Stack

### Frontend (Port 3000)
- **Framework**: React.js
- **Styling**: Material-UI / Tailwind CSS
- **HTTP Client**: Axios
- **Deployment**: Vercel

### Backend (Port 5000)
- **Runtime**: Node.js
- **Framework**: Express.js
- **Database**: MongoDB Atlas
- **Authentication**: JWT
- **APIs**: Google Gemini, OpenWeather

### Python Backend (Port 8000)
- **Framework**: Flask
- **ML Libraries**: TensorFlow, PyTorch, OpenCV
- **APIs**: Google Gemini, OpenWeather

### Python Backend (Railways)
- **Framework**: Flask
- **Email Service**: SMTP (Gmail)
- **Scheduling**: APScheduler
- **Deployment**: Railway.app



## 📋 Prerequisites

Before you begin, ensure you have installed:
- **Node.js** (v14 or higher)
- **Python** (3.8 or higher)
- **npm** or **yarn** package manager
- **Git** for version control
- **MongoDB Atlas** account (free tier works)
- **Code editor** (VS Code recommended)

## 🚀 Installation Guide

### Step 1: Clone the Repository
```bash
git clone https://github.com/yourusername/agritech-ai.git

```

### Step 2: Frontend Setup
```bash
cd frontend
npm install
npm run start
```
The frontend will be available at `http://localhost:3000`

### Step 3: Node.js Backend Setup
```bash
cd backend
npm install
npm run start
```
The backend will be available at `http://localhost:5000`

### Step 4: Python Backend Setup (ML Services)
```bash
cd python-backend

# Create virtual environment
# Windows:
python -m venv venv
venv\Scripts\activate

# macOS/Linux:
python3 -m venv venv
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Run the server
python app.py
```
The Python backend will be available at `http://localhost:8000`

### Step 5: Python Backend for Railways (Optional for Local Testing)
```bash
cd python-backend-railways

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run locally
python app.py
```

## 🔐 Environment Variables

### Frontend `.env` (frontend/)
```
REACT_APP_API_BASE_URL=http://localhost:5000/api
REACT_APP_API_BASE_URL2=http://localhost:8000
REACT_APP_API_TIMEOUT=100000
```

### Backend `.env` (backend/)
```
PORT=5000
MONGO_URI=<your_mongodb_connection_string>
JWT_SECRET=<your_jwt_secret_key>
OPENWEATHER_API_KEY=<your_openweather_api_key>
GEMINI_API_KEY=<your_google_gemini_api_key>
FRONTEND_URL=<your_frontend_url>
LOCAL_FRONTEND=http://localhost:3000
```

### Python Backend `.env` (python-backend/)
```
OPENWEATHER_KEY=<your_openweather_api_key>
GEMINI_API_KEY=<your_google_gemini_api_key>
EMAIL_SENDER=<your_gmail_address>
EMAIL_PASSWORD=<your_gmail_app_password>
FRONTEND_URL=http://localhost:3000
```

### Python Backend Railways
- No local `.env` file required
- Configure environment variables directly in Railway dashboard



## ☁️ Deployment

### Frontend Deployment (Vercel)
1. Push code to GitHub repository
2. Connect repository to Vercel
3. Configure environment variables in Vercel dashboard
4. Deploy automatically on push

### Backend Deployment (Render/Heroku)
1. Create account on deployment platform
2. Connect GitHub repository
3. Add environment variables
4. Deploy the Node.js application

### Python Backend Deployment (Railway)
1. Install Railway CLI
2. Navigate to python-backend-railways
3. Run deployment commands:
```bash
railway login
railway init
railway up
```
4. Configure environment variables in Railway dashboard



## 🤝 Contributing Guidelines

We welcome contributions! Please follow these steps:

1. **Fork** the repository
2. **Create** a feature branch
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. **Commit** your changes
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```
4. **Push** to the branch
   ```bash
   git push origin feature/AmazingFeature
   ```
5. **Open** a Pull Request

### Development Standards
- Write clean, documented code
- Follow existing code style
- Add tests for new features
- Update documentation as needed

## 🐛 Troubleshooting

### Common Issues & Solutions

**Issue**: Frontend can't connect to backend
**Solution**: Check if all servers are running on correct ports

**Issue**: MongoDB connection failed
**Solution**: Verify IP whitelist in MongoDB Atlas

**Issue**: Gemini API not working
**Solution**: Check API key validity and quota

**Issue**: Email alerts not sending
**Solution**: Verify Gmail app password is correct

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Contact & Support

- **Project Maintainer**: Agricultural Technology Team
- **Email**: support@agritech-ai.com
- **GitHub Issues**: [Report a bug](https://github.com/yourusername/agritech-ai/issues)
- **Documentation**: [Wiki](https://github.com/yourusername/agritech-ai/wiki)

## 🙏 Acknowledgments

- **Google Gemini AI** for powering intelligent conversations
- **OpenWeather API** for accurate weather data
- **MongoDB Atlas** for reliable database services
- **Vercel** for seamless frontend hosting
- **Railway** for easy backend deployment
- **Agricultural Universities** for domain expertise

## 📊 Project Status

- ✅ Frontend: Complete and deployed
- ✅ Backend: Complete and functional
- ✅ Python ML Services: Operational
- ✅ Weather Alerts: Active
- 🚀 Mobile App: Coming Soon

---

<p align="center">
  Made with ❤️ for the farming community
  <br>
  © 2024 AgriTech AI. All rights reserved.
</p>
```
