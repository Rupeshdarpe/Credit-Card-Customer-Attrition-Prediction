# Credit-Card-Customer-Attrition-Prediction


## 📊 Project Overview
This project analyzes credit card customer attrition for a major financial institution. The goal is to understand the reasons behind customer churn and predict which customers are most likely to leave. By leveraging historical customer data and machine learning, this analysis provides actionable insights to help the bank reduce churn and improve customer retention strategies.

The analysis confirms that **transaction activity** is the strongest predictor of attrition. A predictive model (Random Forest Classifier) was developed to identify high-risk customers, offering a data-driven approach to proactive customer engagement.

## 🔍 Business Problem
Customer retention is vital for profitability in the banking sector, as acquiring a new customer costs 5-7 times more than retaining an existing one[cite: 680]. The bank is currently facing increased credit card customer attrition but lacks clear visibility into the root causes and high-risk profiles[cite: 685]. This project addresses the need for a predictive framework to identify at-risk customers and the behavioral patterns leading to churn[cite: 688].

## 🎯 Objectives
* **Analyze Data:** Explore customer demographics and transaction behaviors to find patterns linked to attrition[cite: 693].
* **Visualize Trends:** Create visualizations to show churn distribution across key segments like age, income, and card category[cite: 697].
* **Predict Churn:** Develop a Random Forest Classifier to predict churn probability and identify the most important features driving customer decisions[cite: 694, 697].
* **Provide Recommendations:** Offer strategic, data-backed recommendations to improve retention[cite: 675].

## 🛠️ Tools & Technologies
* **Language:** Python [cite: 872]
* **IDE:** Google Colab (Jupyter Notebook environment) [cite: 864]
* **Libraries:**
    * **Pandas:** For data manipulation and cleaning[cite: 878].
    * **NumPy:** For numerical computations[cite: 889].
    * **Matplotlib & Seaborn:** For data visualization and EDA[cite: 896].
    * **Scikit-learn:** For machine learning modeling (Random Forest Classifier)[cite: 872, 894].

## 📂 Dataset
The dataset consists of **10,127 observations** and **23 variables**[cite: 917]. It includes:
* **Target Variable:** `Attrition_Flag` (Existing Customer vs. Attrited Customer)[cite: 919].
* **Demographics:** Age, Gender, Dependent count, Education Level, Marital Status, Income Category[cite: 921].
* **Relationship Data:** Months on book, Total Relationship Count, Months Inactive[cite: 921].
* **Card Usage:** Credit Limit, Total Revolving Balance, Utilization Ratio[cite: 923].
* **Transactions:** Total Transaction Amount, Total Transaction Count, Change in Transaction Amount/Count (Q4 vs. Q1).

## 📈 Key Findings
1.  **Transaction Activity is King:** The strongest predictors of churn are **Total Transaction Count** and **Total Transaction Amount**[cite: 671, 1270]. Low activity is a major red flag.
2.  **The "Cluster of Death":** A distinct cluster of customers exists who make fewer than 40-50 transactions and spend less than $2,500 annually; these customers are at the highest risk of churning.
3.  **Inactivity Signals Risk:** Months of inactivity and a drop in transaction count/amount from Q4 to Q1 are top indicators of disengagement[cite: 1247, 1272].
4.  **Customer Service Contacts:** High frequency of contacts with the bank is linked to higher churn, suggesting unresolved issues or dissatisfaction[cite: 1249].
5.  **Demographics are Less Predictive:** Factors like age, gender, and income category are less significant predictors compared to behavioral transaction data[cite: 1009, 1058].

## 🤖 Model: Random Forest Classifier
A Random Forest Classifier was chosen for its robustness and ability to rank feature importance.
* **Top Feature:** `Total_Trans_Amt` (Total Transaction Amount).
* **Second Feature:** `Total_Trans_Ct` (Total Transaction Count).
* **Third Feature:** `Total_Revolving_Bal` (Total Revolving Balance).
The model confirmed that declining usage and engagement are the primary warning signs of attrition.

## 💡 Recommendations
1.  **Target Low-Activity Users:** Implement automated alerts for customers whose transaction counts fall below the 40-transaction threshold. Trigger personalized engagement campaigns (e.g., rewards for usage).
2.  **Proactive Support:** Identify customers with high contact rates and escalate their cases to retention specialists to resolve underlying issues before they leave.
3.  **Personalized Offers:** Utilize EDA findings to target specific high-risk segments (e.g., age 40-50) with relevant offers like balance transfer benefits or fee waivers.
4.  **Engagement Programs:** Focus on newly onboarded customers to ensure they establish a habit of using the card early on.

## 🚀 Future Scope
* **Real-Time Dashboard:** Deploy the model into a real-time dashboard for branch managers to monitor churn risk.
* **Deep Learning:** Experiment with Artificial Neural Networks to potentially improve prediction accuracy.
* **Sentiment Analysis:** Integrate customer feedback and complaint data to add a qualitative dimension to the churn prediction.


