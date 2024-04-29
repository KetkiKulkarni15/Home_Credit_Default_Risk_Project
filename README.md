# Home_Credit_Default_Risk_Project
Repository for a predictive modeling project aimed at improving loan approvals for individuals with minimal credit history. Utilizes logistic regression and Recursive Feature Elimination (RFE) to predict loan repayment probabilities, enhancing financial inclusion efforts.

## Summary of Business Problem
Home Credit is a global financial company that wants to offer loans to people who are usually not served by traditional banks because they don't have enough credit history. This group represents a large market opportunity but assessing their ability to pay back loans is challenging without standard credit information. This situation increases the chance of loan defaults, which could negatively impact the company’s finances and its mission to provide fair financial access.

## Project Objective
The goal of this project is to create a sophisticated predictive model using machine learning to better predict if loans will be paid back. The model will use a mix of usual credit data and other information sources like phone and transaction data to improve decision-making on who gets a loan. This approach aims to safely extend more loans to those often overlooked, supporting Home Credit's commitment to financial inclusion. This project will help Home Credit make smarter lending decisions that fit with their ethical standards and business objectives.

## Data Overview
This project utilizes a comprehensive dataset from Home Credit, which includes several types of information:
- **Application Data (`application_train/test.csv`)**: Applicant's basic details at the time of application.
- **Bureau Data (`bureau.csv`, `bureau_balance.csv`)**: Information on client's past loans with other financial institutions.
- **Previous Transactions(`previous_application.csv`, `POS_CASH_balance.csv`, `credit_card_balance.csv`, `installments_payments.csv`)**: Details on previous transactions and payment behaviors.

**Data preprocessing** involved handling missing values, encoding categorical features, and creating new features that better capture the underlying credit risk.

## Technologies and Tools Used for the project
- **Python** for all data processing and modeling.
- **Pandas** for data manipulation, **Matplotlib/Seaborn** for visualization, **Scikit-Learn** for machine learning, and **XGBoost** for applying ensemble techniques to enhance model performance.

## My Contribution to the Project
- I focused on two main areas: data preprocessing and model development. In the preprocessing phase, I was responsible for cleaning the dataset, handling missing values, and encoding categorical features to prepare the data for modeling. For model development, I specifically worked on implementing the logistic regression model. I created both a baseline logistic regression model, which achieved an accuracy of 93.33%, and a version with normalized data, enhancing its AUC-ROC to 0.5536. My efforts in these areas ensured that the models had a solid foundation of clean and well-prepared data, contributing to the overall effectiveness and reliability of our predictive models.

## Methodological Approach
The analytical approach was structured as follows:
1. **Exploratory Data Analysis**: Identifying patterns, anomalies, and correlations within the data.
2. **Feature Engineering**: Constructing new variables to better predict outcomes.
3. **Model Development:**
   
     **a. Logistic Regression:** We initially created a baseline model, achieving high accuracy (93.33%) but lower differentiation (AUC-ROC: 0.4286). A version with normalized data was also tested, which enhanced its differentiation capabilities (AUC-ROC: 0.5536).
   
     **b. Recursive Feature Elimination (RFE):** This technique was applied to enhance logistic regression by isolating the top 10 most impactful features, boosting the model's AUC-ROC to 0.6071.
   
     **c. Random Forest:** Implemented with 100 trees, this model demonstrated robust classification capabilities, achieving an AUC-ROC of 0.711 and an accuracy of 91.93%.
   
     **d. XGBoost:** This model was executed with cross-validation, maintaining consistent accuracy (93.33%) and an AUC-ROC of 0.5536. Adjustments through upsampling improved the AUC-ROC to 0.5556, while downsampling reached an AUC-ROC of 0.6667, showing enhanced performance in managing class imbalances.
   
     **e. Model Evaluation:** We utilized comprehensive metrics like Accuracy, Precision, Recall, F1-Score, and ROC-AUC to thoroughly evaluate each model.

## Challenges Encountered
During this project, our group faced several hurdles, such as dealing with unbalanced data and many missing values. We tackled these by using sophisticated methods to fill in missing information and techniques like SMOTE to balance our data. We also found challenges in fine-tuning complex models like XGBoost, which we overcame by using hyperparameter tuning methods to find the best model settings. Another challenge was merging different types of data into a consistent format, which required us to build a strong preprocessing routine. Additionally, coordinating as a team was crucial. We managed this through regular meetings and agile project management, ensuring smooth collaboration and effective sharing of ideas. These challenges greatly sharpened our technical skills and team-working abilities.

## Learning from this project
- This project significantly advanced my understanding and technical expertise in predictive modeling within the financial sector. The meticulous process of data preprocessing not only deepened my appreciation for the importance of data integrity but also highlighted how crucial accuracy and precision are in developing reliable predictive models. Working extensively with logistic regression allowed me to confront and devise strategies for managing imbalanced datasets and optimizing model performance through techniques like ROC-AUC analysis.

Furthermore, collaborating closely with my team enhanced my ability to integrate diverse analytical components into a cohesive system, refining my skills in effective communication and teamwork. This hands-on experience was invaluable in honing both my analytical problem-solving skills and my technical acumen, preparing me for complex challenges in business analytics and ensuring robust model performance in real-world business scenarios.

## Business Impact of Predictive Modeling for Loan Approvals at Home Credit
Implementing the XGBoost model with upsampling at Home Credit offers enhanced credit risk assessment accuracy, supporting financial inclusion by enabling loans to a wider market segment while effectively managing risks. To maximize its impact, Home Credit should ensure high data integrity, continuously monitor model performance, and integrate insights into decision-making processes. Additionally, maintaining ethical standards by regularly evaluating the model for fairness will ensure it aligns with regulatory expectations and customer trust.











   


