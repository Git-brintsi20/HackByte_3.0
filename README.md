# 🌱 PlantZ - AI-Powered Plant Healthcare Platform

[![Node.js](https://img.shields.io/badge/Node.js-v18+-green.svg)](https://nodejs.org/)
[![React](https://img.shields.io/badge/React-v18+-blue.svg)](https://reactjs.org/)
[![MongoDB](https://img.shields.io/badge/MongoDB-v6+-green.svg)](https://mongodb.com/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-v2.0+-orange.svg)](https://tensorflow.org/)
[![Gemini API](https://img.shields.io/badge/Gemini-API-purple.svg)](https://ai.google.dev/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

> **Democratizing Plant Care Through AI-Powered Assistance**

PlantZ is an innovative web application that breaks down barriers to plant care by providing AI-powered guidance, interactive plant management, and community-driven support. Our platform combines cutting-edge machine learning with intuitive design to make plant care accessible to everyone.

## 🚀 Features

### 🤖 AI-Powered Plant Assistant
- **Gemini API Integration**: Natural language plant care conversations
- **Real-time Advice**: Instant responses to plant care questions
- **Context-Aware**: Maintains conversation history for personalized assistance
- **Multilingual Support**: Breaking language barriers in plant care

### 🌿 Interactive Plant Management
- **Plant Avatars**: Expressive visual representations of plant health
- **Smart Dashboard**: Intuitive overview of all your plants
- **Care Scheduling**: Automated reminders and notifications
- **Progress Tracking**: Monitor plant health over time

### 🔬 Disease Detection & Diagnosis
- **CNN-Powered Analysis**: 98% accuracy in disease identification
- **Instant Diagnosis**: Upload plant photos for immediate analysis
- **Treatment Recommendations**: Evidence-based care suggestions
- **Prevention Tips**: Proactive plant health management

### 💰 Voucher-Sponsor System
- **Economic Accessibility**: Reduced barriers through sponsored resources
- **Community Support**: Connect with gardening suppliers and experts
- **Sustainable Ecosystem**: Mutually beneficial for users and sponsors

## 🛠️ Tech Stack

### Frontend
- **React 18+** - Modern UI framework
- **Tailwind CSS** - Utility-first styling
- **Framer Motion** - Smooth animations
- **Cloudinary** - Image management

### Backend
- **Node.js 18+** - Server runtime
- **Express.js** - Web framework
- **MongoDB 6+** - NoSQL database
- **JWT** - Authentication
- **Cloudflare Turnstile** - Security

### AI/ML
- **Google Gemini API** - Conversational AI
- **TensorFlow** - Disease detection model
- **Scikit-learn** - Machine learning utilities
- **OpenCV** - Image processing

## 📊 Performance Metrics

Our AI models deliver exceptional accuracy:

| Component | Accuracy | Precision | Recall | F1-Score |
|-----------|----------|-----------|--------|----------|
| Disease Detection | 98% | 98% | 98% | 98% |
| Plant Identification | 95% | 94% | 96% | 95% |

**Dataset**: 70,029 training images, 17,572 testing images

## 🏗️ Architecture

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   React Client  │    │   Express API   │    │   MongoDB       │
│   (Frontend)    │◄──►│   (Backend)     │◄──►│   (Database)    │
└─────────────────┘    └─────────────────┘    └─────────────────┘
         │                       │                       │
         │              ┌─────────────────┐             │
         └──────────────►│   Gemini API    │             │
                        │   (AI Assistant)│             │
                        └─────────────────┘             │
                                  │                     │
                        ┌─────────────────┐             │
                        │   TensorFlow    │             │
                        │   (CNN Model)   │◄────────────┘
                        └─────────────────┘
```

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ 
- MongoDB 6+
- npm or yarn

### Installation

```bash
# Clone the repository
git clone https://github.com/Divanshu0212/HackByte_3.0.git
cd HackByte_3.0

# Install dependencies
npm install

# Install frontend dependencies
cd frontend
npm install
cd ..

# Install backend dependencies
cd backend
npm install
cd ..
```

### Environment Setup

Create `.env` files in both frontend and backend directories:

**Backend `.env`**
```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
GEMINI_API_KEY=your_gemini_api_key
CLOUDINARY_CLOUD_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_key
CLOUDINARY_API_SECRET=your_cloudinary_secret
```

**Frontend `.env`**
```env
REACT_APP_API_URL=http://localhost:5000
REACT_APP_TURNSTILE_SITE_KEY=your_turnstile_site_key
```

### Running the Application

```bash
# Development mode (runs both frontend and backend)
npm run dev

# OR run separately
# Backend
cd backend && npm start

# Frontend
cd frontend && npm start
```

Visit `http://localhost:3000` to see the application.

## 📝 API Documentation

### Authentication Endpoints
```
POST /api/auth/register    # User registration
POST /api/auth/login       # User login
POST /api/auth/verify      # Email verification
```

### Plant Management
```
GET    /api/plants         # Get user's plants
POST   /api/plants         # Add new plant
PUT    /api/plants/:id     # Update plant
DELETE /api/plants/:id     # Delete plant
```

### AI Assistant
```
POST /api/chat/message     # Send message to AI
GET  /api/chat/history     # Get conversation history
```

### Disease Detection
```
POST /api/diagnosis/analyze  # Analyze plant image
GET  /api/diagnosis/history  # Get diagnosis history
```

### Development Workflow
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Code Style
- Follow ESLint configuration
- Use Prettier for formatting
- Write meaningful commit messages
- Add tests for new features


## 👥 Team

| Name | Role | 
|------|------|
| **Aryan Kesarwani** | Backend Developer |
| **Salugu Harshita Bhanu** | Frontend & Security | 
| **Prakriti Das** | AI/ML Specialist | 
| **Divanshu Bhargava** | AI/ML Specialist | 
## 🙏 Acknowledgments

- [Google Gemini AI](https://ai.google.dev/) for conversational AI capabilities
- [TensorFlow](https://tensorflow.org/) for machine learning framework
- [Plant Disease Dataset](https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset) contributors
- Open source community for various tools and libraries

## 📞 Support
- **Issues**: [GitHub Issues](https://github.com/Git-brintsi20/HackByte_3.0/issues)
- **Email**: shiki2hustle@gmail.com

## ⭐ Show Your Support

If you find PlantZ helpful, please consider giving it a star on GitHub! Your support helps us continue improving the platform.

---

<div align="center">
  <strong>PlantZ - Breaking down the red tape of plant care, one leaf at a time.</strong>
  <br>
  Made with 💚 by the PlantZ Team
</div>

