
# 🏏 Intelligent Sports Team Management Powered by Machine Learning

An intelligent, machine-learning-powered web application designed to transform cricket team management through data-driven player evaluation, auction price prediction, team selection, and match outcome prediction.

The platform focuses on modern cricket leagues such as the **Indian Premier League (IPL)** and **Women's Premier League (WPL)**, helping team managers, coaches, and analysts make smarter and more informed decisions.

---

## 📌 Project Overview

Traditional cricket team management often depends on manual judgment, fragmented statistics, and intuition. This project addresses these challenges by integrating machine learning algorithms with a centralized web-based analytics platform.

The system provides tools for analyzing player performance, estimating fair auction prices, predicting match-winning probabilities, comparing players, managing team rosters, and simulating cricket matches.

It combines web technologies with machine learning to deliver an integrated sports management solution.

---

## ✨ Key Features

### 1. User Authentication
- Secure user registration and login.
- Authenticated access to the application.
- Personalized dashboard.

### 2. Player Management
- Explore detailed player profiles.
- View player performance history.
- Analyze batting and bowling statistics.
- Track fitness scores and injury history.
- Compare multiple players.

### 3. Player Performance Prediction
- Predict future player performance using a **Random Forest Regressor**.
- Analyze historical performance statistics.
- Evaluate players based on multiple parameters.

### 4. Auction Price Prediction
- Estimate player auction prices using a **Gradient Boosting Regressor**.
- Consider player age, runs, average, strike rate, wickets, economy, fitness, and recent form.
- Support data-driven auction decisions.

### 5. Match-Winning Prediction
- Predict match-winning outcomes using a **Random Forest Classifier**.
- Analyze relevant player and team performance factors.
- Provide prediction-based match insights.

### 6. Best Team Selection
- Analyze player statistics.
- Compare player strengths.
- Support balanced team composition.
- Identify suitable players for team selection.

### 7. Auction Management
- Manage player auction information.
- Evaluate player values.
- Support team-building decisions within budget constraints.

### 8. Match Simulation
- Simulate cricket match scenarios.
- Analyze potential match outcomes.
- Support strategic decision-making.

### 9. Centralized Dashboard
- Access player analytics.
- View prediction results.
- Manage teams and players.
- Navigate between application modules.

---

## 🧠 Machine Learning Models

The project implements three machine learning algorithms:

| Model | Algorithm | Purpose |
|---|---|---|
| Player Performance Prediction | Random Forest Regressor | Predict player performance |
| Auction Price Prediction | Gradient Boosting Regressor | Estimate player auction value |
| Match-Winning Prediction | Random Forest Classifier | Predict match-winning outcomes |

### Dataset Features

The machine learning models use player-related attributes such as:

- Age
- Total Runs
- Batting Average
- Strike Rate
- Total Wickets
- Bowling Economy
- Fitness Score
- Recent Form
- Injury History

### Data Preprocessing

The following preprocessing techniques are applied:

1. Missing-value handling.
2. Categorical data encoding.
3. Feature scaling using `StandardScaler`.
4. Dataset splitting into training and testing sets.
5. Model training and prediction using Scikit-learn.

**Train-Test Split:** 80% training data and 20% testing data.

---

## 🛠️ Technology Stack

### Frontend
- HTML5
- CSS3
- JavaScript (ES6)

### Backend
- Node.js
- Express.js

### Database
- MongoDB
- Mongoose

### Machine Learning
- Python
- Flask
- Pandas
- NumPy
- Scikit-learn

---

## 🏗️ System Architecture

The application follows a multi-layer architecture connecting the frontend, backend, database, and machine learning service.

```text
             USER
               |
               v
      FRONTEND (HTML, CSS,
        JavaScript ES6)
               |
               v
       NODE.JS + EXPRESS.JS
          BACKEND API
          /         \
         /           \
        v             v
    MONGODB       PYTHON FLASK
    DATABASE      ML SERVICE
                      |
                      v
                MACHINE LEARNING
                    MODELS
                      |
          --------------------------
          |            |           |
          v            v           v
       Random       Gradient    Random
       Forest       Boosting    Forest
       Regressor    Regressor   Classifier
          |            |           |
          v            v           v
       Player       Auction      Match
     Performance     Price      Prediction
     Prediction   Estimation
```

### Application Workflow

