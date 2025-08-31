# 🎯 Target Brazil SQL Project 🇧🇷

<p align="center">
  <img src="https://1000logos.net/wp-content/uploads/2017/06/Target-Logo.png" alt="Target Logo" width="200"/>
</p>  

## 📖 Overview

Welcome to the **Target Brazil SQL Project** 🛒✨.
Target is a globally recognized retail giant 🏬, known for its **exceptional value, innovation, and unique shopping experience** 💡❤️.

This project explores **Target’s Brazilian operations** 🇧🇷, analyzing **100,000 orders placed between 2016–2018**.
It provides insights into 📦 **orders**, 💳 **payments**, 🚚 **shipping performance**, 🌍 **customer & seller locations**, 🛍️ **products**, and ⭐ **customer reviews**.

✅ **Data Source:** CSV files (7 tables)
✅ **Database:** MySQL (data dumped via Python `mysql-connector`)
✅ **Focus:** End-to-end SQL analysis (basic ➝ intermediate ➝ advanced queries)

---

## 🗂️ Dataset Tables

Here’s a quick peek into the **7 magical tables** 🪄📊:

### 👥 `customers.csv`

* `customer_id` → Consumer ID
* `customer_unique_id` → Unique consumer identifier
* `customer_zip_code_prefix` → Zip code
* `customer_city` → Customer’s city
* `customer_state` → Customer’s state (e.g., SP – São Paulo)

### 🏪 `sellers.csv`

* `seller_id` → Unique seller ID
* `seller_zip_code_prefix` → Seller’s Zip code
* `seller_city` → Seller’s city
* `seller_state` → Seller’s state

### 📦 `order_items.csv`

* `order_id` → Unique order ID
* `order_item_id` → Item ID within an order
* `product_id` → Product ID
* `seller_id` → Seller ID
* `shipping_limit_date` → Deadline for shipping
* `price` → Product price
* `freight_value` → Delivery cost

### 🌍 `geolocation.csv`

* `geolocation_zip_code_prefix` → Zip code prefix
* `geolocation_lat` → Latitude
* `geolocation_lng` → Longitude
* `geolocation_city` → City
* `geolocation_state` → State

### 💳 `payments.csv`

* `order_id` → Order ID
* `payment_sequential` → Payment sequence (for EMI)
* `payment_type` → Mode of payment (e.g., Credit Card)
* `payment_installments` → Number of installments
* `payment_value` → Total paid

### 📑 `orders.csv`

* `order_id` → Unique order ID
* `customer_id` → Customer ID
* `order_status` → Status (delivered, shipped, etc.)
* `order_purchase_timestamp` → Purchase time
* `order_delivered_carrier_date` → Carrier delivery date
* `order_delivered_customer_date` → Customer delivery date
* `order_estimated_delivery_date` → Estimated delivery date

### 🛍️ `products.csv`

* `product_id` → Product ID
* `product_category_name` → Category name
* `product_name_lenght` → Name length
* `product_description_length` → Description length
* `product_photos_qty` → Number of photos
* `product_weight_g` → Weight (grams)
* `product_length_cm` → Length (cm)
* `product_height_cm` → Height (cm)
* `product_width_cm` → Width (cm)

---

## 🧠 SQL Queries

This project is structured into **3 levels of SQL expertise** 🎓:

### 🟢 Basic Queries 🥳

1️⃣ List all unique cities where customers are located 🌍
2️⃣ Count the number of orders placed in 2017 📅
3️⃣ Find the total sales per category 💰
4️⃣ Calculate % of orders paid in installments 💳
5️⃣ Count number of customers from each state 🗺️

### 🟡 Intermediate Queries ⚡

1️⃣ Orders per month in 2018 📈
2️⃣ Average number of products per order, grouped by city 🏙️
3️⃣ % revenue contributed by each product category 💸
4️⃣ Correlation between product price & number of purchases 🔗
5️⃣ Total revenue by seller & rank them by revenue 🏆

### 🔴 Advanced Queries 🚀

1️⃣ Moving average of order values per customer over history 📊
2️⃣ Cumulative sales per month for each year 📅
3️⃣ Year-over-year growth rate of sales 📈
4️⃣ Customer retention rate (repeat purchase within 6 months) ♻️
5️⃣ Top 3 customers who spent the most money in each year 👑

---

## 🚀 Tech Stack

* 🐍 **Python (Jupyter Notebook)** → Data dump into MySQL using \`mysql-con
