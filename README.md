# Email Spam Classifier

This project is a **machine learning model** that classifies emails as **Spam** or **Not Spam** using **Logistic Regression** and **TF-IDF vectorization**.

---

## 📌 Features
- Converts email text into numerical data using **TF-IDF**.
- Trained with **Logistic Regression** for binary classification.
- Achieved **~96% accuracy** on test data.
- Easy to use with saved model and vectorizer.

---

## 📂 Project Structure
email-spam-classifier/
│
├── email.csv # Dataset used for training
├── model.pkl # Saved trained model
├── vectorizer.pkl # Saved TF-IDF vectorizer
├── train_model.py # Script used to train and save the model
└── README.md # Documentation

---

## ⚙️ How to Use

### 1️⃣ Install Required Libraries
```bash
pip install pandas scikit-learn
2️⃣ Load and Use the Model
import pickle

# Load the trained model and vectorizer
model = pickle.load(open("model.pkl", "rb"))
vectorizer = pickle.load(open("vectorizer.pkl", "rb"))

# Example email to test
sample_email = ["Huraay! You won a prize bond of 1 million dollars. Claim it now!"]

# Transform and predict
sample_vector = vectorizer.transform(sample_email)
prediction = model.predict(sample_vector)
confidence = model.predict_proba(sample_vector)

print("Prediction:", "Spam" if prediction[0] == 1 else "Not Spam")
print("Confidence:", confidence)
📊 Model Performance
Metric	Score
Accuracy	96%
Precision	95%
Recall	94%
F1-score	94%
Experiment with more advanced algorithms like Random Forest or BERT.

Expand dataset for better generalization.

Implement email preprocessing for multilingual support.

