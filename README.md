
# 🏥 Health Insurance Cost Predictor

A machine learning-powered web application that predicts health insurance premiums based on individual characteristics and health factors.

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Streamlit](https://img.shields.io/badge/Streamlit-1.28+-red.svg)
![ML](https://img.shields.io/badge/Machine%20Learning-Regression-green.svg)

## 📋 Overview

This project uses machine learning algorithms to predict health insurance costs based on various demographic, lifestyle, and health-related factors. The application provides an intuitive interface for users to input their details and receive instant premium predictions.

## 🎯 Features

- **Interactive UI**: Clean, organized 4x3 grid layout with dark theme
- **Real-time Predictions**: Instant insurance cost estimates via ML model
- **Comprehensive Input Fields**: 12 different health and demographic parameters
- **User-friendly Controls**: Mix of number inputs and dropdown selectors
- **Responsive Design**: Built with Streamlit for seamless user experience

## 🚀 Demo

Visit the live application: [Premium Health Insurance Cost Predictor](https://premium-insurance-prediction-ml-project.streamlit.app)

## 📊 Dataset & Features

### Input Features
- **Age**: 18-100 years
- **Number of Dependants**: 0-20 dependents
- **Income in Lakhs**: Annual income (0-200 lakhs)
- **Genetical Risk**: Risk score 0-5 based on genetic factors
- **Insurance Plan**: Bronze, Silver, or Gold tier
- **Employment Status**: Salaried, Self-Employed, Freelancer
- **Gender**: Male or Female
- **Marital Status**: Married or Unmarried
- **BMI Category**: Normal, Overweight, Underweight, Obesity
- **Smoking Status**: No Smoking, Regular, Occasional
- **Region**: Northeast, Northwest, Southeast, Southwest
- **Medical History**: 
  - No Disease
  - Diabetes
  - High blood pressure
  - Diabetes & High blood pressure
  - Thyroid
  - Heart disease
  - High blood pressure & Heart disease
  - Diabetes & Thyroid
  - Diabetes & Heart disease

## 🛠️ Technology Stack

- **Frontend**: Streamlit
- **Backend**: Python
- **ML Libraries**: 
  - Scikit-learn (Model Training & Prediction)
  - Pandas (Data Manipulation)
  - NumPy (Numerical Computing)
- **Visualization**: Matplotlib, Seaborn (for EDA)
- **Model Persistence**: Pickle/Joblib

## 📁 Project Structure

```
healthcare-premium-prediction/
│
├── artifacts/                      # Trained models and preprocessors
│   ├── model_young.joblib         # ML model for age <= 25
│   ├── model_rest.joblib          # ML model for age > 25
│   ├── scaler_young.joblib        # Scaler for young age group
│   └── scaler_rest.joblib         # Scaler for older age group
│
├── main.py                         # Main Streamlit application
├── prediction_helper.py            # Prediction utility functions
├── requirements.txt                # Python dependencies
├── README.md                       # Project documentation
├── LICENSE                         # Apache-2.0 License
└── .gitignore                      # Git ignore rules
```

## 🔧 Installation & Setup

### Prerequisites
- Python 3.10 or higher
- pip package manager

### Local Setup

1. **Clone the repository**
```bash
git clone https://github.com/thanusree2630/healthcare-premium-prediction.git
cd healthcare-premium-prediction
```

2. **Create a virtual environment**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Run the application**
```bash
streamlit run main.py
```

5. **Access the app**
Open your browser and navigate to `http://localhost:8501`

## 📦 Requirements

```txt
streamlit>=1.28.0
pandas>=2.0.0
numpy>=1.24.0
scikit-learn>=1.3.0
matplotlib>=3.7.0
seaborn>=0.12.0
joblib>=1.3.0
```

## 🧪 Model Development Process

### 1. Exploratory Data Analysis (EDA)
- Data distribution analysis
- Correlation studies
- Outlier detection
- Missing value handling
- Feature importance analysis

### 2. Feature Engineering
- Categorical encoding (One-Hot/Label Encoding)
- Numerical feature scaling
- Feature interaction creation
- Dimensionality reduction (if applicable)

### 3. Model Training
- Algorithm selection (Linear Regression, Random Forest, XGBoost, etc.)
- Cross-validation
- Hyperparameter tuning
- Model evaluation metrics (RMSE, MAE, R²)
- Model persistence

### 4. Model Performance Metrics
- **R² Score** 
- **RMSE**
- **MAE**

## 📈 Usage

1. Open the application in your browser
2. Fill in all required fields in the 4x3 grid layout:
   
   **Row 1:** Age, Number of Dependants, Income in Lakhs
   
   **Row 2:** Genetical Risk, Insurance Plan, Employment Status
   
   **Row 3:** Gender, Marital Status, BMI Category
   
   **Row 4:** Smoking Status, Region, Medical History

3. Click the "Predict" button
4. View your predicted insurance cost displayed as a success message

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Create a Pull Request

## 📝 License

This project is licensed under the Apache-2.0 License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Thanusree**
- GitHub: [@thanusree2630](https://github.com/thanusree2630)
- Repository: [healthcare-premium-prediction](https://github.com/thanusree2630/healthcare-premium-prediction)

## 📞 Support

If you encounter any issues or have questions, please:
- Open an issue on GitHub
- Contact me via email

## 🔮 Future Enhancements

- [ ] Add more ML algorithms comparison
- [ ] Implement SHAP values for model interpretability
- [ ] Add data visualization dashboard
- [ ] Include policy recommendation system
- [ ] Multi-language support
- [ ] Mobile-responsive design improvements
- [ ] API endpoint for programmatic access

---

⭐ If you find this project helpful, please consider giving it a star!
### Screenshots

#### Application Interface
![App Interface]([images/app_interface.png](https://github.com/thanusree2630/healthcare-premium-prediction/blob/main/Screenshot%202025-10-22%20003047.png))

#### Prediction Results
![Prediction Results](images/prediction_results.png)

