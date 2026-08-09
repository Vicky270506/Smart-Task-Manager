# 🧠 Smart Task Manager

An intelligent, mobile-first task management application that combines **React Native, Flask, Machine Learning, and Reinforcement Learning** to help users manage tasks, predict priorities and durations, and automatically generate personalized schedules.

## ✨ Features

* 📝 Create and manage tasks
* ✅ Track pending and completed tasks
* 🎯 AI-powered task priority prediction
* ⏱️ AI-powered task duration prediction
* 📅 Intelligent smart scheduling using Reinforcement Learning
* 📊 Productivity insights and weekly summaries
* 🤖 Machine Learning model retraining using real user feedback
* 📱 Mobile-first React Native application
* ⚙️ Flask REST API backend
* 💾 SQLite database with SQLAlchemy

## 🏗️ Architecture

```text
Smart-Task-Manager/
│
├── SmartTaskManager/          # React Native mobile application
│   ├── App.js
│   ├── navigation/
│   ├── screens/
│   ├── assets/
│   └── __tests__/
│
├── SMT_server/                # Flask backend
│   ├── app.py
│   ├── generate_data.py
│   ├── ml_models/
│   └── requirements.txt
│
├── Dataset/                   # Datasets used for experimentation
│
├── PROJECT_DOCUMENTATION.md
├── requirement.txt
└── README.md
```

## 🧰 Technology Stack

### Frontend

* React Native
* JavaScript / JSX
* React Navigation

### Backend

* Python
* Flask
* SQLAlchemy
* SQLite
* REST API

### AI / Machine Learning

* Supervised Machine Learning
* Task duration prediction
* Task priority prediction
* Reinforcement Learning
* TF-Agents
* DQN-based scheduling

## 🔌 API Endpoints

| Method | Endpoint                      | Description               |
| ------ | ----------------------------- | ------------------------- |
| GET    | `/api/v1/tasks`               | Get all tasks             |
| POST   | `/api/v1/tasks`               | Create a task             |
| PUT    | `/api/v1/tasks/<id>/complete` | Complete a task           |
| GET    | `/api/v1/insights`            | Get productivity insights |
| GET    | `/api/v1/smart-schedule`      | Generate a smart schedule |
| POST   | `/api/v1/retrain`             | Retrain ML models         |

## 🚀 Getting Started

### Prerequisites

Make sure you have:

* Node.js
* npm or Yarn
* Python 3.8+
* React Native development environment
* Android Studio for Android development
* Xcode for iOS development on macOS

### 1. Clone the repository

```bash
git clone https://github.com/Vicky270506/Smart-Task-Manager.git
cd Smart-Task-Manager
```

### 2. Set up the backend

Create a Python virtual environment:

```bash
python -m venv .venv
```

Activate it on Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

Install the dependencies:

```bash
pip install -r SMT_server/requirements.txt
```

Start the Flask server:

```bash
cd SMT_server
python app.py
```

### 3. Set up the React Native application

Open another terminal:

```bash
cd SmartTaskManager
npm install
```

Run on Android:

```bash
npx react-native run-android
```

For iOS on macOS:

```bash
npx react-native run-ios
```

### 4. Optional: Generate demo data

```bash
cd SMT_server
python generate_data.py
```

## 🤖 How the AI Works

The application uses machine learning to make task management more intelligent.

### Task Duration Prediction

The system estimates how many minutes a task may require using the trained duration prediction model.

### Priority Prediction

The application analyzes task information to estimate its priority or urgency.

### Smart Scheduling

A Reinforcement Learning environment uses a DQN agent to recommend suitable time slots for pending tasks based on the user's productivity patterns.

### Continuous Learning

When a user completes a task, the actual completion time can be sent back to the backend. This feedback can be used to retrain the models and improve future predictions.

## 📊 Productivity Insights

The application provides productivity information such as:

* Weekly task summaries
* Completion patterns
* Productivity trends
* Personalized scheduling recommendations
* Learned productive time slots

## 📚 Documentation

For detailed project architecture, API information, ML/RL details, and development notes, see:

[`PROJECT_DOCUMENTATION.md`](./PROJECT_DOCUMENTATION.md)

## 🔮 Future Improvements

* Improve ML model accuracy
* Add comprehensive API documentation with Swagger/OpenAPI
* Add automated testing and CI/CD
* Improve personalized scheduling
* Add cloud database support
* Add notifications and reminders
* Add authentication and multi-user support
* Improve analytics and productivity visualization

## 👨‍💻 Author

**Vicky270506**

GitHub: https://github.com/Vicky270506

## ⭐ Support

If you find this project useful, consider giving it a ⭐ on GitHub.

---

**Smart Task Manager — Plan smarter. Work better. 🚀**
