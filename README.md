# Email Spam Classifier

A simple **machine learning model** to classify emails as **Spam** or **Not Spam** using **Logistic Regression** and **TF-IDF vectorization**.

---

## Features
- Text-to-number conversion with **TF-IDF**  
- Trained Logistic Regression model  
- ~96% accuracy on test data  

---

## Setup
```bash
import pickle

# Load model and vectorizer
model = pickle.load(open("model.pkl", "rb"))
vectorizer = pickle.load(open("vectorizer.pkl", "rb"))

# Test email
email = ["Congratulations! You won $1000, claim now!"]
vec = vectorizer.transform(email)
pred = model.predict(vec)
print("Spam" if pred[0] == 1 else "Not Spam")
📊 Model Performance
Metric	Score
Accuracy	96%
Precision	95%
Recall	94%
F1-score	94%
Experiment with more advanced algorithms like Random Forest or BERT.

Expand dataset for better generalization.

Implement email preprocessing for multilingual support.
