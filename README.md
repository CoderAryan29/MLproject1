# Student Exam Performance Prediction

A machine learning project that predicts a student's **maths exam score** based on demographic information, parental education, lunch type, test preparation, reading score, and writing score.

## 📌 Project Overview

The goal of this project is to build an end-to-end machine learning pipeline for predicting student exam performance.

The project covers the complete ML workflow:

* Data ingestion
* Data preprocessing
* Feature engineering
* Model training
* Model evaluation
* Model selection
* Prediction pipeline
* Flask web application

## 📊 Dataset

The dataset contains information about students and their performance in different subjects.

### Features

| Feature                     | Description                                          |
| --------------------------- | ---------------------------------------------------- |
| Gender                      | Student's gender                                     |
| Race/Ethnicity              | Student's ethnic group                               |
| Parental Level of Education | Highest education level of the student's parents     |
| Lunch                       | Type of lunch received                               |
| Test Preparation Course     | Whether the student completed the preparation course |
| Reading Score               | Reading exam score                                   |
| Writing Score               | Writing exam score                                   |

### Target

**Math Score**

The model predicts the student's mathematics exam score.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Flask
* Matplotlib
* Seaborn
* Pickle

## 🤖 Machine Learning

Multiple regression algorithms were evaluated to determine which model performed best on the dataset.

The models were compared using evaluation metrics such as:

* R² Score
* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)

The best-performing model was selected for the final prediction pipeline.

The project achieved an **R² score of approximately 0.88**, indicating that the model explains a substantial portion of the variation in mathematics scores.

## 🔄 Project Workflow

```text
Raw Dataset
     ↓
Data Ingestion
     ↓
Train/Test Split
     ↓
Data Transformation
     ↓
Feature Engineering
     ↓
Model Training
     ↓
Model Evaluation
     ↓
Best Model Selection
     ↓
Prediction Pipeline
     ↓
Flask Web Application
```

## 📁 Project Structure

```text
MLproject1/
│
├── artifacts/
│   ├── model.pkl
│   ├── preprocessor.pkl
│   ├── train.csv
│   └── test.csv
│
├── notebooks/
│   ├── data/
│   └── ...
│
├── src/
│   ├── components/
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   └── model_trainer.py
│   │
│   ├── pipeline/
│   │   ├── predict_pipeline.py
│   │   └── __init__.py
│   │
│   └── __init__.py
│
├── templates/
│   ├── index.html
│   └── home.html
│
├── app.py
├── requirements.txt
├── setup.py
└── README.md
```

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/CoderAryan29/MLproject1.git
cd MLproject1
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate the virtual environment on Windows:

```bash
venv\Scripts\activate
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

## ▶️ Running the Project

Run the Flask application:

```bash
python app.py
```

The application will start locally.

Open the URL displayed in the terminal, usually:

```text
http://127.0.0.1:5000/
```

Enter the student's information and submit the form to receive the predicted mathematics score.

## 📈 Model Evaluation

The project evaluates different regression models and compares their performance using R², MAE, and RMSE.

Example:


Linear Regression

Training R²: ~0.87
Test R²:     ~0.88


The final model is selected based on its performance on the test data.

## 💡 Key Learning Outcomes

Through this project, I implemented an end-to-end machine learning workflow including:

* Handling structured/tabular data
* Exploratory data analysis
* Categorical feature encoding
* Numerical feature scaling
* Building preprocessing pipelines
* Training multiple regression models
* Comparing model performance
* Saving trained models using Pickle
* Creating a prediction pipeline
* Deploying the model using Flask

## 🚀 Future Improvements

Possible improvements include:

* Cross-validation
* Improved UI/UX
* Cloud deployment
* Experiment tracking
* Additional feature engineering
* Model monitoring

## 👨‍💻 Author

    "ARYAN"

This project was created as part of my machine learning learning journey.
