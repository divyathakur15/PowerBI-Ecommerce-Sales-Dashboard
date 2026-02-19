# 🚀 Getting Started Guide

## Welcome to E-Commerce Sales Data Analysis Dashboard!

This guide will help you set up and use the Power BI dashboard effectively.

---

## 📋 Table of Contents
1. [Prerequisites](#prerequisites)
2. [Installation Steps](#installation-steps)
3. [Opening the Dashboard](#opening-the-dashboard)
4. [Data Source Configuration](#data-source-configuration)
5. [Dashboard Navigation](#dashboard-navigation)
6. [Troubleshooting](#troubleshooting)
7. [Tips & Best Practices](#tips--best-practices)

---

## ✅ Prerequisites

Before you begin, ensure you have:

### Software Requirements:
- **Power BI Desktop** (Latest version recommended)
  - Download from: [Microsoft Power BI](https://powerbi.microsoft.com/desktop/)
  - Free to use
  - Windows 10/11 or Windows Server 2016 or later

### System Requirements:
- **OS**: Windows 10 or later (64-bit)
- **RAM**: Minimum 2 GB (4 GB+ recommended)
- **Display**: 1440 × 900 or higher resolution
- **Internet**: Required for initial download and updates

### Knowledge Requirements:
- Basic understanding of data analysis concepts
- Familiarity with charts and graphs
- No coding knowledge required!

---

## 📥 Installation Steps

### Step 1: Install Power BI Desktop

1. Visit [https://powerbi.microsoft.com/desktop/](https://powerbi.microsoft.com/desktop/)
2. Click **"Download Free"**
3. Choose installation method:
   - **Option A**: Download from Microsoft Store (Recommended)
   - **Option B**: Download .exe installer
4. Follow installation wizard
5. Launch Power BI Desktop

### Step 2: Download This Project

**Method 1: Using Git**
```bash
git clone https://github.com/divyathakur15/Store-Ecommerce-Sales-Data-Analysis.git
cd Store-Ecommerce-Sales-Data-Analysis
```

**Method 2: Direct Download**
1. Go to the repository page
2. Click **"Code"** → **"Download ZIP"**
3. Extract the ZIP file to your preferred location

---

## 📂 Opening the Dashboard

### Method 1: Direct Open
1. Navigate to the project folder
2. Go to `dashboard` folder
3. Double-click `Ecommerce Sales Analysis Dashboard.pbix`
4. Power BI Desktop will open automatically

### Method 2: From Power BI Desktop
1. Open Power BI Desktop
2. Click **"File"** → **"Open"**
3. Browse to: `dashboard/Ecommerce Sales Analysis Dashboard.pbix`
4. Click **"Open"**

⏱️ **Loading Time**: 10-30 seconds depending on your system

---

## 🔌 Data Source Configuration

### Initial Setup (First Time Only)

If you see a data refresh error:

1. **Click "Transform Data"** in the Home ribbon
2. **Power Query Editor** will open
3. In the left panel, right-click on **"Orders"** query
4. Select **"Advanced Editor"**
5. Update the file path:
   ```
   Source = Csv.Document(File.Contents("C:\YOUR\PATH\raw_data\Orders.csv"))
   ```
   Replace with your actual path to the `raw_data` folder

6. Repeat for **"Details"** query

7. Click **"Close & Apply"**

### Refresh Data

To refresh the dashboard with latest data:

1. Click **"Refresh"** button (Home ribbon)
2. Or press **F5**
3. Wait for refresh to complete

---

## 🧭 Dashboard Navigation

### Main Components:

#### 1. **Filters Panel** (Left Side)
- Filter by date range
- Select specific states/cities
- Choose product categories
- Filter by payment mode

#### 2. **KPI Cards** (Top)
- 💰 Total Sales
- 📊 Total Profit
- 📦 Quantity Sold
- 🛒 Number of Orders

#### 3. **Visualizations** (Center)
- Bar charts for category analysis
- Line charts for trends
- Maps for geographic distribution
- Pie charts for payment modes

#### 4. **Drill-Through Features**
- Right-click any data point
- Select "Drill through" for details
- Use breadcrumbs to navigate back

### Interactive Features:

#### Cross-Filtering
- Click any chart element
- Other visuals filter automatically
- Click again to deselect

#### Tooltips
- Hover over any data point
- View detailed information
- No clicking required

#### Slicers
- Use date slicers for time periods
- Multi-select using **Ctrl + Click**
- Clear selection using eraser icon

---

## 🔧 Troubleshooting

### Problem 1: Dashboard Won't Open
**Error**: "Cannot open file"

**Solutions**:
- Ensure Power BI Desktop is installed
- Check file isn't corrupted
- Try opening Power BI first, then the file
- Verify file extension is `.pbix`

---

### Problem 2: Data Refresh Failed
**Error**: "DataSource.Error"

**Solutions**:
1. Check CSV files are in `raw_data` folder
2. Update data source paths (see [Data Source Configuration](#data-source-configuration))
3. Ensure files aren't open in Excel
4. Check file permissions

---

### Problem 3: Visuals Show "Blank" or "Error"
**Causes**: Data type mismatch or missing relationships

**Solutions**:
1. Check data types in Power Query
2. Verify relationships in Model view
3. Refresh the data source
4. Restart Power BI Desktop

---

### Problem 4: Slow Performance
**Symptoms**: Dashboard takes long to load

**Solutions**:
- Close other applications
- Upgrade RAM if possible
- Remove unnecessary visuals
- Optimize data model
- Use DirectQuery instead of Import

---

### Problem 5: Incorrect Date Formats
**Error**: Dates appear as text

**Solutions**:
1. Go to Power Query Editor
2. Select Date column
3. Change type to **Date**
4. Update format: **DD/MM/YYYY**
5. Close & Apply

---

## 💡 Tips & Best Practices

### For Better Performance:
✅ Close unused programs before opening dashboard
✅ Keep Power BI Desktop updated
✅ Use filters to focus on specific data
✅ Clear cache periodically
✅ Avoid too many visuals on one page

### For Better Analysis:
✅ Start with high-level KPIs
✅ Drill down into specifics
✅ Compare time periods
✅ Look for patterns and anomalies
✅ Export insights to PowerPoint

### For Data Refresh:
✅ Keep CSV files in `raw_data` folder
✅ Don't modify file names
✅ Maintain consistent data structure
✅ Backup before major changes
✅ Test refresh after updates

### Keyboard Shortcuts:
| Shortcut | Action |
|----------|--------|
| **F5** | Refresh data |
| **Ctrl + S** | Save dashboard |
| **Ctrl + N** | New report |
| **Ctrl + O** | Open file |
| **Alt + F4** | Close Power BI |
| **Ctrl + C** | Copy visual |
| **Ctrl + V** | Paste visual |

---

## 📊 Understanding the Data

### Key Metrics Explained:

**Total Sales**
- Sum of all order amounts
- Represents gross revenue
- In Indian Rupees (₹)

**Total Profit**
- Sales minus costs
- Can be negative for loss-making items
- Indicates business profitability

**Profit Margin %**
- (Profit / Sales) × 100
- Shows efficiency
- Higher is better

**Quantity Sold**
- Total items sold
- Indicates demand
- Use for inventory planning

---

## 🎓 Learning Resources

### Power BI Tutorials:
- [Microsoft Learn - Power BI](https://learn.microsoft.com/en-us/power-bi/)
- [Power BI YouTube Channel](https://www.youtube.com/user/mspowerbi)
- [Power BI Community](https://community.powerbi.com/)

### DAX Learning:
- [DAX Guide](https://dax.guide/)
- [SQL BI DAX Resources](https://www.sqlbi.com/topics/dax/)

### Data Visualization Best Practices:
- [Storytelling with Data](https://www.storytellingwithdata.com/)
- [Power BI Design Principles](https://learn.microsoft.com/en-us/power-bi/visuals/power-bi-visualization-best-practices)

---

## 📞 Need Help?

### Common Questions:

**Q: Can I edit the dashboard?**
A: Yes! Click "Edit" to enter edit mode and customize visuals.

**Q: Can I share this dashboard?**
A: Yes! Use File → Publish to Power BI Service (requires account).

**Q: Can I add my own data?**
A: Yes! Replace CSV files in `raw_data` folder with same structure.

**Q: Is this dashboard mobile-friendly?**
A: You can create mobile layouts in Power BI Desktop.

**Q: Can I export data?**
A: Yes! Right-click any visual → Export data → Choose format.

---

## 🎯 Next Steps

After successfully opening the dashboard:

1. ✅ **Explore**: Navigate through different pages
2. ✅ **Interact**: Use filters and slicers
3. ✅ **Analyze**: Identify insights and trends
4. ✅ **Customize**: Modify visuals to your needs
5. ✅ **Share**: Export insights with stakeholders

---

## 📝 Feedback

Found an issue or have suggestions?
- Create an issue on GitHub
- Contact the project maintainer
- Contribute improvements via Pull Request

---

**Happy Analyzing! 📊✨**

---

*Last Updated: February 2026*
*Version: 1.0*
