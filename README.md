# Weather-Classification
🌤️ Weather Regression Model – Predicting Temperature from Weather Features
This project implements a machine learning pipeline to predict the temperature (Celsius) using real-world weather data. The pipeline includes outlier handling, feature selection, data visualization, and training multiple regression models (Random Forest, Linear Regression, SVM, etc.). The workflow is built using pandas, matplotlib, seaborn, and scikit-learn.

📂 Dataset
The dataset used is weatherHistory.csv and contains 96,453 rows of hourly weather observations. The features include humidity, wind speed, wind direction, visibility, and more. It must be placed in your local working directory or update the path in the notebook accordingly.

📁 Example structure:

project/
├── weatherHistory.csv
├── regression_weather.ipynb
🚀 Features & Workflow
✅ Step 1: Preprocessing
Loads weather data and drops duplicate entries

Removes irrelevant columns: Summary, Apparent Temperature, Daily Summary, etc.

Handles missing values by dropping nulls

Detects and removes outliers using IQR method

✅ Step 2: Feature Selection & Label Encoding
Retains only numeric features: Humidity, Wind Speed, Wind Bearing, Visibility

Encodes categorical features like Precip Type using LabelEncoder

✅ Step 3: Model Training & Evaluation
Splits dataset into train and test sets

Trains multiple models:

✅ Random Forest Regressor

✅ Logistic Regression (for classification evaluation)

✅ Support Vector Machine (SVM)

Evaluates models using:

Accuracy Score

Precision, Recall, F1 Score

Confusion Matrix

📦 Dependencies
Install the required Python libraries:

pip install numpy pandas matplotlib seaborn scikit-learn
🧠 How to Use
Download or clone this repository.

Place weatherHistory.csv in the root directory.

Open the notebook (regression_weather.ipynb) and run all cells.

Review model evaluation results and visualizations.

📊 Visualizations
📌 Confusion Matrix for classification models

📌 Heatmap of correlations

📌 3D plots of feature distributions

📌 PCA plots for dimensionality reduction (if included)

📝 Outputs
Trained regression and classification models

Model performance metrics (accuracy, F1, etc.)

Cleaned and preprocessed dataset (in memory)

Visual insights from weather features

