# Email Spam Detection Using Machine Learning

## 📌 Project Overview

This project is a beginner-friendly Machine Learning application that classifies email messages as either **Spam** or **Ham (Not Spam)**.

The model uses Natural Language Processing (NLP) techniques to analyze email text and predict whether a message is genuine or an unwanted, promotional, or phishing email.

## 🎯 Objectives

* Analyze email text data using Python.
* Perform Exploratory Data Analysis (EDA).
* Clean and preprocess email text data.
* Convert email messages into numerical features using TF-IDF.
* Train Machine Learning classification models.
* Evaluate model performance.
* Predict whether a new email is Spam or Ham.

## 🛠️ Technologies Used

* **Language:** Python
* **Environment:** Jupyter Notebook
* **Data Manipulation & Analysis:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Machine Learning & NLP:** Scikit-learn, NLTK
* **Model Serialization:** Joblib

## 📊 Dataset

**Dataset:** Email Spam Dataset

The dataset contains labeled email messages structured into two main columns:

| Column | Description |
| :--- | :--- |
| `label` | Message category (`ham` or `spam`) |
| `message` | Email subject and body text |

**Labels:**

* `ham` – Genuine, legitimate email message.
* `spam` – Unwanted, unsolicited, promotional, or phishing email message.

## 🔄 Project Workflow

### 1. Data Collection
Load the email spam dataset into Python using Pandas.

### 2. Data Cleaning
* Check for missing values.
* Remove duplicate email records.
* Remove empty email texts.
* Clean and standardize the `label` and `message` columns.

### 3. Exploratory Data Analysis (EDA)
* Analyze dataset dimensions and data types.
* Count the distribution of Spam and Ham emails.
* Calculate email character length and word count.
* Compute statistical metrics (mean, median, and mode).
* Visualize email distributions using graphs.

### 4. Text Feature Extraction
Use **TF-IDF (Term Frequency-Inverse Document Frequency)** to convert raw email text into numerical feature vectors that Machine Learning algorithms can process.

### 5. Model Training
Split the dataset into training and testing sets, then train classification models using:
* **Multinomial Naive Bayes**
* **Logistic Regression**

### 6. Model Evaluation
Evaluate the trained models using standard classification metrics:
* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

### 7. Spam Prediction
Input a custom email message and predict whether it is classified as Spam or Ham.

### 8. Model Saving
Save the trained model and TF-IDF vectorizer using **Joblib** so they can be reused for future predictions without retraining.

## 📁 Project Folder Structure

```text
Email-Spam-Detection/
│
├── Email_Spam_Detection.ipynb   # Main Jupyter Notebook with code and analysis
├── spam_emails.csv              # Dataset file
├── spam_model.pkl               # Saved trained ML model
├── tfidf_vectorizer.pkl         # Saved TF-IDF vectorizer
└── README.md                    # Project documentation
```

## 🚀 How to Run the Project

**Step 1: Clone the repository**

```bash
git clone https://github.com/YOUR_USERNAME/Email-Spam-Detection.git
```

**Step 2: Navigate to the project directory**

```bash
cd Email-Spam-Detection
```

**Step 3: Install required libraries**

```bash
pip install pandas numpy matplotlib seaborn scikit-learn nltk joblib jupyter
```

**Step 4: Launch Jupyter Notebook**

```bash
jupyter notebook
```

**Step 5: Run the Notebook**
Open `Email_Spam_Detection.ipynb` in your browser and run the cells sequentially.

## 💡 Sample Prediction

**Input:**

```text
Subject: Urgent Claim! You have won a free cash voucher. Click here to redeem your prize now!
```

**Expected Output:**

```text
Prediction: Spam
```

*(Note: Actual predictions depend on the dataset and trained model weights.)*

## 🧠 Learning Outcomes

Through this project, I gained hands-on experience in:

* Python programming for Data Science.
* Data cleaning and email text preprocessing.
* Exploratory Data Analysis (EDA) and statistical profiling.
* Data visualization with Matplotlib and Seaborn.
* Natural Language Processing (NLP) fundamentals.
* TF-IDF feature extraction.
* Training and evaluating classification algorithms.
* Model serialization using Joblib.

## 🔮 Future Improvements

* Build an interactive web application using **Streamlit** or **Flask** for pasting and checking emails.
* Include email headers, sender metadata, and URL indicators as additional features.
* Experiment with other classifiers such as Support Vector Machines (SVM) or Random Forest.
* Train on larger, multi-source email datasets for stronger real-world accuracy.

## 👤 Author

**Gokhul J**

*Machine Learning | Python | Data Science*