# 🍕 Pizza Sales Performance & Revenue Analysis

A data analysis project analyzing transactional sales, product demand, and operational trends for a pizza restaurant using MySQL.

---

## 📌 Project Overview

This project evaluates restaurant performance metrics from historical transaction records to help optimize menu offerings, inventory planning, and revenue forecasting.

The analysis focuses on:
* **Sales Volume & Revenue:** Overall earnings, peak periods, and daily average volume.
* **Product Insights:** High-demand pizza types, size popularity, and price outliers.
* **Category Performance:** Relative revenue contribution and top performers by category.
* **Trend Analysis:** Cumulative growth and peak ordering hours.

---

## 📊 Key Highlights & Findings

| Metric | Insight / Value |
| :--- | :--- |
| **Total Orders** | 48,620 orders recorded |
| **Total Revenue** | $817,860.05 |
| **Average Velocity** | ~138 pizzas ordered per day |
| **Top Size Preference** | Large (L) with 18,526 orders |
| **Highest Priced Item** | The Greek Pizza at $35.95 |
| **Top Revenue Driver** | The Thai Chicken Pizza ($43,434.25) |
| **Category Leaders** | Classic leads both in volume (14,888 units) and revenue contribution (26.91%) |
| **Peak Ordering Hours** | Lunch rush (12:00 PM – 1:00 PM) and dinner rush (5:00 PM – 6:00 PM) |

---

## 🗄️ Relational Data Schema

The dataset consists of four interrelated relational tables:

* `orders`: Order transactions metadata (`order_id`, `order_date`, `order_time`).
* `order_details`: Line-item details per order (`order_details_id`, `order_id`, `pizza_id`, `quantity`).
* `pizzas`: SKU-level product data (`pizza_id`, `pizza_type_id`, `size`, `price`).
* `pizza_types`: Catalog information (`pizza_type_id`, `name`, `category`, `ingredients`).

---

## 💡 Business Recommendations

* **Inventory Alignment:** Stock key ingredients for Classic pizzas and Large dough sizes, as they account for the bulk of daily operations.
* **Staff Scheduling:** Adjust shift coverage around peak order windows (12 PM–1 PM and 5 PM–6 PM) to reduce ticket times.
* **Menu Optimization:** Promote high-margin, high-revenue specialty pizzas like The Thai Chicken Pizza and The Barbecue Chicken Pizza through combo deals.
