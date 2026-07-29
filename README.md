# 📧 Email Spam Detection using Naive Bayes with Gmail API

A Machine Learning project that detects whether an email is **Spam** or **Ham (Not Spam)** using the **Naive Bayes Classification Algorithm**. The project trains a model on a labeled email dataset, evaluates its performance, and integrates with the **Gmail API** to classify the latest emails from a Gmail inbox in real time.

---

## 📌 Project Overview

Email spam is one of the most common cybersecurity challenges. This project uses the **Multinomial Naive Bayes** algorithm to automatically classify emails as Spam or Ham based on their textual content.

After training the model, it connects securely to a Gmail account using the Gmail API, retrieves the latest emails, predicts whether each email is spam or ham, displays prediction probabilities, and summarizes the results with a graphical analysis.

---

## ⚙️ How the Program Works

The dataset is first loaded and preprocessed by converting the labels into numerical values. The email text is transformed into numerical features using **CountVectorizer**, which converts words into a Bag-of-Words representation. A **Multinomial Naive Bayes** classifier is then trained on the processed data and evaluated using accuracy, classification report, and confusion matrix. The trained model and vectorizer are saved for future use. In the second phase, the application authenticates with Gmail using OAuth 2.0, retrieves recent emails, extracts their subject and body, converts the text into feature vectors, predicts whether each email is Spam or Ham, displays prediction probabilities, and finally visualizes the number of spam and ham emails using a bar chart.

---

## 🛠 Technologies Used

- Python
- Pandas
- Scikit-learn
- CountVectorizer
- Multinomial Naive Bayes
- Joblib
- Gmail API
- Google OAuth 2.0
- Matplotlib

---

## 🔍 Features

- Train a Naive Bayes spam detection model
- Email text preprocessing using CountVectorizer
- Save trained model using Joblib
- Model evaluation using:
  - Accuracy
  - Classification Report
  - Confusion Matrix
- Secure Gmail authentication using OAuth 2.0
- Read the latest Gmail messages
- Predict Spam or Ham for each email
- Display Spam and Ham probabilities
- Summary of classified emails
- Visual analysis using a Bar Chart

---

## 📂 Project Structure

```
Gmail-Detection-API-Naive-Bayes/
│
├── Gmail_predict.py
├── spam.csv
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 📊 Model Evaluation

The project evaluates the trained model using:

- Accuracy Score
- Classification Report
- Confusion Matrix

These metrics help measure the overall performance of the spam classifier before using it on real Gmail emails.

---

## 📈 Output

The application displays:

- First five records of the dataset
- Dataset information
- Model accuracy
- Classification report
- Confusion matrix
- Gmail authentication status
- Latest emails
- Sender
- Subject
- Spam/Ham prediction
- Spam probability
- Ham probability
- Total spam emails
- Total ham emails
- Bar chart showing Spam vs Ham email distribution

---

## 🚀 Installation

### Clone the repository

```bash
git clone https://github.com/your-username/Gmail-Detection-API-Naive-Bayes.git
```

### Navigate to the project

```bash
cd Gmail-Detection-API-Naive-Bayes
```

### Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Project

```bash
python Gmail_predict.py
```

---

## 🔐 Gmail API Setup

1. Create a project in Google Cloud Console.
2. Enable the Gmail API.
3. Create OAuth Client Credentials.
4. Download the credentials file.
5. Rename it as:

```
credentials.json
```

6. Place it inside the project folder.
7. Run the project.
8. Log in with your Gmail account when prompted.
9. A `token.json` file will be created automatically for future authentication.

---

## 📚 Concepts Learned

- Natural Language Processing (NLP)
- Text Vectorization
- Bag of Words
- CountVectorizer
- Naive Bayes Classification
- Model Training
- Model Evaluation
- Confusion Matrix
- Classification Report
- Machine Learning Workflow
- Gmail API Integration
- OAuth Authentication
- Data Visualization

---

## 📌 Future Improvements

- TF-IDF Vectorization
- Support multiple machine learning algorithms
- Deep Learning based spam detection
- Web interface using Flask or Django
- Real-time email monitoring
- Email attachment analysis
- Spam keyword highlighting
- Model performance comparison

---

## 👨‍💻 Author

**Danish Solkar**

Machine Learning Enthusiast | Python Developer | Data Analytics Learner

---

## ⭐ If you found this project useful, consider giving it a Star!
