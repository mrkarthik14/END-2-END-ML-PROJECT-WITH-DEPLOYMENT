# End-to-End Machine Learning Project with Deployment

**Author:** Karthik M (mrkarthik14)

---

## 📋 Project Overview

This is a comprehensive **end-to-end Machine Learning project** that demonstrates the complete workflow from data exploration to model training and deployment. The project focuses on predicting forest fire intensity using environmental factors, deployed as a web application using Flask.

### Key Features

- **Data Processing & Analysis** - Complete exploratory data analysis with cleaned datasets
- **Model Training** - Ridge Regression model trained on Algerian forest fire datasets
- **Feature Scaling** - StandardScaler for data normalization
- **Web Deployment** - Flask-based web application for real-time predictions
- **Interactive UI** - User-friendly interface to input parameters and get predictions
- **Production Ready** - Serialized models for easy deployment

---

## 🎯 Objective

Predict the intensity of forest fires based on environmental and weather parameters including:
- Temperature
- Relative Humidity (RH)
- Wind Speed (Ws)
- Rainfall
- FFMC (Fine Fuel Moisture Code)
- DMC (Duff Moisture Code)
- ISI (Initial Spread Index)
- Forest Classes
- Region

---

## 📁 Project Structure

```
End-2-End-ML-Project-with-Deployment/
├── README.md                                       # Project documentation
├── requirements.txt                                # Python dependencies
├── application.py                                  # Flask web application
├── data/
│   ├── Algerian_forest_fires_dataset.csv          # Original dataset
│   ├── Algerian_forest_fires_dataset_UPDATE.csv   # Updated dataset
│   └── Algerian_forest_fires_dataset_cleaned_data.csv  # Cleaned dataset
├── models/
│   ├── ridge.pkl                                  # Trained Ridge Regression model
│   └── scaler.pkl                                 # Fitted StandardScaler
├── notebooks/
│   ├── Model_Training.ipynb                       # Main model training notebook
│   └── Ridge_Lasso_Regression.ipynb              # Regression analysis notebook
└── templates/
    ├── index.html                                 # Home page
    └── home.html                                  # Prediction form page
```

---

## 🛠️ Installation & Setup

### Prerequisites
- Python 3.7 or higher
- pip (Python package manager)

### Step 1: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 2: Verify Model Files

Ensure the following pickle files exist in the models/ directory:
- idge.pkl - Pre-trained Ridge Regression model
- scaler.pkl - Fitted StandardScaler for feature normalization

### Step 3: Run the Application

```bash
python application.py
```

The application will start on http://localhost:5000

---

## 📦 Dependencies

| Package | Purpose |
|---------|---------|
| Flask | Web framework for building the application |
| NumPy | Numerical computations |
| Pandas | Data manipulation and analysis |
| Matplotlib | Data visualization |
| Scikit-learn | Machine learning algorithms and preprocessing |

---

## 🚀 Usage

### Web Interface

1. Open your browser and navigate to http://localhost:5000
2. Click on the prediction form link
3. Enter the environmental parameters:
   - Temperature (°C)
   - Relative Humidity (%)
   - Wind Speed (km/h)
   - Rainfall (mm)
   - FFMC Index
   - DMC Index
   - ISI Index
   - Forest Classes
   - Region
4. Click "Predict" to get the forest fire intensity prediction

### API Endpoint

**POST** /predictdata

Accepts form data with the following parameters and returns the predicted fire intensity.

---

## 📊 Model Details

- **Algorithm**: Ridge Regression
- **Features**: 9 environmental and meteorological parameters
- **Data Source**: Algerian Forest Fires Dataset
- **Preprocessing**: StandardScaler normalization
- **Model Format**: Pickle (.pkl) for easy serialization

---

## 📈 Dataset Information

The project uses the **Algerian Forest Fires Dataset** which contains:
- 244 instances from the Sidi-Bel-Abbès region (June 2021 - September 2021)
- 122 instances from the Mont de Marson region (June 2021 - September 2021)
- 9 input features related to weather and fuel conditions
- 1 output variable representing fire intensity

---

## 🔧 Model Training

To retrain the model:

1. Open 
otebooks/Model_Training.ipynb in Jupyter Notebook
2. Follow the steps for:
   - Data loading and exploration
   - Feature engineering
   - Model training
   - Model evaluation
   - Model serialization

```bash
jupyter notebook notebooks/Model_Training.ipynb
```

---

## 📝 Key Files

| File | Description |
|------|-------------|
| pplication.py | Main Flask application with routes for home page and predictions |
| Model_Training.ipynb | Complete ML pipeline with data analysis and model training |
| home.html | Prediction form interface |
| index.html | Landing page |

---

## 🎓 Learning Outcomes

This project demonstrates:
- End-to-end machine learning workflow
- Data preprocessing and feature scaling
- Model training and evaluation
- Model serialization and deployment
- Web application development with Flask
- Integration of ML models in production environments

---

## 📧 Contact & Support

For questions or support regarding this project, please reach out to the project author.

---

## 📄 License

This project is open source and available for educational and research purposes.

---

**Last Updated**: May 2026  
**Version**: 1.0
