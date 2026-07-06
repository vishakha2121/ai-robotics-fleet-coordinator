# 🤖 AI Autonomous Robotics Fleet Coordinator

[![GitHub stars](https://img.shields.io/github/stars/vishakha2121/ai-robotics-fleet-coordinator)](https://github.com/vishakha2121/ai-robotics-fleet-coordinator/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/vishakha2121/ai-robotics-fleet-coordinator)](https://github.com/vishakha2121/ai-robotics-fleet-coordinator/network)
[![License](https://img.shields.io/github/license/vishakha2121/ai-robotics-fleet-coordinator)](https://github.com/vishakha2121/ai-robotics-fleet-coordinator/blob/main/LICENSE)
[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/)
[![React](https://img.shields.io/badge/React-18.2.0-61DAFB.svg)](https://reactjs.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.104.1-009688.svg)](https://fastapi.tiangolo.com/)

> 🚀 AI-powered warehouse robotics fleet coordinator using Multi-Agent Reinforcement Learning, ROS2 simulation, and graph planning algorithms.

## 📋 Overview

An intelligent fleet coordination system that manages hundreds of warehouse robots in real-time using advanced AI techniques. The system handles task allocation, dynamic routing, and collision avoidance with an interactive 3D visualization dashboard.

## ✨ Key Features

### 🤖 Fleet Management
- **Multi-Agent RL**: Intelligent task allocation using reinforcement learning
- **Real-time Monitoring**: Live tracking of all robots in the fleet
- **Status Updates**: Battery levels, task progress, and health monitoring
- **Dynamic Scaling**: Support for 100+ robots simultaneously

### 🗺️ Path Planning & Navigation
- **Graph-Based Planning**: A* and Dijkstra algorithms for optimal routing
- **Collision Avoidance**: Real-time obstacle detection and avoidance
- **Traffic Management**: Intelligent traffic flow optimization
- **Dynamic Re-routing**: Adaptive path planning based on real-time conditions

### 🎮 Simulation & Visualization
- **3D Warehouse Simulation**: Realistic 3D environment using Three.js
- **Live Animations**: Real-time robot movements and interactions
- **Interactive Controls**: Start, pause, and customize simulations
- **Path Visualization**: Visual representation of planned routes

### 📊 Analytics & Insights
- **Performance Metrics**: Efficiency, utilization, and throughput
- **Predictive Analytics**: AI-powered predictions using Gemini API
- **Real-time Dashboards**: Live updates via WebSocket
- **Historical Data**: Comprehensive reporting and analysis

## 🛠️ Tech Stack

### Backend
```yaml
Framework: FastAPI 0.104.1
Language: Python 3.9+
Database: PostgreSQL
AI/ML: PyTorch, Stable-Baselines3, Gymnasium
Path Planning: NetworkX, A*, Dijkstra
Real-time: WebSockets, Redis
API Integration: Google Gemini AI

Framework: React 18.2.0
Styling: Tailwind CSS, Material-UI
3D Visualization: Three.js, React Three Fiber
Charts: Recharts
State Management: React Context API
Real-time: Socket.io-client

Containerization: Docker, Docker Compose
CI/CD: GitHub Actions
Monitoring: Custom logging system
Deployment: Nginx, Gunicorn

git clone https://github.com/vishakha2121/ai-robotics-fleet-coordinator.git
cd ai-robotics-fleet-coordinator

cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt

cd frontend
npm install

# Using Docker
docker-compose up -d postgres

# Or manually create database
createdb fleet_db

# Copy example env files
cp backend/.env.example backend/.env
cp frontend/.env.example frontend/.env

# Edit .env files with your credentials

# Start backend
cd backend
python run.py

# Start frontend (in new terminal)
cd frontend
npm run dev