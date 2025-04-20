# 🚗 Used Car Price Prediction App

A machine learning-powered web application built with **Streamlit** that predicts the price of used cars in Malaysia. The app uses a trained **XGBoost** model along with a data preprocessing pipeline that includes scaling, encoding, and dimensionality reduction (TruncatedSVD).

## 🔍 Features

- Predict car prices based on user-selected specifications
- Dynamic dropdowns for brand, model, and variant based on sample dataset
- Auto-classification of car type as **Luxury** or **Regular**
- Clean and interactive Streamlit interface
- Built using preprocessed and dimensionally-reduced data for fast prediction

## 📁 Project Structure

car-price-prediction-app/ ├── app.py # Streamlit app ├── pipeline_xgb.pkl # Preprocessing pipeline (encoding, scaling, SVD) ├── model_xgb.pkl # Trained XGBoost model ├── requirements.txt # Required Python packages ├── README.md # Project overview └── data/ └── sample_data.csv # Sample data used for dropdown options


## 🧠 Model Info

- **Model**: XGBoost Regressor
- **Preprocessing**:
  - One-Hot Encoding for categorical variables
  - Standard Scaling for numeric variables
  - Dimensionality reduction using TruncatedSVD with 300 components
  - Car Type (Luxury vs Regular) derived based on brand

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/car-price-prediction-app.git
cd car-price-prediction-app

### 2. Install Requirements
pip install -r requirements.txt

### 3. Run the Streamlit App
streamlit run app.py

## 📝 Notes
The model expects inputs to match the format and features used during training.

Ensure all necessary .pkl files are available in the root directory before running the app.

## 📬 Contact
If you find this useful or have suggestions for improvement, feel free to open an issue or reach out!
