🚗 Car Price Predictor

A machine learning project that predicts the selling price of a car based on its features such as brand, year, mileage, fuel type, and more.
Built with Python, scikit-learn, pandas, and Flask.

📌 Features

- End-to-end ML pipeline for regression.
- Data preprocessing (missing values, categorical encoding, scaling).
- Model training and evaluation (Linear Regression & alternatives).
- Saved trained model with preprocessing pipeline for deployment.
- Flask web app for user-friendly predictions.

📂 Project Structure

Car-Price-Predictor/
│
├── Application.py               # Flask app for deployment
├── LinearRegressionModel.pkl    # Trained model (saved with sklearn/joblib)
├── requirements.txt             # Dependencies with versions
├── static/                      # CSS/JS files for the web UI
├── templates/                   # HTML templates (Flask uses Jinja2)
├── data/                        # Dataset (CSV or Excel file)
└── notebook.ipynb               # Jupyter Notebook for EDA & model training

⚙️ Installation

1. Clone the repo
   git clone https://github.com/yourusername/Car-Price-Predictor.git
   cd Car-Price-Predictor

2. Create a virtual environment (recommended)
   python -m venv venv
   venv\Scripts\activate   # On Windows
   # or
   source venv/bin/activate   # On Mac/Linux

3. Install dependencies
   pip install -r requirements.txt

⚠️ Important: Use the same scikit-learn version used for model training (e.g., scikit-learn==1.5.1) to avoid pickle compatibility issues.

🚀 Usage

Train the model:
- Open notebook.ipynb in Jupyter and run the cells to:
  - Clean & preprocess the dataset.
  - Train the regression model.
  - Save it as LinearRegressionModel.pkl.

Run the Flask app:
- python Application.py
- Go to http://127.0.0.1:5000/ in your browser to use the predictor.

🛠️ Tech Stack

- Python 3.10+
- scikit-learn for machine learning
- pandas & numpy for data processing
- Flask for web deployment
- HTML/CSS for frontend

📊 Example Input / Output

Input:
- Brand: Hyundai
- Year: 2017
- Fuel: Petrol
- Mileage: 40,000 km

Predicted Price:
- ₹ 3.45 Lakhs

📌 Improvements (Future Work)

- Try advanced models (Random Forest, XGBoost, CatBoost).
- Deploy on cloud (Heroku, AWS, Render).
- Add a better frontend with React/Streamlit.
- Handle more datasets for generalization.
