🧠 🔹 TAYYOR — AgroRisk-AI README.md (FULL PROFESSIONAL VERSION)

📌 BU FAQAT KO‘CHIRILADI VA README.md’ga JOYLASHTIRILADI

# 🌾 AgroRisk-AI  
### AI-driven Credit Risk Scoring, Fraud Detection & Payment Risk Analytics Platform for Agrobank

AgroRisk-AI — bu Agrobank uchun yaratilgan sun’iy intellektga asoslangan risk baholash tizimi bo‘lib, kreditni qaytarmaslik ehtimolini (Default Risk), shubhali tranzaksiyalarni (Fraud) va kechikish xavfini (Late Payment Risk) aniqlab beradi.

Loyiha **klassik Machine Learning (XGBoost, CatBoost, Sklearn)** va **Anomaly Detection (Isolation Forest, LOF)** asosida qurilgan.

---

## 🚀 Platforma imkoniyatlari

### 🔵 1. **Credit Default Risk Scoring (XGBoost)**
- Mijozning kredit qaytarish-qaytarmaslik ehtimolini 0–1 ko‘rsatkichda qaytaradi  
- Feature Engineering + SHAP interpretatsiya  
- Model: `XGBoostClassifier`

### 🟣 2. **Fraud Transaction Detection (Anomaly Detection)**
- Shubhali tranzaksiyalarni aniqlash  
- Isolation Forest / Local Outlier Factor  
- Real-time scoring uchun API

### 🟢 3. **Late Payment Risk Predictor**
- Kim kredit to‘lovini kechiktirishi mumkinligini bashorat qiladi  
- Payment history, DPD, behavioral features asosida

### 🟠 4. **AI Dashboard**
- Streamlit orqali vizual panel  
- Risk ko‘rsatkichlari  
- Fraud heatmap  
- Approval/reject simulyatsiya

---

## 🏗 Texnik arxitektura



AgroRisk-AI
│
├── data/ # Demo datasets (CSV)
├── notebooks/ # Jupyter Notebooks (EDA, modeling)
├── models/ # Trained ML models (.pkl)
├── src/
│ ├── train.py # Model training pipeline
│ ├── predict.py # Prediction functions
│ ├── fraud_detector.py # Anomaly detection pipeline
│ ├── shap_explain.py # SHAP explainability visualizations
│ └── api.py # FastAPI backend
│
├── dashboard/
│ └── app.py # Streamlit UI
│
├── requirements.txt # Python dependencies
└── README.md # Project documentation


---

## 🧠 Model va texnologiyalar

- **Python 3.10+**  
- **Pandas, NumPy**  
- **Scikit-learn, XGBoost, CatBoost, LightGBM**  
- **Matplotlib, Seaborn, Plotly**  
- **SHAP (feature importance & interpretability)**  
- **FastAPI (REST API)**  
- **Streamlit (dashboard)**  
- **SQLite / CSV demo data**

---

## 📊 Metrikalar (Demo)

| Model | Accuracy | ROC-AUC | Precision | Recall |
|-------|----------|----------|-----------|--------|
| XGBoost (Default Risk) | 0.86 | 0.91 | 0.88 | 0.84 |
| Isolation Forest (Fraud) | – | – | – | 74% detection |
| Late Payment Risk | 0.78 | 0.83 | 0.79 | 0.76 |

*(Hackathon davomida real metrikalar bilan yangilanadi)*

---

## 🔌 API endpoints (Demo)



POST /predict_default
POST /predict_fraud
POST /predict_late
GET /shap_summary


---

## 👤 Muallif

**Xojimurod Xalimjonov**  
FinTech AI & Machine Learning Engineer  
Telegram: @Xojimurod_Xalimjonov  
GitHub: https://github.com/Xojimurod1

---

## 📜 License

MIT License  
data/.gitkeep

notebooks/.gitkeep

models/.gitkeep

src/train.py

src/predict.py

src/fraud_detector.py

src/shap_explain.py

src/api.py

dashboard/app.py

requirements.txt
