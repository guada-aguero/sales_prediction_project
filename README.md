# Sales Prediction Project

## Overview
This project involves predicting sales for various stores based on historical data. We have applied several machine learning models, including Decision Trees, Random Forests, and Gradient Boosting, to build a robust predictive model.

## Features
- **Date Transformation**: Convert dates to ordinal numbers for easier processing by the models.
- **State Holiday Encoding**: Map state holidays to numerical values.
- **Data Filtering**: Exclude data where stores are closed as sales are always 0 in those cases.

## Model
The final model used in this project is a Gradient Boosting model (`gboost_model.pkl`).

### Download the Model
The trained model `gboost_model.pkl` is too large to be stored in this repository. You can download it from the following link:

[Download gboost_model.pkl](https://github.com/guada-aguero/sales_prediction_project/releases/tag/v1.0)

## How to Use
1. **Clone the repository**:
   ```bash
   git clone https://github.com/guada-aguero/sales_prediction_project.git
   cd sales_prediction_project

2. **Install dependencies**:
   Make sure you have all the necessary Python packages installed. You can do this using `pip` and the `requirements.txt` file:

   ```bash
   pip install -r requirements.txt

3. **Run the Notebook**:
   Open the Jupyter Notebook `iron-kaggle.ipynb` to see the full implementation and explore the results.

4. **Load the Model**:
   Download the `gboost_model.pkl` file from the Releases section and use it in your own predictions.

   ```python
   import pickle

   # Load the model from the file
   with open('gboost_model.pkl', 'rb') as file:
       model = pickle.load(file)

## Project Structure

- `iron-kaggle.ipynb`: Jupyter Notebook with the full analysis and model training process.
- `sales.csv`: Dataset used for training the models.
- `validation_for_students.csv`: Validation dataset for testing the models.
- `gboost_model.pkl`: The trained Gradient Boosting model (available in the Releases section).

## Requirements

- Python 3.7+
- Pandas
- NumPy
- Scikit-learn
- XGBoost
