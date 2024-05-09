 Singapore_Resale_Flat-prices_prediction

 
## Overview
This Streamlit web application predicts house prices using machine learning. It utilizes input features like town, flat type, storey range, floor area, and more to estimate prices.

## Usage
1. **Setup Environment**
   Ensure Python is installed on your machine. Install all required libraries with:
   ```
   pip install -r requirements.txt
   ```

2. **Run the App**
   Launch the Streamlit app using:
   ```
   streamlit run app.py
   ```

3. **Input Features**
   Interact with the app via sidebar input widgets. Select or enter values for each feature.

4. **Predict**
   Click "Predict" to receive the house price estimate.

## Files
- `app.py`: Contains the Streamlit application code.
- `requirements.txt`: Lists the dependencies required for the app.

## Model
The app uses a trained machine learning model (`house_price_model.pkl`) for predictions.

## Technologies Used
- **Streamlit**: An open-source framework for ML and Data Science in Python.
- **NumPy**: Essential for scientific computing.
- **Pickle**: For serializing and deserializing Python objects.

## Note
- The app is for demonstration and may not reflect actual house prices.
- Predictions are based on historical data and should not be used for real transactions.

## Data Workflow
1. **Data Preparation**
   - Concatenates CSV files into a DataFrame.
   - Drops missing values and extracts unique town names.
   - Retrieves and combines location data for addresses.

2. **Data Analysis**
   - Calculates distances to MRT stations and the CBD.
   - Merges coordinate data with flat data.

3. **Data Preprocessing**
   - Imputes missing values and computes median storey ranges.
   - Removes outliers.

4. **Exploratory Data Analysis**
   - Visualizes feature distributions and correlations.

5. **Model Building**
   - Splits data, defines regression models, and evaluates them.

6. **Streamlit Application**
   - Sets up the app with navigation and prediction functionality.

7. **Saving the Model**
   - Saves the model and scaler for future use.

The script encompasses data preprocessing, analysis, model building, and deployment for predicting resale flat prices in Singapore.
```
