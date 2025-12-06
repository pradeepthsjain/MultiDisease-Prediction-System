# Multi-Disease Prediction System

A comprehensive machine learning-based web application that predicts multiple diseases using various patient health parameters. This system leverages trained ML models to provide predictions for 8 different diseases through an interactive Streamlit interface.

## 📋 Project Overview

This Multi-Disease Prediction System is designed to assist in early disease detection by analyzing patient symptoms and health metrics. The application uses pre-trained machine learning models to predict the likelihood of various diseases, providing a user-friendly interface for healthcare assessment.

### Supported Disease Predictions

1. **General Disease Prediction** - Based on symptoms analysis
2. **Diabetes** - Glucose levels, BMI, age, and other factors
3. **Heart Disease** - Cardiovascular health parameters
4. **Parkinson's Disease** - Voice and motor function metrics
5. **Liver Disease** - Liver function test parameters
6. **Hepatitis C** - Liver enzyme and protein levels
7. **Lung Cancer** - Smoking history and symptoms
8. **Chronic Kidney Disease** - Kidney function indicators
9. **Breast Cancer** - Tumor characteristics

## 🛠️ Technologies Used

- **Python 3.10.11**
- **Streamlit** - Web application framework
- **Scikit-learn** - Machine learning models
- **Pandas & NumPy** - Data manipulation
- **Plotly & Matplotlib** - Data visualization
- **Joblib** - Model persistence

## 📁 Project Structure

```
Multi-Disease-Prediction-main/
├── Frontend/
│   ├── app.py                    # Main Streamlit application
│   ├── code/
│   │   ├── DiseaseModel.py      # Disease prediction model class
│   │   ├── helper.py            # Helper functions
│   │   └── train.py             # Model training scripts
│   ├── models/                   # Pre-trained ML models (.sav files)
│   ├── data/                     # Disease datasets and descriptions
│   └── 2022/                     # Training and testing datasets
├── Datasets/                     # Raw datasets for various diseases
│   └── Code/                     # Jupyter notebooks for model training
├── models/                       # Saved ML models
├── requirements.txt              # Python dependencies
└── README.md                     # Project documentation
```

## 🚀 Setup Instructions

Follow these steps to set up and run the application on your local machine:

### 1. Create Conda Environment

Open your terminal/command prompt and create a new conda environment with Python 3.10.11:

```bash
conda create -n disease python=3.10.11 -y
```

### 2. Activate the Environment

Activate the newly created conda environment:

```bash
conda activate disease
```

### 3. Install Dependencies

Install all required Python packages using pip:

```bash
pip install -r requirements.txt
```

### 4. Navigate to Frontend Directory

Change to the Frontend directory where the main application is located:

```bash
cd Frontend
```

### 5. Run the Application

Launch the Streamlit application:

```bash
streamlit run app.py
```

The application will automatically open in your default web browser at `http://localhost:8501`

## 💡 How to Use

1. **Select Disease Type**: Use the sidebar menu to choose which disease prediction you want to perform
2. **Enter Parameters**: Input the required health parameters and symptoms based on the selected disease
3. **Get Prediction**: Click the prediction button to receive the analysis
4. **View Results**: The system will display the prediction result along with relevant visualizations

## 📊 Features

- **Multiple Disease Detection**: Single platform for 8+ disease predictions
- **Interactive UI**: User-friendly Streamlit interface with option menus
- **Data Visualization**: Plotly and Matplotlib charts for better insights
- **Pre-trained Models**: Optimized machine learning models for accurate predictions
- **Real-time Predictions**: Instant results based on input parameters
- **Symptom-based Analysis**: Intelligent symptom mapping for disease prediction

## 🔬 Model Information

The system uses various machine learning algorithms including:
- Decision Trees
- Random Forest
- Support Vector Machines (SVM)
- XGBoost
- Logistic Regression

All models are pre-trained on medical datasets and saved in `.sav` format for efficient loading and prediction.

## 📝 Dataset Sources

The project includes multiple datasets for different diseases:
- Diabetes Dataset
- Heart Disease Dataset
- Parkinson's Disease Dataset
- Liver Disease Dataset
- Hepatitis C Dataset
- Lung Cancer Dataset
- Chronic Kidney Disease Dataset
- Breast Cancer Dataset

## ⚠️ Disclaimer

**Important**: This application is intended for educational and research purposes only. It should NOT be used as a substitute for professional medical advice, diagnosis, or treatment. Always consult with qualified healthcare professionals for medical concerns.

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests
- Improve documentation

## 📄 License

This project is available for educational and research purposes.

## 👥 Contact

For questions or feedback regarding this project, please open an issue in the repository.

---

**Note**: Make sure you have all the required model files in the `Frontend/models/` directory before running the application. The models should include:
- `diabetes_model.sav`
- `heart_disease_model.sav`
- `parkinsons_model.sav`
- `lung_cancer_model.sav`
- `breast_cancer.sav`
- `chronic_model.sav`
- `hepititisc_model.sav`
- `liver_model.sav`
