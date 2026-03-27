# 🌱 Soil Fertility Predictor

> AI-Augmented Soil Fertility Index Generation 
> Using Temporal and Visual Deep Learning 
> Pipelines Optimization

![Python](https://img.shields.io/badge/Python-3.8-blue)
![Flask](https://img.shields.io/badge/Flask-2.x-green)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)
![MySQL](https://img.shields.io/badge/MySQL-8.x-blue)

## 📌 About
A deep learning web application that predicts 
soil fertility by combining LSTM-based soil 
parameter analysis with MobileNetV2-based 
leaf color classification, delivering a unified 
Soil Fertility Score (SFS) with crop, fertilizer 
and pesticide recommendations.

## 👨‍💻 Author
**Shabeeb Mohammed Sakir P**

[![GitHub](https://img.shields.io/badge/GitHub-Shabeeb--Mohammed--Sakir--P-black?logo=github)](https://github.com/Shabeeb-Mohammed-Sakir-P)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Shabeeb--Mohammed--Sakir-blue?logo=linkedin)](https://www.linkedin.com/in/shabeeb-mohammed-sakir)
[![Email](https://img.shields.io/badge/Email-sshabeebmohammedsakir%40gmail.com-red?logo=gmail)](mailto:sshabeebmohammedsakir@gmail.com)


## 🧠 Models
| Model | Purpose | Accuracy |
|-------|---------|----------|
| LSTM | Soil fertility classification | 95% |
| MobileNetV2 | Leaf Color Classification (LCC) | ~90% |
| Weighted Fusion | 60% soil + 40% leaf = SFS | 0–100 |

## 🌐 Tech Stack
- **Backend:** Python 3.8, Flask 2.x
- **ML/DL:** TensorFlow, Keras, OpenCV
- **Database:** MySQL 8.x
- **Frontend:** HTML5, CSS3, Jinja2

## 👥 User Roles
| Role | Access |
|------|--------|
| 🌾 Farmer | Submit soil data, view predictions |
| 🔬 Geologist | Extended form with location data |
| 🛡️ Admin | Monitor all predictions and users |

## ⚙️ Installation

### 1. Clone the repository
```bash
git clone https://github.com/Shabeeb-Mohammed-Sakir-P/soil-fertility-predictor.git
cd soil-fertility-predictor
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Setup MySQL Database
```sql
CREATE DATABASE soil_fertility_db;
```
Then run `database/schema.sql`

### 4. Add trained models
Place these in the `models/` folder:
- `lstm_model.h5`
- `efficientnet_model.h5`
- `scaler.pkl`

### 5. Run the application
```bash
python app/app.py
```

## 📁 Project Structure
```
soil-fertility-predictor/
├── app/
│   ├── app.py
│   └── templates/
│       ├── login.html
│       ├── register.html
│       ├── farmer_dashboard.html
│       ├── geologist_dashboard.html
│       ├── admin_dashboard.html
│       └── result.html
├── models/
│   └── (place .h5 and .pkl files here)
├── data/
│   └── (place dataset files here)
├── static/
│   └── uploads/
├── database/
│   └── schema.sql
├── requirements.txt
└── .gitignore
```

## 🔮 Future Enhancements
- 📡 IoT sensor integration
- 📱 Mobile application (Android/iOS)
- 🛰️ Satellite imagery fusion
- 🌍 Multilingual support
- 🔍 Explainability (SHAP values)

## 📊 SFS Score Interpretation
| Score Range | Fertility Level | Action |
|-------------|----------------|--------|
| 10 – 35% | 🔴 Low | Urgent soil treatment needed |
| 40 – 65% | 🟡 Medium | Balanced fertilization recommended |
| 70 – 95% | 🟢 High | Minimal intervention needed |


