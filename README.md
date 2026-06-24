# Algerian Forest Fire Prediction

This project is a Flask web application for predicting forest fire area using a trained regression model and user-provided weather/fire condition inputs.

## Live Demo

- 🚀 Live demo: https://forest-fire-predictor.up.railway.app/predictdata

## Project Structure

- `application.py` - Flask application entry point.
- `models/` - contains serialized model artifacts:
  - `ridge_model.pkl` - trained Ridge regression model.
  - `scaler.pkl` - standard scaler used for feature scaling.
- `templates/` - HTML templates used by Flask:
  - `index.html` - main landing page.
  - `home.html` - prediction form and result page.
- `requirements.txt` - Python dependencies.
- `notebooks/` - project notebooks:
  - `2.0-EDA And FE Algerian Forest Fires.ipynb` - exploratory data analysis and feature engineering notebook.
  - `3.0-Model Training.ipynb` - model training notebook.

## Setup

1. Create and activate a virtual environment:

```bash
python -m venv venv
venv\Scripts\activate
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

## Run the App

Start the Flask application:

```bash
python application.py
```

Open your browser at `http://127.0.0.1:5000`.

## Usage

- Submit values for temperature, relative humidity, wind speed, rain, and fire danger indices.
- The app scales inputs and returns a predicted burned area value.

## Notes

- Ensure the `models/` folder contains the required pickle files.
- If using a different Python environment, adjust the activation command accordingly.
