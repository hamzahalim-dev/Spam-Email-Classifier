Email Spam Classifier

A simple machine learning model to classify emails as Spam or Not Spam using Logistic Regression and TF-IDF vectorization.

Features

Converts email text into numerical format using TF-IDF.

Trained Logistic Regression model for classification.

Achieves around 96% accuracy on test data.

Setup

Run the following command to install required libraries:
**pip install pandas scikit-learn**
Usage

Load the trained model and vectorizer using pickle.

Convert the input email text into numerical format using the vectorizer.

Pass the transformed text to the model to get predictions.

The model will return either "Spam" or "Not Spam".

Example workflow:

Load model and vectorizer.

Transform the email text with TF-IDF.

Use model.predict() to get the classification.

📊 Model Performance
Metric	Score
Accuracy	96%
Precision	95%
Recall	94%
F1-score	94%

🔮 Future Work

Experiment with more advanced algorithms like Random Forest or BERT.

Expand dataset for better generalization.

Implement email preprocessing for multilingual support.
