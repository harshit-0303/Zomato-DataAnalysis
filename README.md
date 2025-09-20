# 🍽️ Zomato Dataset Analysis  

An in-depth **SQL-based analysis** of the Zomato restaurant dataset to uncover insights into **ratings, pricing, cuisines, service options, and customer preferences**.  
The project also includes a **Power BI dashboard** for interactive data exploration.  

---

## 🔑 Key Insights from SQL Analysis  

### 1️⃣ Rating Distribution & Trends  
- Average rating by **city** and **price range**  
- Best and worst-rated **cuisines**  
- **Top 10** most voted and highly rated restaurants  
- Overall **distribution of ratings** across the dataset  

### 2️⃣ Rating-Based Filtering  
- Top-rated restaurants by **city** and **locality**  
- High-rated restaurants offering **delivery** or **table booking**  
- Currently delivering restaurants with **rating > 4.5**  
- Best restaurants across different **price ranges**  

### 3️⃣ Comparative Insights  
- Ratings comparison: **with vs. without table booking**  
- Ratings comparison: **delivery vs. no delivery**  
- Top-rated restaurants (**rating > 4.5**) segmented by **cuisine**  
- **Cost vs. rating** correlation analysis  

### 4️⃣ Group-Based Aggregations  
- Average rating per **cuisine**  
- **Locality-wise** rating and restaurant count  
- **City leaderboard** based on ratings  
- Rating segmentation:  
  - 🥇 Gold: 4.5–5  
  - 🥈 Silver: 4–4.4  
  - 🥉 Bronze: 3–3.9  
  - ⚠️ Low-rated: <3  

### 5️⃣ Outlier Detection  
- High rating but **low votes** (suspicious quality)  
- High votes but **low rating** (potentially overrated)  
- High cost (≥2000) with **very low rating** (≤1)  

### 6️⃣ Predictive Insights  
- Relationship between **cost and rating**  
- Most consistent **price range** in terms of rating stability  
- City with the **highest average cost**  

---

## 📊 Power BI Dashboard  

To enhance analysis, I developed an **interactive Power BI dashboard** with:  
- 🔍 Filters for city, price range, rating, and cuisine  
- 📈 Visuals for rating distribution, top cuisines, and cost insights  
- 🏆 Role-based leaderboards (top restaurants by votes, cost, and rating)  
- ⚡ Drill-throughs for city-wise and locality-wise exploration
<p align="center">
  <b>Zomato Power BI Dashboard</b>
</p>

<p align="center">
  <img src="https://ik.imagekit.io/vtwmik0pw/Screenshot%202025-08-24%20222404.png?updatedAt=1758391459169" alt="Zomato Power BI Dashboard" width="800"/>
</p> 

---

## 🚀 Additional Features  

- **Customer Preference Analysis**: Which cuisines are most popular in each city  
- **Service Impact Study**: Does offering delivery/table booking boost ratings?  
- **Price Sensitivity Check**: How does restaurant pricing affect customer perception?  
- **Consistency Metrics**: Identifying restaurants with stable performance over time  
- **Potential Business Insights**: Best cities and cuisines to launch new restaurants  

---

## 🛠️ Tech Stack  

- **SQL** → Data extraction and insight generation  
- **Power BI** → Interactive dashboard and visualizations  
- **Excel/CSV** → Dataset handling and preprocessing  

---

## 📂 Project Structure  

Zomato_Dataset_Analysis/  
│
├── SQL_Queries/ # SQL scripts for analysis   
├── PowerBI_Dashboard/ # .pbix dashboard file    
├── Data/ # Zomato dataset (CSV/Excel)    
└── README.md # Documentation    
