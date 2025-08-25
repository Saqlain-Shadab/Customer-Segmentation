<div align="center"> 
## 📊 Customer Segmentation with RFM Analysis & K-Means Clustering
  
</div>

**Project Overview**  
This project uses **RFM (Recency, Frequency, Monetary)** analysis and **K-Means clustering** to segment customers based on purchasing behavior. The goal is to identify customer groups like **high-value buyers**, **inactive customers**, and **average shoppers** to support personalized marketing and business decision-making.

---

**💻 Technologies Used**

- **Python**: Core programming language  
- **Pandas & NumPy**: Data wrangling and aggregation  
- **Matplotlib & Seaborn**: Visualizations  
- **Scikit-learn**: Clustering and scaling  

**🧾 Dataset Overview**  
The dataset includes over **522,000** retail transactions and contains:

- 🧾 **fBillNo**: Invoice number  
- 📦 **Itemname**: Name of the product  
- 🔢 **Quantity**: Number of items purchased  
- 📅 **Date**: Date and time of purchase  
- 💰 **Price**: Price per item (corrected for formatting)  
- 🧍 **CustomerID**: Unique identifier for each customer  
- 🌍 **Country**: Country where the customer is located  
---

**📐 RFM Feature Engineering**  

- 🕒 **Recency**: Days since last purchase from a reference date (`2012-01-01`)  
- 🔁 **Frequency**: Number of unique purchase days per customer  
- 💵 **Monetary**: Total spending of each customer

**📊 Clustering with K-Means**  

- Used the **Elbow Method** to choose optimal clusters  
- Applied **K-Means** with `n_clusters=3`

Final customer segments:

- 🐳 **Whales**: High spenders, frequent buyers, recent transactions  
- 😴 **Lapsed Customers**: Haven’t shopped in a long time, low spending  
- 🙂 **Average Customers**: Moderate spending, recent activity

---

**📈 Segment Summary (Cluster Averages)**  

| Segment         | Recency (days) | Frequency | Monetary Value |
|------------------|----------------|-----------|-----------------|
| 🐳 Whales         | 48.76          | 58.96     | 81,980.00       |
| 😴 Lapsed Cx      | 281.75         | 1.54      | 495.48          |
| 🙂 Avg. Customers | 68.63          | 4.80      | 1,913.38        |

**📊 Segment Distribution**

- 🙂 **Average Customers**: 3,102  
- 😴 **Lapsed Customers**: 1,170  
- 🐳 **Whales**: 25  
---

**🔍 Key Insights**

- A small segment of **Whales** contributes disproportionately to revenue  
- A large group of **Lapsed Customers** shows opportunity for re-engagement  
- **Average Customers** form the bulk of the customer base and can be upsold  
- RFM + Clustering enables **data-driven customer relationship management**
