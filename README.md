# Food Delivery Data Analysis

## 📌 Project Overview
This project focuses on analyzing food delivery data by combining multiple real-world datasets in different formats. The goal is to create a single source of truth and derive meaningful insights related to user behavior, restaurant performance, revenue trends, and membership impact.

The analysis is performed using **Python and Pandas**.

---

## 📂 Datasets Used
The project uses three different data sources:

- **orders.csv**  
  Transactional data containing order-level details.

- **users.json**  
  User master data containing user information and membership details.

- **restaurants.sql**  
  Restaurant master data containing restaurant details such as cuisine and rating.

---

## 🔗 Data Integration
The datasets are merged using **Left Joins** to ensure all orders are retained.

### Join Keys:
- `orders.user_id` → `users.user_id`
- `orders.restaurant_id` → `restaurants.restaurant_id`

The final merged dataset represents order-level transactional data enriched with user and restaurant attributes.

---

## 🧪 Tools & Technologies
- Python  
- Pandas  
- SQLite (for loading SQL file)  
- Jupyter Notebook / Google Colab  

---

## 📊 Key Analysis Performed
- Total and average revenue analysis
- Gold vs Regular membership comparison
- City-wise and cuisine-wise performance
- Restaurant rating impact on revenue
- Order trends by quarter
- User behavior analysis

---

## 📁 Output
- **final_food_delivery_dataset.csv**  
  This dataset acts as the single source of truth for all analysis and questions.

---

## 🏆 Key Learnings
- Handling and merging datasets from multiple formats (CSV, JSON, SQL)
- Performing left joins using Pandas
- Using groupby, aggregation, and filtering techniques
- Extracting insights from real-world transactional data

---

## ▶️ How to Run
1. Clone the repository  
2. Install required libraries:
   ```bash
   pip install pandas
