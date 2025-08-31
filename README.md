# Smart Study Planner - AI Project

## Overview
Smart Study Planner is an AI-powered application designed to help students optimize their study schedules, improve academic performance, and maintain a healthy lifestyle. The project leverages machine learning models to provide personalized recommendations based on user data, including exam scores, extracurricular activities, physical activity, sleep hours, and emotional state.

## Features
- **Personalized Study Scheduling:** Uses constraint satisfaction and machine learning to generate optimal study plans.
- **Emotion Detection:** Integrates an emotion recognition model to assess the user's emotional state via facial expressions.
- **Performance Prediction:** Predicts exam scores and provides actionable feedback using CatBoost and other ML models.
- **Lifestyle Analysis:** Considers extracurricular activities, physical activity, and sleep patterns for holistic planning.
- **User Authentication:** Secure login system for personalized experiences.
- **Visualizations:** Generates visual representations of schedules and training history.

## Project Structure
```
app.py                        # Main application entry point
csp_scheduler.py              # Constraint satisfaction scheduler
emotion_detector.py           # Facial emotion recognition logic
ml_classifier.py              # Machine learning classifier for performance
modeltraining.py              # Model training scripts
schedule_visualizer.py        # Schedule visualization
combine.py, pass.py, pratice.py, emotion.py # Supporting scripts
catboost_exam_score.cbm       # CatBoost model for exam score prediction
emotion_recognition_model.h5  # Emotion recognition model
model_*.pkl                   # Pickled ML models
scaler.pkl                    # Data scaler
users.json                    # User data
static/                       # Static files (CSS, images)
templates/                    # HTML templates
plots/, scores/, data/        # Data, results, and visualizations
fer2013/                      # Emotion dataset
myenv1/                       # Python virtual environment
```

## Setup Instructions
1. **Clone the repository:**
   ```powershell
   git clone <repo-url>
   cd <project-directory>
   ```
2. **Create and activate a virtual environment:**
   ```powershell
   python -m venv myenv1
   .\myenv1\Scripts\activate
   ```
3. **Install dependencies:**
   ```powershell
   pip install -r requirements.txt
   ```
   *(If `requirements.txt` is missing, install Flask, numpy, pandas, scikit-learn, catboost, keras, opencv-python, etc.)*
4. **Run the application:**
   ```powershell
   python app.py
   ```
5. **Access the app:**
   Open your browser and go to `http://localhost:5000`

## Usage
- Register or log in as a user.
- Upload or input your study and lifestyle data.
- Use the planner to generate a personalized study schedule.
- Visualize your schedule and track your progress.
- Use the emotion detection feature for mood-based recommendations.

## Models & Data
- **CatBoost, Keras, and Scikit-learn** models are used for predictions.
- Datasets are stored in the `data/` folder.
- Emotion recognition uses the FER2013 dataset.



---
*For any issues or contributions, please open an issue or submit a pull request.*
