<h1>📩 Spam Detection Model</h1>

A Machine Learning model that classifies SMS messages as 📬 Ham (Not Spam) or 🚨 Spam using NLP techniques and Multinomial Naive Bayes.

📊 Accuracy

✅ ~98%

📂 Files in this Repo

📝 notebook79952c767c.ipynb → Training & evaluation code

🤖 spam_model.pkl → Trained model file

🔠 vectorizer.pkl → TF-IDF vectorizer for text preprocessing

<h1>⚙️ How to Use</h1>
Clone the repo

git clone https://github.com/your-username/spam-detection-model.git 

cd spam-detection-model

import pickle

model = pickle.load(open('spam_model.pkl', 'rb'))

vectorizer = pickle.load(open('vectorizer.pkl', 'rb'))

text = ["You won a free iPhone!"]

prediction = model.predict(vectorizer.transform(text))

print(prediction)

<h1>🚀 Future Upgrades</h1>

🌐 Backend integration (Flask/FastAPI)

💻 Simple web UI

☁️ Deploy online

<h1>📜 License</h1>

 Open source under the MIT License.

