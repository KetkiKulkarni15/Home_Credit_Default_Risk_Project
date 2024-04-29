# Home_Credit_Default_Risk_Project
Repository for a predictive modeling project aimed at improving loan approvals for individuals with minimal credit history. Utilizes logistic regression and Recursive Feature Elimination (RFE) to predict loan repayment probabilities, enhancing financial inclusion efforts.
## Business Problem Statement
-Home Credit, a global financial institution, is dedicated to expanding financial access to customers who often find themselves excluded from the conventional banking system due to their insufficient credit histories. This demographic represents a significant portion of the global market, yet poses a unique challenge: assessing their creditworthiness accurately without traditional credit data, which increases the risk of defaults. High default rates can have serious repercussions, not only affecting the company's financial health but also its mission to foster financial inclusion responsibly.
-This project addresses this critical challenge by developing an advanced predictive model utilizing machine learning techniques. Leveraging a combination of traditional credit data and alternative data sources, such as telecommunications and transaction histories, the model aims to enhance the accuracy of predicting loan repayment probabilities. By improving how creditworthiness is assessed, Home Credit hopes to achieve a dual objective: extending more credit opportunities to those who are typically overlooked while managing risk more effectively. This balance is crucial for promoting financial inclusion without compromising on lending standards and ensuring that loans are both accessible and sustainable.
-The insights and tools generated from this project are intended to guide Home Credit in making informed lending decisions that support the financial empowerment of a broader customer base, aligning with ethical lending practices and the company's strategic goals

## Data Overview
This project utilizes a comprehensive dataset from Home Credit, which includes several types of information:
- **Application Data (`application_train/test.csv`)**: Applicant's basic details at the time of application.
- **Bureau Data (`bureau.csv`, `bureau_balance.csv`)**: Information on client's past loans with other financial institutions.
- **Previous Transactions(`previous_application.csv`, `POS_CASH_balance.csv`, `credit_card_balance.csv`, `installments_payments.csv`)**: Details on previous transactions and payment behaviors.

**Data preprocessing** involved handling missing values, encoding categorical features, and creating new features that better capture the underlying credit risk.

## Technologies and Tools Used for the project
- **Python** for all data processing and modeling.
- **Pandas** for data manipulation, **Matplotlib/Seaborn** for visualization, **Scikit-Learn** for machine learning, and **XGBoost** for applying ensemble techniques to enhance model performance.

## Methodological Approach
The analytical approach was structured as follows:
1. **Exploratory Data Analysis**: Identifying patterns, anomalies, and correlations within the data.
2. **Feature Engineering**: Constructing new variables to better predict outcomes.
3. **Model Development**:
   - **Logistic Regression** with and without data normalization.
   - **Recursive Feature Elimination (RFE)** to identify the most influential features.
4. **Model Evaluation**: Using metrics such as Accuracy, Precision, Recall, F1-Score, and ROC-AUC to assess each model's performance.

## Key Findings
- Normalized models demonstrated improved predictive performance over non-normalized approaches.
- RFE helped in pinpointing critical features, significantly optimizing the model's performance with an AUC-ROC of 0.625.

## Challenges Encountered and Resolutions
Dealing with imbalanced data and extensive missing values posed significant challenges. Techniques like synthetic data generation and advanced imputation methods were utilized to address these issues, enhancing model robustness and reliability.

## Conclusion and Next Steps
This project underscores the potential of machine learning to revolutionize financial inclusivity. Future directions include exploring more complex algorithms and incorporating real-time data feeds to continuously refine the predictive accuracy.

   


