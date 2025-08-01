# 🚚 Supply Chain Optimization



---

## 🛒 Background

A retail company wants to improve supply chain efficiency by analyzing:

- Supplier performance  
- Inventory levels  
- Order fulfillment  
- Shipment trends

---

## 🎯 Objectives

- Identify reliable suppliers  
- Reduce stockouts and carrying costs  
- Optimize delivery and order timelines  
- Extract trends for strategic planning

---

## 🗂️ Database Schema

### Suppliers Table

| Column Name      | Description           |
|------------------|-----------------------|
| `supplier_id`    | Primary Key           |
| `supplier_name`  | Supplier Name         |
| `contact_person` | Main Contact          |
| `phone_number`   | Contact Number        |
| `email`          | Email Address         |

### Products Table

| Column Name      | Description              |
|------------------|--------------------------|
| `product_id`     | Primary Key              |
| `product_name`   | Product Name             |
| `description`    | Description              |
| `unit_price`     | Price per Unit           |
| `quantity_in_stock` | Inventory Level      |

### Orders Table

| Column Name      | Description              |
|------------------|--------------------------|
| `order_id`       | Primary Key              |
| `product_id`     | FK → Products            |
| `supplier_id`    | FK → Suppliers           |
| `order_date`     | Order Placement Date     |
| `quantity_ordered` | Quantity               |
| `order_status`   | In Progress / Complete   |

### Shipments Table

| Column Name      | Description              |
|------------------|--------------------------|
| `shipment_id`    | Primary Key              |
| `order_id`       | FK → Orders              |
| `shipment_date`  | Shipping Date            |
| `delivery_date`  | Delivery Date            |
| `shipping_company` | Carrier Name           |
| `tracking_number` | Shipment ID             |

📥 **Dataset Download**: _Click here_  
🔧 *If data lacks fields, create sample data.*

---

## 📊 Analysis & Recommendations

### 1️⃣ Supplier Performance

- Revenue by supplier  
- Avg. delivery time  
- Identify suppliers with declining or unstable performance

### 2️⃣ Inventory Optimization

- Highlight low-stock items (<50 units)  
- Demand forecasting  
- Auto-replenishment triggers

### 3️⃣ Order Fulfillment

- Bottleneck identification  
- Avg. shipment duration by shipping company  
- Order processing performance metrics

### 4️⃣ Trend & Strategic Insights

- Seasonal product demand  
- Customer demographics vs. product orders  
- Forecast future demand

---

## 🧪 SQL Analysis

### 🟢 Basic

- Select all suppliers  
- Product name + price  
- Orders: IDs + dates  
- Shipments: IDs + dates  
- Count total products in stock  
- Avg. unit price  
- Max quantity ordered  
- Suppliers & contacts  
- Product descriptions  
- Shipment tracking details

### 🟡 Intermediate

- Orders + supplier info  
- Products with price > $15  
- Order count per supplier  
- Quantity ordered per product  
- Shipments + order info  
- Suppliers with >2 contacts  
- Avg. quantity ordered  
- Products with order count  
- Orders in progress  
- Earliest & latest order dates  
- Total revenue  
- Quantity ordered per supplier

### 🔴 Advanced

- Products with highest price  
- Top 3 most ordered products  
- Completed orders percentage  
- Shipments per carrier  
- Inactive suppliers  
- Orders + shipment details  
- Top 5 suppliers by quantity  
- Revenue by supplier  
- Avg. delivery per carrier  
- Products never ordered  
- Top shipping companies  
- Completed orders % by supplier  
- Low stock items (<50)  
- Top 5 suppliers by revenue  
- Monthly order volume  
- Suppliers with 3-month drop  
- Avg. shipment duration  
- Seasonal demand  
- Product popularity trends  
- Correlations with demographics  
- Forecast future demand
