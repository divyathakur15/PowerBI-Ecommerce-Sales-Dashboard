# 📊 E-Commerce Sales Data Analysis Dashboard

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Data Analysis](https://img.shields.io/badge/Data%20Analysis-4285F4?style=for-the-badge&logo=google-analytics&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-success?style=for-the-badge)

## 📋 Project Overview

This project presents a comprehensive **E-Commerce Sales Data Analysis** using Power BI. The dashboard provides actionable insights into sales performance, customer behavior, product categories, and payment preferences across different states and cities in India.

### 🎯 Objectives

- Analyze e-commerce sales trends across different time periods (2018)
- Identify top-performing products, categories, and regions
- Understand customer purchasing patterns and payment mode preferences
- Visualize profit margins and revenue distribution
- Provide data-driven insights for business decision-making

---

## 📁 Project Structure

```
PowerBI-Ecommerce-Sales-Dashboard/
│
├── raw_data/                      # Raw dataset files
│   ├── Orders.csv                 # Customer order information
│   └── Details.csv                # Transaction details
│
├── dashboard/                     # Power BI dashboard files
│   └── Ecommerce Sales Analysis Dashboard.pbix
│
├── output/                        # Screenshots and exports
│   ├── Ecommerce Sales Dashboard.PNG  # Dashboard screenshot
│   └── README.md                      # Output folder guide
│
├── README.md                      # Project documentation
└── dark-gradient.jpg              # Dashboard background asset
```

---

## 📊 Dataset Description

### 1. **Orders.csv**
Contains customer and order information:
- **Order ID**: Unique identifier for each order
- **Order Date**: Date when the order was placed (format: DD-MM-YYYY)
- **CustomerName**: Name of the customer
- **State**: State where the order was shipped
- **City**: City where the order was shipped

**Sample Size**: 500 orders
**Time Period**: January 2018 - December 2018

### 2. **Details.csv**
Contains transaction-level details:
- **Order ID**: Links to Orders.csv
- **Amount**: Total sale amount
- **Profit**: Profit earned from the transaction
- **Quantity**: Number of items sold
- **Category**: Product category (Electronics, Furniture, Clothing)
- **Sub-Category**: Detailed product classification
- **PaymentMode**: Payment method used (COD, Credit Card, EMI, UPI)

**Sample Size**: 1,502 transaction records

---

## 🔍 Key Insights & Metrics

### Categories Analyzed:
1. **Electronics**
   - Phones
   - Printers
   - Accessories
   - Electronic Games

2. **Furniture**
   - Chairs
   - Tables
   - Bookcases

3. **Clothing**
   - Saree, Kurti, Stole
   - Trousers, Leggings
   - Hankerchief, Skirt

### Geographic Coverage:
- **States**: 20+ states across India
- **Major Cities**: Mumbai, Delhi, Pune, Indore, Bangalore, Hyderabad, Chennai, and more

### Payment Methods:
- Credit Card
- Cash on Delivery (COD)
- EMI (Equated Monthly Installment)
- UPI (Unified Payments Interface)

---

## 🛠️ Tools & Technologies

- **Power BI Desktop**: Dashboard creation and data visualization
- **DAX (Data Analysis Expressions)**: Calculated measures and KPIs
- **Power Query**: Data cleaning and transformation
- **CSV**: Raw data format

---

## 📈 Dashboard Features

### Key Performance Indicators (KPIs):
- 💰 **Total Revenue**: Sum of all sales
- 📊 **Total Profit**: Overall profitability
- 📦 **Total Quantity Sold**: Volume of products
- 🛒 **Number of Orders**: Total transactions

### Visualizations Include:
- 📍 **Geographic Sales Distribution** (State/City-wise analysis)
- 📅 **Time Series Analysis** (Monthly trends)
- 🏷️ **Category & Sub-Category Performance**
- 💳 **Payment Mode Distribution**
- 👥 **Top Customers Analysis**
- 📉 **Profit Margin Analysis**
- 🎯 **Product Performance Comparison**

---

## 🚀 Getting Started

### Prerequisites
- **Power BI Desktop** (Download from [Microsoft Store](https://powerbi.microsoft.com/desktop/))
- Windows 10 or later / macOS with Power BI

### How to Use

1. **Clone this repository**
   ```bash
   git clone https://github.com/divyathakur15/PowerBI-Ecommerce-Sales-Dashboard.git
   ```

2. **Navigate to the project folder**
   ```bash
   cd PowerBI-Ecommerce-Sales-Dashboard
   ```

3. **Open the Power BI file**
   - Go to the `dashboard` folder
   - Double-click on `Ecommerce Sales Analysis Dashboard.pbix`
   - The dashboard will open in Power BI Desktop

4. **Refresh Data** (if needed)
   - Click on "Refresh" in the Home ribbon
   - Ensure the CSV files are in the `raw_data` folder

5. **Explore the Dashboard**
   - Use filters and slicers to interact with the data
   - Hover over visuals for detailed tooltips
   - Drill down into specific categories or regions

---

## 📊 Data Preparation Steps

1. **Data Import**: Loaded CSV files into Power BI
2. **Data Cleaning**: 
   - Handled missing values
   - Standardized date formats
   - Removed duplicates
3. **Data Transformation**:
   - Created relationships between Orders and Details tables
   - Added calculated columns for time intelligence
4. **Data Modeling**:
   - Established one-to-many relationships
   - Created measures using DAX

---

## 💡 Business Insights

Some potential insights this dashboard can reveal:

- 🎯 **Which product categories generate the highest profit margins?**
- 📍 **Which states/cities are the most profitable markets?**
- 💳 **What payment methods do customers prefer?**
- 📆 **What are the peak sales months?**
- 👤 **Who are the top-spending customers?**
- 📉 **Which products have negative profit margins?**

---

## 📸 Screenshots

### Main Dashboard
![Dashboard Overview](output/Ecommerce%20Sales%20Dashboard.PNG)

*Full interactive dashboard available in the `dashboard` folder*

---

## 🔄 Future Enhancements

- [ ] Add year-over-year comparison functionality
- [ ] Implement predictive analytics for sales forecasting
- [ ] Create mobile-optimized dashboard layout
- [ ] Add customer segmentation analysis
- [ ] Integrate real-time data refresh
- [ ] Include inventory management metrics

---

## 📝 Lessons Learned

- Data quality is crucial for accurate analysis
- Proper data modeling improves dashboard performance
- Interactive filters enhance user experience
- Visual hierarchy guides insight discovery

---

## 🤝 Contributing

Contributions are welcome! If you'd like to improve this project:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 👤 Author

**Divya Thakur**

- GitHub: [@divyathakur15](https://github.com/divyathakur15)
- LinkedIn: [Connect with me](https://www.linkedin.com/in/divyathakur15)

---

## 🙏 Acknowledgments

- Thanks to the Power BI community for inspiration and resources
- Dataset simulated for educational and analytical purposes
- Special thanks to Power BI DECODE for guidance

---

## 📧 Contact

For questions or feedback, please reach out through:
- 📧 Email: [divya.thakur1506@gmail.com]
- 💼 LinkedIn: [ linkedin.com/in/divya-thakur-15june2004/ ]

---

<div align="center">
  
### ⭐ If you found this project helpful, please consider giving it a star!

**Made with ❤️ and Power BI**

</div>