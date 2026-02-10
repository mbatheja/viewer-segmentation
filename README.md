# Viewer Churn Prediction and Clustering

This project focuses on analyzing viewer data to predict churn and extract actionable insights using machine learning. The analysis explores demographics, subscription details, and service usage to identify key drivers of customer retention.

## Features
* **Data Preprocessing:** Cleaning and preparing 6,588 viewer records for modeling.
* **Churn Prediction:** Comparison of Logistic Regression and Random Forest models to identify at-risk customers.
* **Clustering:** Segmenting viewers using KMeans and PCA for behavioral analysis.
* **Feature Importance:** Determining which specific customer attributes (e.g., tenure, monthly charges) most influence retention.

## Key Findings & Model Performance

### Churn Drivers (Feature Importance)
The Random Forest model identified the following features as the most significant predictors of viewer churn (ranked by importance):
1. **Tenure in Months:** Longer-term customers are significantly less likely to churn.
2. **Monthly Charge:** Higher costs are strongly correlated with a higher probability of cancellation.
3. **Total Revenue:** Total spend over time serves as a key indicator of long-term loyalty.
4. **Number of Referrals:** Viewers who refer others are more likely to stay with the service.
5. **Age:** Specific age demographics show varying levels of stability.

### Model Evaluation
The predictive models were evaluated using several metrics to ensure accuracy in identifying potential churners:
* **Accuracy:** Overall correctness of the model's predictions.
* **Recall:** The ability of the model to find all actual churners (crucial for retention efforts).
* **Precision:** The accuracy of the "churn" predictions made by the model.
* **ROC-AUC:** Measures the model's ability to distinguish between "Stayed" and "Churned" statuses.


## Clustering Insights
Using KMeans clustering, the viewer base was divided into segments to better understand usage patterns:
* **High-Value Loyalists:** Long tenure, high referrals, and low churn.
* **At-Risk Newcomers:** Short tenure and high monthly charges.
* **Budget Streamers:** Lower monthly charges but consistent engagement with streaming services.

## Setup Instructions

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Run the Notebook:**
    Launch Jupyter Lab or Notebook and open `viewer_churn.ipynb`.
