# 📖 Data Dictionary

## Overview
This document provides detailed information about all the fields in the dataset used for the E-Commerce Sales Data Analysis project.

---

## 📋 Orders.csv

| Column Name | Data Type | Description | Example | Nullable |
|------------|-----------|-------------|---------|----------|
| **Order ID** | String | Unique identifier for each order, follows format B-XXXXX | B-26055 | No |
| **Order Date** | Date | Date when the order was placed, format: DD-MM-YYYY | 10-03-2018 | No |
| **CustomerName** | String | Full name of the customer who placed the order | Harivansh | No |
| **State** | String | Indian state where the order was delivered | Maharashtra | No |
| **City** | String | City where the order was delivered | Mumbai | No |

### States Covered (20+ States):
- Maharashtra, Delhi, Uttar Pradesh, Madhya Pradesh
- Gujarat, Karnataka, Tamil Nadu, Andhra Pradesh
- West Bengal, Rajasthan, Punjab, Haryana
- Kerala, Bihar, Himachal Pradesh, Jammu and Kashmir
- Goa, Sikkim, Nagaland

### Major Cities:
- Mumbai, Delhi, Pune, Indore, Bangalore
- Hyderabad, Chennai, Ahmedabad, Kolkata, Jaipur
- Chandigarh, Lucknow, Bhopal, Surat, and more

---

## 💰 Details.csv

| Column Name | Data Type | Description | Example | Nullable | Range/Values |
|------------|-----------|-------------|---------|----------|--------------|
| **Order ID** | String | Links to Orders.csv, foreign key relationship | B-26055 | No | Format: B-XXXXX |
| **Amount** | Decimal | Total sale amount in INR (₹) | 5729 | No | Positive values |
| **Profit** | Decimal | Profit/Loss from the transaction in INR (₹) | 64 | No | Can be negative |
| **Quantity** | Integer | Number of items sold in the order | 14 | No | 1-15 |
| **Category** | String | Main product category | Electronics | No | See below |
| **Sub-Category** | String | Detailed product classification | Chairs | No | See below |
| **PaymentMode** | String | Payment method used by customer | Credit Card | No | See below |

---

## 🏷️ Categories Breakdown

### 1. **Electronics**
| Sub-Category | Description |
|-------------|-------------|
| Phones | Mobile phones and smartphones |
| Printers | Printing devices |
| Accessories | Electronic accessories |
| Electronic Games | Gaming devices and consoles |

### 2. **Furniture**
| Sub-Category | Description |
|-------------|-------------|
| Chairs | Office and home chairs |
| Tables | Various types of tables |
| Bookcases | Storage furniture |

### 3. **Clothing**
| Sub-Category | Description |
|-------------|-------------|
| Saree | Traditional Indian wear |
| Kurti | Indian ethnic top wear |
| Stole | Fashion accessory |
| Trousers | Bottom wear |
| Leggings | Casual wear |
| Hankerchief | Accessories |
| Skirt | Women's clothing |

---

## 💳 Payment Modes

| Payment Mode | Description | Typical Use Case |
|-------------|-------------|------------------|
| **Credit Card** | Card-based payment | High-value transactions |
| **COD** | Cash on Delivery | Customers preferring to pay at delivery |
| **EMI** | Equated Monthly Installment | Large purchases split into monthly payments |
| **UPI** | Unified Payments Interface | Digital wallet/bank transfers |

---

## 📊 Data Characteristics

### Data Quality Metrics:
- **Total Orders**: 500 unique orders
- **Total Transactions**: 1,502 records
- **Time Period**: January 1, 2018 - December 31, 2018
- **Geographic Scope**: Pan-India (20+ states)
- **Currency**: Indian Rupees (INR/₹)

### Key Metrics:
- **Average Order Value**: Varies by category
- **Profit Margin**: Can be positive or negative
- **Order Frequency**: Multiple orders per customer possible
- **Quantity Range**: 1-15 items per order

---

## 🔍 Data Relationships

```
Orders.csv (1) ─────< (Many) Details.csv
    │                        │
    └── Order ID ────────── Order ID (Foreign Key)
```

**Relationship Type**: One-to-Many
- One order can have multiple detail records
- Primary Key: Order ID in Orders.csv
- Foreign Key: Order ID in Details.csv

---

## 📈 Calculated Fields (Power BI)

These are commonly used calculated measures in the dashboard:

| Measure Name | Formula/Logic | Purpose |
|-------------|---------------|---------|
| Total Sales | SUM(Details[Amount]) | Calculate total revenue |
| Total Profit | SUM(Details[Profit]) | Calculate total profitability |
| Profit Margin % | (Total Profit / Total Sales) * 100 | Calculate profit percentage |
| Total Quantity | SUM(Details[Quantity]) | Count items sold |
| Total Orders | DISTINCTCOUNT(Orders[Order ID]) | Count unique orders |
| Avg Order Value | Total Sales / Total Orders | Average transaction size |

---

## ⚠️ Data Considerations

### Negative Profit Values:
Some transactions show negative profit, indicating:
- Products sold at a loss
- Discounts/offers applied
- Clearance sales
- Competitive pricing strategies

### Date Format:
- Source Format: DD-MM-YYYY
- Must be converted to proper date format in Power BI
- Enables time intelligence functions

### Data Limitations:
- Data is for 2018 only (single year)
- No product pricing details available
- No customer demographics beyond name
- No shipping or delivery details
- No return/refund information

---

## 🔄 Data Update Frequency

**Current Status**: Static dataset for analysis
**Recommended Updates**: If connecting to live data, consider:
- Daily refresh for operational dashboards
- Weekly refresh for trend analysis
- Monthly refresh for strategic planning

---

## 📝 Notes for Analysts

1. **Profit Analysis**: Always investigate negative profit margins
2. **Seasonality**: Check for seasonal patterns in 2018 data
3. **Geographic Insights**: State/city-level analysis reveals market opportunities
4. **Payment Preferences**: Understand customer payment behavior
5. **Category Performance**: Compare performance across product lines

---

## 📞 Questions or Issues?

If you find any data inconsistencies or need clarification:
- Review the main README.md file
- Check data source documentation
- Contact the project maintainer

---

**Last Updated**: February 2026
**Version**: 1.0
