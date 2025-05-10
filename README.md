COMPANY : CODTECH IT SOLUTIONS

NAME : NAVEEN K

INTERN ID : CT06DA721

DOMAIN : MACHINE LEARNING

DURATION : 6 WEEKS

MENTOR : NEELA SANTHOSH KUMAR


  Task 2 – Sentiment Analysis using TF-IDF and Logistic Regression

  Internship Project - Machine Learning (CodTech)

Hello! This repository contains the solution to **Task 2** of the CodTech Machine Learning Internship. The task was to perform **Sentiment Analysis** on a dataset of customer reviews using **TF-IDF vectorization** and a **Logistic Regression classifier**.

The objective is to automatically determine whether a customer review expresses a **positive** or **negative** sentiment.

---

  Objective

To build a complete NLP pipeline that:
- Takes a dataset of customer reviews
- Preprocesses the text to make it clean and readable
- Converts the text into numerical form using TF-IDF
- Trains a Logistic Regression model to classify sentiment
- Evaluates and visualizes model performance

---

 Dataset

I used a dataset converted from `amazon_cells_labelled.txt` into a CSV format. It contains **999 reviews** with two columns:
- `review` – The customer’s review text
- `sentiment` – The corresponding label (1 = positive, 0 = negative)

---

  Step-by-Step Workflow

 🔹 Step 1: Data Loading
The CSV file was loaded into a pandas DataFrame, and column names were stripped of hidden spaces to avoid errors.

 🔹 Step 2: Data Exploration
I checked for class balance, verified data types, and printed samples to understand the structure.

 🔹 Step 3: Text Preprocessing
A cleaning function was used to:
- Convert text to lowercase
- Remove punctuation, numbers, and extra spaces

The cleaned text was stored in a new column called `cleaned_review`.

 🔹 Step 4: TF-IDF Vectorization
Using `TfidfVectorizer`, I transformed the cleaned text into a numerical matrix of TF-IDF features. This step converts natural language into a format understandable by the model.

 🔹 Step 5: Train-Test Split
The dataset was split 80:20 into training and testing sets.

 🔹 Step 6: Logistic Regression Model
A `LogisticRegression` model from scikit-learn was trained on the TF-IDF vectors.

 🔹 Step 7: Model Evaluation
I predicted sentiments for the test set and evaluated performance using:
- Accuracy Score
- Classification Report (Precision, Recall, F1)

Output:

![Image](https://github.com/user-attachments/assets/4a2a492d-5b30-4105-a11f-d706f932ce83)

