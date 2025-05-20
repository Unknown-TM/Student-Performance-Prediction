# Student Performance Prediction

This project aims to predict student performance levels (`High`, `Medium`, or `Low`) based on academic scores and demographic features using machine learning.

## Project Overview

The model is trained using a dataset of students’ math, reading, and writing scores along with categorical attributes like test preparation course. The target variable is a categorized performance level based on the average of the scores.

### Dataset

- **Source**: Local CSV file
- **Features**:
  - Gender
  - Race/Ethnicity
  - Parental Level of Education
  - Lunch
  - Test Preparation Course
  - Math Score
  - Reading Score
  - Writing Score
- **Target**:
  - Performance (Low, Medium, High — based on average score)

## Workflow

1. **Preprocessing**:
   - Feature engineering: Calculate average score
   - Categorize average into `Low`, `Medium`, or `High`
   - Encode categorical variables
   - Scale features

2. **Model**:
   - Trained using `RandomForestClassifier`
   - Evaluation includes confusion matrix and classification report

3. **Serialization**:
   - Trained model, scaler, and label encoders saved using `joblib`

4. **Sample Prediction**:
   - Uses two synthetic student profiles to demonstrate predictions and visualization

## Dependencies

- pandas
- numpy
- scikit-learn
- seaborn
- matplotlib
- joblib
