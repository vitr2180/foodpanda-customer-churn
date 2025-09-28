# Foodpanda Customer Churn & Loyalty Analysis

This project focuses on understanding and reducing customer churn for **Foodpanda**, a leading online food delivery platform that operates across multiple countries. Foodpanda connects millions of customers to restaurants, cafes, and grocery stores, offering everything from hot meals to daily essentials delivered straight to their doorsteps. With its wide reach and convenience, Foodpanda has become an important player in the rapidly growing food delivery industry.  

But in such a competitive market, keeping customers loyal is just as important as acquiring new ones. Customer acquisition campaigns are costly, and when users stop ordering, Foodpanda not only loses future revenue but also faces the added expense of replacing those customers. Retaining users, on the other hand, strengthens long-term profitability, improves customer lifetime value, and creates a base of loyal advocates who are more likely to order repeatedly and try new services.  

This project takes a closer look at Foodpanda’s customer data to uncover the factors that influence whether users stay engaged or become inactive. By examining patterns such as ordering behavior, loyalty points, spending levels, and delivery experiences, we aim to provide insights that can help Foodpanda design smarter retention strategies. The ultimate goal is to use these insights to support better business decisions, reduce churn, and create more sustainable growth for the platform.

---

## 📊 Dataset
- **Source:** [Foodpanda Analysis Dataset 2025 (Kaggle)](https://www.kaggle.com/datasets/nabihazahid/foodpanda-analysis-dataset-2025)  
- **Size:** 6,000 customer records  
- **Features include:**
  - Demographics (age, gender, city)  
  - Order behavior (frequency, value, recency)  
  - Loyalty points & ratings  
  - Delivery experience & churn status  

---

## 🔍 Methodology
We structured the analysis into three phases:

1. **Descriptive Analytics (EDA)**  
   - Explored churn by gender, city, and delivery status  
   - Compared loyalty points, order frequency, and order value between active and inactive customers  

2. **Predictive Analytics (ML Models)**  
   - Tested Logistic Regression and Random Forest classifiers  
   - Found limited predictive power (AUC ≈ 0.5), showing churn is difficult to predict with current features  

3. **Prescriptive Analytics (Optimization)**  
   - Designed **budget-constrained retention campaigns**  
   - Compared single-channel and multi-channel strategies (loyalty boosts, discounts, free delivery)  
   - Showed which mix of interventions maximizes retention impact within budget limits  

---

## ✅ Key Findings
- **Churn Drivers**:  
  - Recency (days since last order) and delivery experience are strong churn indicators  
  - Loyalty points strongly linked with customer activity  

- **Model Insights**:  
  - Predictive models struggled to distinguish churners vs. non-churners  
  - Indicates churn may depend on external factors not in the dataset (e.g., competition, food quality)  

- **Campaign Optimization**:  
  - Budget of **25k gave the best ROI per cost unit**  
  - Loyalty points were the **most effective retention lever** compared to discounts or free delivery  

---

## 📌 Business Recommendations
- **Prioritize retention campaigns** around loyalty points rather than discounts, which are less cost-effective  
- **Segment customers** by recency and loyalty points to maximize campaign ROI  
- **Use prescriptive optimization** to allocate budgets more efficiently under financial constraints  
- **Future work**: include external variables (competitor pricing, food quality) to strengthen prediction  

---

## 🛠️ Tools Used
- Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)  
- PuLP for optimization modeling  
- Jupyter Notebook  

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/YOURUSERNAME/foodpanda-churn-analysis.git
   cd foodpanda-churn-analysis
