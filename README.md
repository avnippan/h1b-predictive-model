# H1-B Visa Approval Prediction

## Overview

This project explores the prediction of H1-B visa approval outcomes using machine learning techniques. The goal is to build a model that can help employers and applicants better anticipate visa outcomes, enabling more informed decision-making and strategic planning.

The H1-B visa program allows US employers to temporarily employ foreign workers in specialty occupations.  Due to high demand and limited availability, the approval process is highly competitive. Predictive modeling offers a data-driven approach to understanding and anticipating these outcomes.

## Files

*   `h1_b_approval.ipynb`: Jupyter Notebook containing the data analysis, preprocessing, model building, and evaluation.
*   `ITCS-5154-Final-Presentation-Updated.pdf`: Presentation deck summarizing the project's background, methodology, and findings.

## Problem Statement

Predict the likelihood of H1-B Visa approval based on available data. This is framed as a binary classification problem (Approved vs. Not Approved).

## Motivation

*   **High Demand, Low Approval Rate:** The H1-B visa process is highly competitive. In 2019, only 42% of applicants were approved.
*   **Informed Decision-Making:** Predictive models can help applicants and employers make informed decisions.
*   **Efficiency and Transparency:** Machine learning can improve the efficiency and transparency of the visa adjudication process.

## Dataset

The project utilizes the H-1B Visa Petitions dataset (2011-2016). This dataset contains approximately 3 million records (obtained from Kaggle; originally used in [Kumar and Naresh's paper]).

### Key Features:

*   `EMPLOYER_NAME`: Name of the employer submitting the application.
*   `SOC_NAME`: Occupational name associated with the SOC code.
*   `JOB_TITLE`: Title of the job.
*   `FULL_TIME_POSITION`: Indicates whether the position is full-time (Y) or part-time (N).
*   `PREVAILING_WAGE`: The average wage paid to employees with similar qualifications in the intended area of employment.
*   `YEAR`: The year of filing the petition.
*   `WORKSITE_CITY_FULL`: City of the applicant’s job.
*   `WORKSITE_STATE_FULL`: State of applicant’s job.

## Implementation

The `h1_b_approval.ipynb` notebook details the full implementation, including:

1.  **Data Preprocessing:**
    *   Handling missing values.
    *   Dropping unnecessary or redundant columns.
    *   One-hot encoding of categorical variables.
    *   Train-test split (80-20).
    *   Standard scaling of features.
2.  **Modeling:**
    *   **Logistic Regression:**  Used for binary classification.
    *   **Random Forest Classifier:** An ensemble method to improve prediction accuracy.

## Challenges

*   **Imbalanced Dataset:** The number of approved petitions significantly outweighs the number of denied petitions.
*   **Data Preprocessing:**  Requires careful handling of missing values and categorical features.
*   **Model Selection:** Choosing the right model to handle the data imbalance and deliver reliable results.

## Related Work

This project builds upon existing research in H1-B visa approval prediction, including:

*   Kumar and Naresh used Gaussian Naïve Bayes, Random Forest, and XGBoost.
*   Santhoshi et al. (2022) found the H-1B approval rate in 2019 was approximately 42%.
*   Dombe, Rewale, & Swain (2022) used Logistic Regression, Decision Tree, Random Forest, and KNN.

## Usage

To run the analysis:

1.  Ensure you have Jupyter Notebook installed (`pip install notebook`).
2.  Install the necessary Python libraries (e.g., pandas, scikit-learn, etc.).  A `requirements.txt` file will be added to the repository soon.
3.  Open `h1_b_approval.ipynb` in Jupyter Notebook.
4.  Run the cells sequentially to reproduce the analysis.
