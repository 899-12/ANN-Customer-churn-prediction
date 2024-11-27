# Customer Churn Prediction using Artificial Neural Network (ANN)

This project demonstrates a customer churn prediction system using an Artificial Neural Network (ANN). The model predicts whether a customer will churn (leave a service) based on the provided dataset. The application is built using **Streamlit** for an interactive and user-friendly interface.

---

## Table of Contents

1. [Introduction](#introduction)  
2. [Dataset Description](#dataset-description)  
3. [Steps Involved](#steps-involved)  
4. [Technology Stack](#technology-stack)  
5. [How to Run the Application](#how-to-run-the-application)  
6. [Project Structure](#project-structure)  
7. [Conclusion](#conclusion)  

---

## Introduction

Customer churn is a critical problem for many businesses, where retaining customers is often cheaper than acquiring new ones. This project uses an Artificial Neural Network (ANN) to analyze customer data and predict churn.

---

## Dataset Description

The dataset contains customer information such as demographics, geography, and account details.  
The **`Exited`** column indicates whether a customer churned (1) or not (0).  
The key columns used in the model include:

- Gender  
- Geography  
- Credit Score  
- Age  
- Balance  
- Estimated Salary  
- Tenure  
- Exited (Target Variable)  

---

## Steps Involved

### 1. **Feature Extraction**
- Unnecessary columns are dropped from the dataset.  
- Focused on retaining relevant features for the model.

### 2. **Encoding Categorical Variables**
- **`Gender`** and **`Geography`** columns are encoded:  
  - Label Encoding for **`Gender`**.  
  - One-Hot Encoding for **`Geography`**.

### 3. **Target Variable Selection**
- The **`Exited`** column is chosen as the target variable for prediction.

### 4. **Data Splitting**
- The dataset is split into training and testing sets to evaluate model performance.

### 5. **Model Building**
- Built using the **Sequential Layer API** in TensorFlow/Keras.  
- Key layers:
  - Input Layer
  - Hidden Layers (with activation functions)
  - Output Layer (with sigmoid activation for binary classification)  

### 6. **Integration with Streamlit**
- Deployed the model into a **Streamlit** web application.  
- The app allows users to input customer details and view the churn prediction.

---

## Technology Stack

- **Programming Language**: Python  
- **Frameworks**: TensorFlow/Keras, Streamlit  
- **Libraries**: Pandas, NumPy, Scikit-learn, Matplotlib  

---

## How to Run the Application

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/your-repo-link
   cd customer-churn-ann
   ```bash 
2. **Install Dependencies**
    Install all required libraries from the requirements.txt file:
'''python
  pip install -r requirements.txt
3. **Run the Streamlit Application**
```python
   streamlit run app.py
