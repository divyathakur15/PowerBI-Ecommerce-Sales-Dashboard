# 📁 Project Structure

## Visual Folder Hierarchy

```
Store-Ecommerce-Sales-Data-Analysis/
│
├── 📂 raw_data/                          # Source Data Files
│   ├── 📄 Orders.csv                     # Customer order information (500 orders)
│   └── 📄 Details.csv                    # Transaction details (1,502 records)
│
├── 📂 dashboard/                         # Power BI Files
│   └── 📊 Ecommerce Sales Analysis Dashboard.pbix    # Main dashboard
│
├── 📂 output/                            # Exports & Screenshots
│   ├── 📸 Ecommerce Sales Dashboard.PNG  # Dashboard screenshot
│   └── 📄 README.md                      # Output folder guide
│
├── 📂 .git/                              # Git version control
│
├── 📄 README.md                          # Main project documentation ⭐
├── 📄 DATA_DICTIONARY.md                 # Detailed field descriptions
├── 📄 GETTING_STARTED.md                 # User setup guide
├── 📄 CHANGELOG.md                       # Version history
├── 📄 PROJECT_STRUCTURE.md               # Project structure documentation
├── 📄 RESTRUCTURING_SUMMARY.md           # Restructuring summary
├── 📄 .gitignore                         # Git ignore rules
└── 🖼️ dark-gradient.jpg                  # Dashboard background asset
```

---

## 📋 File Descriptions

### Root Level Files

| File | Purpose | Size | Priority |
|------|---------|------|----------|
| **README.md** | Main project documentation, overview, features | ~8 KB | ⭐⭐⭐ |
| **DATA_DICTIONARY.md** | Field definitions and data schema | ~6 KB | ⭐⭐⭐ |
| **GETTING_STARTED.md** | Setup and usage instructions | ~7 KB | ⭐⭐⭐ |
| **CHANGELOG.md** | Version history and updates | ~3 KB | ⭐⭐ |
| **.gitignore** | Git exclusion rules | ~1 KB | ⭐⭐ |
| **dark-gradient.jpg** | Dashboard visual asset | Variable | ⭐ |

---

### 📂 raw_data/ Folder

**Purpose**: Store source CSV files

| File | Records | Columns | Description |
|------|---------|---------|-------------|
| **Orders.csv** | 500 | 5 | Order and customer information |
| **Details.csv** | 1,502 | 7 | Transaction-level details |

**Key Points:**
- ✅ Keep files in this folder for proper dashboard functioning
- ✅ Don't rename these files
- ✅ Maintain the same column structure when updating
- ⚠️ Backup before modifying

---

### 📂 dashboard/ Folder

**Purpose**: Store Power BI dashboard file

| File | Type | Description |
|------|------|-------------|
| **Ecommerce Sales Analysis Dashboard.pbix** | Power BI | Main interactive dashboard |

**Features:**
- Interactive visualizations
- Multiple pages/tabs
- Custom DAX measures
- Data relationships
- Filters and slicers

**To Use:**
1. Double-click to open in Power BI Desktop
2. Or open Power BI first, then load file
3. Refresh data if needed (F5)

---

### 📂 output/ Folder

**Purpose**: Store exported files and screenshots

**Recommended Contents:**
```
output/
├── 📸 screenshots/
│   ├── dashboard-overview.png
│   ├── sales-by-category.png
│   ├── geographic-map.png
│   └── payment-analysis.png
│
├── 📊 reports/
│   ├── monthly-report.pdf
│   ├── executive-summary.pptx
│   └── data-export.xlsx
│
└── 📝 README.md
```

**Note:** This folder starts empty. Add your exports here.

---

## 🔄 Data Flow

```
┌─────────────────┐
│   Orders.csv    │────┐
└─────────────────┘    │
                       │
                       ├───► 📊 Power BI Dashboard
                       │     │
┌─────────────────┐    │     │
│   Details.csv   │────┘     ├───► 📈 Visualizations
└─────────────────┘          │
                             ├───► 📊 KPIs
                             │
                             └───► 📂 Exported Reports
                                   (output folder)
```

---

## 📊 File Sizes (Approximate)

| Component | Size Range |
|-----------|------------|
| Orders.csv | ~50-100 KB |
| Details.csv | ~100-150 KB |
| Dashboard.pbix | ~500 KB - 2 MB |
| Documentation | ~25 KB total |
| Total Project | ~1-3 MB |

*Sizes may vary based on data volume and dashboard complexity*

---

## 🎯 File Usage Guide

### For End Users:
1. ⭐ **Start Here**: `README.md`
2. 📖 **Learn Setup**: `GETTING_STARTED.md`
3. 📊 **Open Dashboard**: `dashboard/Ecommerce Sales Analysis Dashboard.pbix`
4. 📚 **Understand Data**: `DATA_DICTIONARY.md`

### For Developers/Analysts:
1. 📊 Modify dashboard: `dashboard/*.pbix`
2. 📝 Update docs: `README.md`, `DATA_DICTIONARY.md`
3. 🔄 Track changes: `CHANGELOG.md`
4. 💾 Version control: `.git/`, `.gitignore`

### For Data Updates:
1. 📂 Replace files in: `raw_data/`
2. 🔄 Refresh dashboard: Press F5 in Power BI
3. ✅ Verify visuals update correctly
4. 📸 Export new screenshots: `output/`

---

## 🔐 Important Notes

### DO ✅
- Keep raw_data folder structure intact
- Backup before making changes
- Document any modifications in CHANGELOG
- Save dashboard frequently (Ctrl+S)
- Export important insights to output/

### DON'T ❌
- Rename CSV files
- Change column headers in CSVs
- Delete relationship connections in Power BI
- Open CSV files while dashboard is refreshing
- Commit large files (>100MB) to Git

---

## 🚀 Quick Navigation

| I Want To... | Go To... |
|--------------|----------|
| Understand the project | `README.md` |
| Open the dashboard | `dashboard/Ecommerce Sales Analysis Dashboard.pbix` |
| Learn field meanings | `DATA_DICTIONARY.md` |
| Set up for first time | `GETTING_STARTED.md` |
| Update data | `raw_data/*.csv` |
| Save exports | `output/` |
| Check version history | `CHANGELOG.md` |

---

## 📦 Backup Recommendations

**What to Backup:**
1. ✅ Entire project folder
2. ✅ Especially: `dashboard/*.pbix`
3. ✅ And: `raw_data/*.csv`

**Backup Frequency:**
- Before major changes: **Always**
- During development: **Daily**
- Production version: **Weekly**

**Backup Locations:**
- Local: External drive
- Cloud: OneDrive, Google Drive, Dropbox
- Version Control: GitHub repository

---

## 🔄 Update Workflow

```
1. Backup current version
   ↓
2. Update CSV files in raw_data/
   ↓
3. Open dashboard in Power BI
   ↓
4. Refresh data (F5)
   ↓
5. Verify visuals are correct
   ↓
6. Save dashboard (Ctrl+S)
   ↓
7. Export reports to output/
   ↓
8. Update CHANGELOG.md
   ↓
9. Commit to Git (if using version control)
```

---

## 📞 Need Help?

**File-Related Issues:**
- Missing files → Check folder structure above
- Can't find file → Use search (Ctrl+F) in File Explorer
- File won't open → Check file extension and associated program

**Dashboard Issues:**
- Data refresh errors → Check CSV file paths
- Broken visuals → Verify data relationships
- Performance issues → Check file sizes and system resources

---

**Last Updated**: February 2026
**Version**: 1.0
**Maintained by**: Divya Thakur
