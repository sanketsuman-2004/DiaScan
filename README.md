# DiaScan

A **Streamlit web application** that predicts the likelihood of diabetes in a patient based on various health parameters. The prediction is made using a **Random Forest Classifier** trained on the **Pima Indians Diabetes Database**.

---

## Features

- **User Input Interface**: Input patient data through sliders for various health metrics.  
- **Diabetes Prediction**: Predicts whether the patient is diabetic or not using a trained machine learning model.  
- **Data Visualization**: Visualizes user input data against the training dataset for context and comparison.  
- **Model Accuracy Display**: Shows the accuracy of the machine learning model.  

---

## How It Works

### 1. User Input
Users provide health data through an intuitive sidebar interface. The following parameters are collected:

- **Pregnancies**: Number of times pregnant  
- **Glucose**: Plasma glucose concentration  
- **Blood Pressure**: Diastolic blood pressure (mm Hg)  
- **Skin Thickness**: Triceps skinfold thickness (mm)  
- **Insulin**: 2-Hour serum insulin (mu U/ml)  
- **BMI**: Body mass index (weight in kg/(height in m)^2)  
- **Diabetes Pedigree Function**: Scores likelihood of diabetes based on family history  
- **Age**: Age of the patient  

### 2. Data Processing
- The input data is formatted into a dataframe matching the training dataset structure.  
- The formatted data is fed into the trained Random Forest model to make a prediction.  

### 3. Machine Learning Model
- **Model Used**: Random Forest Classifier  
- **Training Data**: Pima Indians Diabetes Database  
- **Training & Testing**: Model is trained on a training subset and tested on a test subset for accuracy.  

### 4. Visualization
- **Scatter Plots**: Compare user data with the training dataset across various health parameters (e.g., Age vs. Glucose, Age vs. BMI).  
- User input is highlighted to provide clear visual feedback.  

### 5. Output
- **Prediction**: Displays whether the user is likely diabetic or not.  
- **Model Accuracy**: Shows the reliability of the prediction.  

---

## Usage

1. Run the Streamlit app:

```bash
streamlit run app.py
