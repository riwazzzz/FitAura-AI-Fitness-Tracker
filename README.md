# FitAura – AI-Powered Fitness Tracker & Predictor

Full-stack desktop fitness analytics system developed with C++, Qt, Python, and Machine Learning, featuring fitness scoring, personalized recommendations, and 14-day fitness forecasting.

---

## Overview:

FitAura is a fitness analytics application developed using **C++**, **Qt**, **Python**, and **Machine Learning**. The system allows users to track their daily fitness activities, calculate fitness scores, generate health recommendations, and forecast future fitness performance.

The project demonstrates the integration of traditional software engineering principles with predictive analytics to create a data-driven fitness monitoring solution.

---

## Features:

- User Authentication System
- Daily Fitness Tracking
- Fitness Score Calculation
- Personalized Health Recommendations
- Machine Learning-Based Predictions
- Automated Fitness Report Generation
- JSON-Based Data Exchange
- C++ and Python Integration
- Interactive Graphical User Interface

---

## Technologies Used:

| Technology | Purpose |
|------------|----------|
| C++17 | Core Backend Development |
| Qt Framework | GUI Development |
| Python 3.13 | Machine Learning Module |
| Scikit-Learn | Predictive Modeling |
| Pandas | Data Processing |
| NumPy | Numerical Computation |
| JSON | Data Storage and Exchange |
| Git & GitHub | Version Control |

---

## System Architecture:

```text
User
 │
 ▼
GUI Layer (Qt)
 │
 ▼
C++ Backend
 │
 ▼
Python Machine Learning Engine
 │
 ▼
Predictions & Reports
```

---

## Project Structure:

```text
FitAura/
├── main.cpp
├── user.h
├── user.cpp
├── fitnesslog.h
├── fitnesslog.cpp
├── tracker.h
├── tracker.cpp
├── predictor.py
│
├── outputs/
│   ├── report.txt
│   └── fitness_predictions.json
│
├── assets/
│
└── README.md
```

---

## Object-Oriented Design:

### User Class
Responsible for storing user-related information.

### FitnessLog Class
Stores and manages daily fitness records.

### Tracker Class
Processes fitness data, calculates scores, and generates recommendations.

### AppController Class
Handles application flow and user authentication.

---

## Machine Learning Module:

The Machine Learning subsystem is implemented using Python and Scikit-Learn.

### Algorithm Used:

**Linear Regression**

Used to predict future values for:

- Steps
- Calories Burned
- Sleep Hours
- Water Intake

### Workflow:

```text
Historical Data
      ↓
Data Preprocessing
      ↓
Model Training
      ↓
Prediction Generation
      ↓
JSON Output
```

---

## C++ and Python Integration:

The backend executes the machine learning script using Qt's `QProcess`.

```cpp
QProcess pythonProcess;
pythonProcess.start(pythonExe, QStringList() << scriptPath);
```

The generated predictions are stored in:

- `report.txt`
- `fitness_predictions.json`

and then read back into the C++ application.

---

## 📊 Output

### Fitness Report

The generated report includes:

- Fitness Score
- Health Analysis
- Personalized Recommendations

### Prediction Results:

Forecasts the next 14 days for:

- Steps
- Calories Burned
- Sleep Hours
- Water Intake

---

## Future Enhancements:

- Real-Time Fitness Tracking
- Wearable Device Integration
- Cloud Database Support
- Mobile Application Version
- Advanced Deep Learning Models
- Real-Time Analytics Dashboard

---

## Screenshots:

### Welcome Page

![Welcome Page](screenshots/welcome.png)

### Dashboard

![Dashboard](screenshots/dashboard.png)

### Summary Page

![Summary Page](screenshots/summary.png)

---

## Team:

Riwaz Mahat  
Shreyana Adhikari  
Sulav Pandey

---

## License:

This project was developed for academic and educational purposes. All rights reserved by the authors.
