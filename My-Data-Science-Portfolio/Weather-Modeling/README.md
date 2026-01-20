# Weather Analytics: Rain Prediction & Risk Regression
A dual-pipeline study using the "Rain in Australia" dataset to predict rainfall occurrence and environmental risk through classification and regression.

### 📈 Results & Metrics

#### 1. Classification (Rain Prediction)
Predicting whether it will rain tomorrow based on atmospheric pressure, humidity, and temperature.
* **Overall Accuracy:** 100.0%
* **Detailed Breakdown:**
    * **Class 0 (No Rain):** 100% Precision, 100% Recall.
    * **Class 1 (Rain):** 100% Precision, 100% Recall.
* **Top Model:** Random Forest Classifier.

#### 2. Regression (Risk & Intensity)
Predicting numerical weather metrics using a comparative model approach to determine the most accurate forecasting method.
* **Top Model:** Random Forest Regressor ($R^2$: 97.77%)
* **Model Performance Comparison:**
    * **Random Forest:** 97.77% $R^2$ Score
    * **Decision Tree:** 95.68% $R^2$ Score
    * **Linear SVR:** 95.39% $R^2$ Score
    * **Linear Regression:** 95.39% $R^2$ Score
    * **AdaBoost:** 4.77 Mean Squared Error (MSE)

### 🛠️ Technical Implementation
* **Dataset:** Historical "Rain in Australia" dataset containing daily weather observations from numerous Australian weather stations.
* **Architecture:** * **Classification Pipeline:** Focused on high-precision event detection using ensemble learning.
    * **Regression Suite:** Evaluated five distinct algorithms (Linear Regression, Decision Tree, SVR, Random Forest, and AdaBoost) to identify the best fit for non-linear weather variance.
* **Preprocessing:** * Advanced data cleaning and handling of missing meteorological values.
    * Feature scaling via `StandardScaler` to optimize distance-based estimators like SVR.
    * Label Encoding for categorical regional and station data.

### 🔍 Key Insights
The **Random Forest Regressor** significantly outperformed other models, achieving an $R^2$ of **97.77%**, proving that ensemble tree-based methods are highly effective at capturing the complex, non-linear relationships found in atmospheric data compared to standard linear models.
