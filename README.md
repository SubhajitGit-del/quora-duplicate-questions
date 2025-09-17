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

## 🔹 Setup (Local)

1. Clone repo:
   ```bash
   git clone https://github.com/<your-username>/quora-duplicate-questions.git
   cd quora-duplicate-questions

Create virtual environment:

2. python -m venv venv
# Activate
.\venv\Scripts\activate   # Windows
source venv/bin/activate  # Mac/Linux

3. Install requirements:

pip install --upgrade pip
pip install -r requirements.txt


4. Run app locally:

streamlit run app.py


Local URL: http://localhost:8501

🔹 Deployment (Render)

1. Push repo to GitHub (include .pkl model files).

2. Connect Render → New Web Service → GitHub repo.

3. Configure:

   Build Command

        pip install --upgrade pip setuptools wheel && pip install -r requirements.txt


   Start Command

        streamlit run app.py --server.port $PORT --server.enableCORS false


4. Add runtime.txt:

python-3.12.6


(Ensures compatibility with pandas, Pillow, scikit-learn.)

5. Deploy! 🎉

🔹 Learnings

        Always pin Python version (runtime.txt) to avoid runtime issues.

        Use dependency ranges (>=,<) instead of hard pins (==).

        Debug Render via Events → Logs.

        Test locally with a venv before deployment.
