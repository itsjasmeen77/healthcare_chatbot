# 🩺 Healthcare Chatbot using Machine Learning

## 📌 Project Overview

The **Healthcare Chatbot** is a Machine Learning-based application developed in Python that predicts the most likely disease based on the symptoms entered by the user. The chatbot uses a **Random Forest Classifier** trained on a symptom-disease dataset and provides additional information such as the disease description, confidence score, and recommended precautions.

The chatbot interacts with users through a conversational interface, making it easy to enter symptoms in natural language. It also supports symptom synonyms and fuzzy matching to recognize common spelling mistakes.

---

# 🎯 Objectives

- Predict diseases based on user symptoms.
- Provide disease descriptions and precautions.
- Improve symptom recognition using synonyms and fuzzy matching.
- Offer an interactive healthcare assistance system.
- Demonstrate the use of Machine Learning in healthcare applications.

---

# ✨ Features

- Interactive command-line chatbot
- Disease prediction using Random Forest Classifier
- Symptom extraction from natural language
- Synonym recognition
- Fuzzy matching for misspelled symptoms
- Follow-up questions for better prediction
- Confidence score for predictions
- Disease description
- Recommended precautions
- Personalized user interaction
- Motivational health quotes

---

# 🛠 Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Programming Language |
| Pandas | Data loading and preprocessing |
| NumPy | Numerical operations |
| Scikit-learn | Machine Learning model |
| Random Forest Classifier | Disease prediction |
| LabelEncoder | Encoding disease labels |
| Regular Expressions (re) | Text processing |
| Difflib | Fuzzy symptom matching |
| CSV | Reading master data |
| Random | Random health quotes |

---

# 📂 Project Structure

```
Healthcare-Chatbot/
│
├── chatbot.py
├── requirements.txt
├── README.md
│
├── Data/
│   ├── Training.csv
│   └── Testing.csv
│
├── MasterData/
│   ├── symptom_Description.csv
│   ├── symptom_precaution.csv
│   └── Symptom_severity.csv
│
└── Screenshots/
```

---

# 📊 Dataset

The project uses the following datasets:

### Training.csv

Contains:

- Symptoms
- Disease labels (Prognosis)

Used for training the Random Forest model.

---

### Testing.csv

Used to test and validate the trained model.

---

### symptom_Description.csv

Contains a brief description of every disease.

Example:

| Disease | Description |
|----------|-------------|
| Malaria | A mosquito-borne infectious disease |

---

### Symptom_severity.csv

Contains severity scores for symptoms.

Example:

| Symptom | Severity |
|----------|----------|
| Fever | 5 |

---

### symptom_precaution.csv

Contains precautions for each disease.

Example:

| Disease | Precautions |
|----------|-------------|
| Malaria | Drink water, take medicines, consult doctor |

---

# ⚙ Working of the Project

## Step 1

Load the datasets using Pandas.

---

## Step 2

Remove duplicate symptom columns.

---

## Step 3

Separate

- Features (Symptoms)
- Target (Disease)

---

## Step 4

Encode disease names into numerical labels using LabelEncoder.

---

## Step 5

Split the dataset into training and testing sets.

---

## Step 6

Train the Random Forest Classifier.

---

## Step 7

Load:

- Disease descriptions
- Symptom severity
- Precautions

from CSV files.

---

## Step 8

Accept symptoms from the user.

Example:

```
I have fever, headache and stomach pain
```

---

## Step 9

Extract symptoms using

- Exact Matching
- Synonym Matching
- Fuzzy Matching

---

## Step 10

Convert symptoms into a binary feature vector.

---

## Step 11

Predict the disease using the trained model.

---

## Step 12

Ask follow-up questions related to the predicted disease.

---

## Step 13

Predict the disease again using updated symptoms.

---

## Step 14

Display:

- Predicted Disease
- Confidence Score
- Disease Description
- Precautions
- Health Quote

---

# 🤖 Machine Learning Algorithm

## Random Forest Classifier

Random Forest is an ensemble machine learning algorithm that combines multiple decision trees to improve prediction accuracy.

### Advantages

- High Accuracy
- Handles large datasets
- Reduces overfitting
- Fast prediction
- Robust to noisy data

---

# 📥 User Inputs

The chatbot asks the following information:

- Name
- Age
- Gender
- Symptoms
- Number of days
- Severity level (1–10)
- Pre-existing medical conditions
- Lifestyle habits
- Family medical history
- Follow-up symptom questions

---

# 📤 Output

The chatbot displays:

- Predicted Disease
- Confidence Percentage
- Disease Description
- Recommended Precautions
- Motivational Health Quote

---

# ▶ How to Run the Project

## Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/Healthcare-Chatbot.git
```

---

## Move into the project folder

```bash
cd Healthcare-Chatbot
```

---

## Install required libraries

```bash
pip install -r requirements.txt
```

---

## Run the project

```bash
python chatbot.py
```

---

# 📦 Requirements

```
pandas
numpy
scikit-learn
```

Install using:

```bash
pip install pandas numpy scikit-learn
```

---

# 🔮 Future Enhancements

- GUI using Streamlit or Tkinter
- Voice-based chatbot
- Integration with hospital databases
- Medicine recommendations
- Appointment booking
- Real-time health monitoring
- Support for multiple languages
- Web and mobile application

---

# 📸 Sample Output

```
====== Welcome to HealthCare ChatBot ======

What is your name?
Jasmeen

Enter your age:
20

Describe your symptoms:
I have fever and headache.

Detected Symptoms:
fever
headache

Predicted Disease:
Viral Fever

Confidence:
96.42%

Description:
A viral infection causing fever and body pain.

Precautions:
1. Drink plenty of fluids
2. Take adequate rest
3. Consult a doctor if symptoms worsen
4. Take prescribed medicines

Health is wealth, take care of yourself.
```

---

# ⚠ Disclaimer

This project is developed for **educational purposes only**.

The predictions generated by this chatbot are based on the available dataset and machine learning model. They should **not** be considered a substitute for professional medical advice, diagnosis, or treatment. Always consult a qualified healthcare professional for medical concerns.

---

# 👩‍💻 Author

**Jasmeen**

B.Tech Computer Science Engineering

Healthcare Chatbot using Machine Learning

Academic Project
