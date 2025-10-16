House Price Prediction – Machine Learning Project
📌 Overview

This project predicts the selling price of a house based on key features such as area, number of bedrooms, bathrooms, location, and age. It uses supervised machine learning techniques (like Linear Regression and Gradient Boosting) to build a predictive model from historical housing data.

🎯 Aim

To develop an ML model that estimates house prices accurately, helping users make better real-estate decisions.

🚀 Features

📊 Data Analysis & Visualization – Understand how different features affect price

🤖 Model Training – Train multiple ML models (Linear Regression, Ridge, Random Forest, Gradient Boosting)

📈 Best Model Selection – Automatically picks the model with lowest RMSE

🔍 CLI Prediction Tool – Predict house price directly from the terminal

🌐 Web App (Flask) – Interactive web interface to input house details and view predictions

📂 Custom Dataset Support – Easily replace with your own CSV data

🛠️ Tech Stack

Language: Python 3.12+

Libraries: pandas, numpy, scikit-learn, Flask, joblib

Frontend: HTML5, CSS3, Bootstrap

Tools: Jupyter/VS Code, Git, GitHub

📊 Dataset

Default: housing_data.csv (synthetic sample provided)

Format:

Area	Bedrooms	Bathrooms	Location	Age	Price
1200	3	2	Suburb	10	8500000
2000	4	3	CityCenter	5	14000000

📁 You can replace this with a real dataset (same column names) for real-world predictions.

⚙️ Installation & Setup

Clone the repository

git clone https://github.com/your-username/house-price-ml.git
cd house-price-ml


Create and activate a virtual environment

python -m venv .venv
.\.venv\Scripts\Activate.ps1    # Windows
source .venv/bin/activate       # macOS/Linux


Install dependencies

pip install -r requirements.txt


Train the model

python train.py --data housing_data.csv --output best_model.joblib


Test predictions (CLI)

python predict_cli.py --area 1500 --bedrooms 3 --bathrooms 2 --location Suburb --age 10


Run the web application

python app.py


Visit 👉 http://127.0.0.1:5000
 in your browser.

📈 Results

Example output after training:

Model Performance on Test Set:
- LinearRegression   RMSE=56,032.06 | R2=0.5994
- Ridge              RMSE=56,071.98 | R2=0.5989
- GradientBoosting   RMSE=58,055.62 | R2=0.5700
- RandomForest       RMSE=62,948.39 | R2=0.4944

Best model: LinearRegression with RMSE=56,032.06

📂 Project Structure
├── app.py                 # Flask web application
├── train.py              # Model training script
├── predict_cli.py        # CLI-based prediction tool
├── housing_data.csv      # Sample dataset
├── best_model.joblib     # Saved model (after training)
├── requirements.txt      # Dependencies
└── README.md             # Project documentation

📊 Future Improvements

Add dark/light mode toggle 🌙

Deploy the app using Streamlit or Docker ☁️

Add feature importance visualization 📈

Use real-world data from Kaggle 🏘️
