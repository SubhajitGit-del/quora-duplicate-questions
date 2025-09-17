# Quora Duplicate Question Detection 🚀

A Streamlit web app that predicts whether two Quora questions are duplicates using NLP and a trained ML model.  
Deployed on **Render** with CI/CD from GitHub.

---

## 🔹 Demo
👉 Live App: [https://quora-duplicate-questions.onrender.com](https://quora-duplicate-questions.onrender.com)

---

## 🔹 Features
- Preprocessing with **CountVectorizer** and **custom stopwords**
- Model trained with **scikit-learn**
- Simple **Streamlit UI** for question input
- Deployed with **Render Free Tier**

---

## 🔹 Project Structure
├── app.py # Streamlit app
├── model.pkl # Trained ML model
├── cv.pkl # CountVectorizer object
├── stopwords.pkl # Stopwords list
├── requirements.txt # Dependencies
├── runtime.txt # Python version (3.12.6 for Render)
└── README.md # Project docs


