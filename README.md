# Credit-Card-Customer-Attrition-Prediction


## 📊 Project Overview
This project analyzes credit card customer attrition for a major financial institution. The goal is to understand the reasons behind customer churn and predict which customers are most likely to leave. By leveraging historical customer data and machine learning, this analysis provides actionable insights to help the bank reduce churn and improve customer retention strategies.

The analysis confirms that **transaction activity** is the strongest predictor of attrition. A predictive model (Random Forest Classifier) was developed to identify high-risk customers, offering a data-driven approach to proactive customer engagement.

## 🔍 Business Problem
[cite_start]Customer retention is vital for profitability in the banking sector, as acquiring a new customer costs 5-7 times more than retaining an existing one[cite: 680]. [cite_start]The bank is currently facing increased credit card customer attrition but lacks clear visibility into the root causes and high-risk profiles[cite: 685]. [cite_start]This project addresses the need for a predictive framework to identify at-risk customers and the behavioral patterns leading to churn[cite: 688].

## 🎯 Objectives
* [cite_start]**Analyze Data:** Explore customer demographics and transaction behaviors to find patterns linked to attrition[cite: 693].
* [cite_start]**Visualize Trends:** Create visualizations to show churn distribution across key segments like age, income, and card category[cite: 697].
* [cite_start]**Predict Churn:** Develop a Random Forest Classifier to predict churn probability and identify the most important features driving customer decisions[cite: 694, 697].
* [cite_start]**Provide Recommendations:** Offer strategic, data-backed recommendations to improve retention[cite: 675].

## 🛠️ Tools & Technologies
* [cite_start]**Language:** Python [cite: 872]
* [cite_start]**IDE:** Google Colab (Jupyter Notebook environment) [cite: 864]
* **Libraries:**
    * [cite_start]**Pandas:** For data manipulation and cleaning[cite: 878].
    * [cite_start]**NumPy:** For numerical computations[cite: 889].
    * [cite_start]**Matplotlib & Seaborn:** For data visualization and EDA[cite: 896].
    * [cite_start]**Scikit-learn:** For machine learning modeling (Random Forest Classifier)[cite: 872, 894].

## 📂 Dataset
[cite_start]The dataset consists of **10,127 observations** and **23 variables**[cite: 917]. It includes:
* [cite_start]**Target Variable:** `Attrition_Flag` (Existing Customer vs. Attrited Customer)[cite: 919].
* [cite_start]**Demographics:** Age, Gender, Dependent count, Education Level, Marital Status, Income Category[cite: 921].
* [cite_start]**Relationship Data:** Months on book, Total Relationship Count, Months Inactive[cite: 921].
* [cite_start]**Card Usage:** Credit Limit, Total Revolving Balance, Utilization Ratio[cite: 923].
* [cite_start]**Transactions:** Total Transaction Amount, Total Transaction Count, Change in Transaction Amount/Count (Q4 vs. Q1)[cite: 923].

## 📈 Key Findings
1.  [cite_start]**Transaction Activity is King:** The strongest predictors of churn are **Total Transaction Count** and **Total Transaction Amount**[cite: 671, 1270]. Low activity is a major red flag.
2.  [cite_start]**The "Cluster of Death":** A distinct cluster of customers exists who make fewer than 40-50 transactions and spend less than $2,500 annually; these customers are at the highest risk of churning[cite: 1136, 672].
3.  [cite_start]**Inactivity Signals Risk:** Months of inactivity and a drop in transaction count/amount from Q4 to Q1 are top indicators of disengagement[cite: 1247, 1272].
4.  [cite_start]**Customer Service Contacts:** High frequency of contacts with the bank is linked to higher churn, suggesting unresolved issues or dissatisfaction[cite: 1249].
5.  [cite_start]**Demographics are Less Predictive:** Factors like age, gender, and income category are less significant predictors compared to behavioral transaction data[cite: 1009, 1058].

## 🤖 Model: Random Forest Classifier
A Random Forest Classifier was chosen for its robustness and ability to rank feature importance.
* [cite_start]**Top Feature:** `Total_Trans_Amt` (Total Transaction Amount)[cite: 1221, 1243].
* [cite_start]**Second Feature:** `Total_Trans_Ct` (Total Transaction Count)[cite: 1222, 1243].
* [cite_start]**Third Feature:** `Total_Revolving_Bal` (Total Revolving Balance)[cite: 1223].
[cite_start]The model confirmed that declining usage and engagement are the primary warning signs of attrition[cite: 1272].

## 💡 Recommendations
1.  **Target Low-Activity Users:** Implement automated alerts for customers whose transaction counts fall below the 40-transaction threshold. [cite_start]Trigger personalized engagement campaigns (e.g., rewards for usage)[cite: 1258, 1259].
2.  [cite_start]**Proactive Support:** Identify customers with high contact rates and escalate their cases to retention specialists to resolve underlying issues before they leave[cite: 1276].
3.  [cite_start]**Personalized Offers:** Utilize EDA findings to target specific high-risk segments (e.g., age 40-50) with relevant offers like balance transfer benefits or fee waivers[cite: 1261].
4.  [cite_start]**Engagement Programs:** Focus on newly onboarded customers to ensure they establish a habit of using the card early on[cite: 1276].

## 🚀 Future Scope
* [cite_start]**Real-Time Dashboard:** Deploy the model into a real-time dashboard for branch managers to monitor churn risk[cite: 1280].
* [cite_start]**Deep Learning:** Experiment with Artificial Neural Networks to potentially improve prediction accuracy[cite: 1282].
* [cite_start]**Sentiment Analysis:** Integrate customer feedback and complaint data to add a qualitative dimension to the churn prediction[cite: 1283].