1. The user accesses the web application through the frontend.
2. The frontend communicates with the Node.js and Express.js backend.
3. The backend retrieves or stores information in MongoDB.
4. When predictions are requested, the backend communicates with the Python Flask service.
5. Flask processes the input data and executes the appropriate trained ML model.
6. Prediction results are returned to the backend.
7. The frontend displays the results through the dashboard.

---

## 📂 Project Modules

| Module | Description |
|---|---|
| Authentication | User registration and login |
| Dashboard | Centralized application interface |
| Player Management | Player profiles and statistics |
| Player Comparison | Comparative player analytics |
| Performance Prediction | Predicts player performance |
| Auction Management | Player auction management |
| Auction Price Prediction | Estimates player auction values |
| Best Team Selection | Helps select balanced teams |
| Match Simulation | Simulates cricket match scenarios |
| Match Prediction | Predicts match-winning outcomes |

---

## ⚙️ Installation and Setup

### Prerequisites

Make sure you have installed:

- Node.js
- npm
- Python 3.x
- MongoDB
- Git

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/intelligent-sports-team-management.git
```

### Step 2: Navigate to the Project Directory

```bash
cd intelligent-sports-team-management
```

### Step 3: Install Node.js Dependencies

```bash
npm install
```

### Step 4: Install Python Dependencies

Create and activate a Python virtual environment:

```bash
python -m venv venv
```

Activate it:

**Windows:**
```bash
venv\Scripts\activate
```

**Linux / macOS:**
```bash
source venv/bin/activate
```

Install the required Python packages:

```bash
pip install flask pandas numpy scikit-learn
```

### Step 5: Configure MongoDB

Start your MongoDB server and configure the database connection string in your environment variables.

Example `.env` file:

```env
PORT=5000
MONGO_URI=mongodb://127.0.0.1:27017/sports_management
```

Adjust the port and configuration according to your backend and Flask service setup.

### Step 6: Start the Backend Server

```bash
npm start
```

### Step 7: Start the Flask ML Service

Navigate to the machine learning directory and execute:

```bash
python app.py
```

### Step 8: Open the Application

Open the frontend in your browser or access it through the configured backend server.

---

## 📊 Machine Learning Workflow

```text
Player Dataset
      |
      v
Data Collection
      |
      v
Data Preprocessing
      |
      v
Feature Selection
      |
      v
Train-Test Split (80:20)
      |
      v
Model Training
      |
      v
Model Evaluation
      |
      v
Prediction
      |
      v
Results on Dashboard
```

---

## 🎯 Project Objectives

- Develop a centralized cricket team management platform.
- Apply machine learning to cricket player analytics.
- Predict player performance using historical statistics.
- Estimate fair auction prices for players.
- Predict potential match-winning outcomes.
- Improve team selection and squad composition.
- Reduce dependency on subjective decision-making.
- Provide an interactive and data-driven decision-support system.

---

## 🚀 Future Enhancements

- Integration with real-time IPL and WPL cricket data.
- Live match score integration.
- Advanced player performance analytics.
- Deep learning-based prediction models.
- Interactive statistical visualizations.
- Automated optimal playing XI selection.
- Advanced auction strategy recommendations.
- Mobile application integration.
- Integration with live cricket APIs.

---

## 👨‍💻 Project Team

**Project Title:** Intelligent Sports Team Management Powered by Machine Learning

**Developed By:**

1. Md Khizar Hamed
2. Syed Maroof
3. Vedant More

**Project Guide:** Ms. R. B. Bacchewar

**Department:** Computer Science and Engineering

**College:** MGM's College of Engineering, Nanded

---

## 🙏 Acknowledgement

We sincerely express our gratitude to our project guide, Ms. R. B. Bacchewar, for her valuable guidance, continuous support, suggestions, and encouragement throughout the development of this project.

We also extend our thanks to Dr. A. M. Rajurkar, Head of the Computer Science and Engineering Department, and Dr. G. S. Lathkar, Director of MGM's College of Engineering, Nanded, for providing the necessary facilities and support.

Finally, we thank everyone who directly or indirectly contributed to the successful completion of this project.

---

## 📜 License

This project is developed for academic and educational purposes.

---

## ⭐ Support

If you find this project interesting or useful, consider giving the repository a star ⭐ on GitHub.

**Intelligent Sports Team Management Powered by Machine Learning — Making Cricket Decisions Smarter with AI.**
