# E-commerce Customer Spending Prediction

This project implements a Multiple Linear Regression model to predict the yearly amount spent by e-commerce customers based on their interaction with the company's app and website, as well as their membership duration.

##  Objective
The goal is to determine which factors most influence the yearly spending of customers. By analyzing the coefficients of the linear regression model, we can identify the most impactful drivers of revenue to help the company focus its marketing and development efforts.

##  Dataset
The dataset used is `Ecommerce Customers.csv`, which contains the following features for 500 customers:
- **Avg. Session Length**: Average time spent per session.
- **Time on App**: Total time spent on the mobile app.
- **Time on Website**: Total time spent on the website.
- **Length of Membership**: Duration of the customer's membership (in years).
- **Yearly Amount Spent**: The target variable we aim to predict.

##  Workflow
The analysis is performed in the `Linear-Stats.ipynb` notebook:

1. **Exploratory Data Analysis (EDA)**: 
   - Used `seaborn` and `matplotlib` to visualize relationships between features and the target variable.
   - Pairplots and Jointplots were used to identify strong linear correlations, specifically noting the strong relationship between `Length of Membership` and `Yearly Amount Spent`.
2. **Data Preprocessing**:
   - Split the data into training (70%) and testing (30%) sets.
3. **Model Training**:
   - Implemented a `LinearRegression` model from `scikit-learn`.
   - Fit the model to the training data using the four primary behavioral features.
4. **Evaluation**:
   - Evaluated the model using Mean Absolute Error (MAE), Mean Squared Error (MSE), and Root Mean Squared Error (RMSE).
   - Analyzed residuals to check for normality and model fit.

##  Key Findings
Based on the model coefficients:
- **Length of Membership** has the most significant impact on yearly spending.
- **Time on App** is also a strong predictor of spending.
- **Time on Website** has a minimal impact compared to the app.

##  Requirements
To run the analysis, you will need the following Python libraries:
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`

##  How to Run
1. Ensure you have the `Ecommerce Customers.csv` file in the project directory.
2. Open `Linear-Stats.ipynb` in a Jupyter environment.
3. Run all cells to see the analysis, visualizations, and model performance.
# E-commerce-Customer-Spending-Prediction
