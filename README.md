# AdventureWorks Analytics

A comprehensive analytics project featuring the AdventureWorks dataset with data files in both CSV and Excel formats, along with Power BI visualizations.

## 📊 Project Overview

This repository contains the AdventureWorks sample database in multiple formats, designed for analytics and business intelligence projects. It includes sales data, customer information, product catalogs, and return transactions.

## 📁 Project Structure

```
AdventureWorks/
├── CSV Files/                              # CSV format data files
│   ├── Adventure Works.csv                 # Main sales transactions
│   ├── AdventureWorks_Calendar.csv         # Calendar dimension
│   ├── AdventureWorks_Customers.csv        # Customer information
│   ├── AdventureWorks_Product_Categories.csv
│   ├── AdventureWorks_Product_Subcategories.csv
│   ├── AdventureWorks_Products.csv         # Product catalog
│   ├── AdventureWorks_Returns.csv          # Product returns
│   └── AdventureWorks_Territories.csv      # Sales territories
├── Excel Files/                            # Excel format data files
│   ├── Adventure Works.xlsx
│   ├── AdventureWorks_Calendar.xlsx
│   ├── AdventureWorks_Customers.xlsx
│   ├── AdventureWorks_Product_Categories.xlsx
│   ├── AdventureWorks_Product_Subcategories.xlsx
│   ├── AdventureWorks_Products.xlsx
│   ├── AdventureWorks_Returns.xlsx
│   └── AdventureWorks_Territories.xlsx
├── AdventureWork.pbix                      # Power BI dashboard file
├── AdventureWork Dashboard.png             # Dashboard screenshot
└── README.md                               # This file
```

## 📋 Data Files Description

### Sales Data
- **Adventure Works.csv/xlsx** - Main transaction data containing sales records with dates, customers, products, and amounts

### Dimensions
- **AdventureWorks_Calendar.csv/xlsx** - Date dimension for time-based analysis
- **AdventureWorks_Customers.csv/xlsx** - Customer master data with demographics
- **AdventureWorks_Products.csv/xlsx** - Product information and specifications
- **AdventureWorks_Product_Categories.csv/xlsx** - Product category hierarchy
- **AdventureWorks_Product_Subcategories.csv/xlsx** - Product subcategory details
- **AdventureWorks_Territories.csv/xlsx** - Geographic sales territories

### Operations
- **AdventureWorks_Returns.csv/xlsx** - Product return transactions

## 🛠️ Tools & Technologies

- **Data Format**: CSV and Excel
- **Visualization**: Power BI Desktop
- **Dataset**: AdventureWorks Sample Database

## 📈 Use Cases

This dataset is ideal for:
- Sales analytics and reporting
- Customer behavior analysis
- Product performance analysis
- Territory and region analysis
- Time-series analysis
- Data visualization practice
- Business intelligence projects

## 🚀 Getting Started

### Using CSV Files
```python
import pandas as pd

# Load main sales data
sales = pd.read_csv('CSV Files/Adventure Works.csv')
customers = pd.read_csv('CSV Files/AdventureWorks_Customers.csv')
products = pd.read_csv('CSV Files/AdventureWorks_Products.csv')
```

### Using Excel Files
```python
import pandas as pd

# Load from Excel
sales = pd.read_excel('Excel Files/Adventure Works.xlsx')
customers = pd.read_excel('Excel Files/AdventureWorks_Customers.xlsx')
```

### Power BI Analysis
1. Open `AdventureWork.pbix` in Power BI Desktop
2. Explore the pre-built dashboard visualization
3. Refresh data connections to your local files as needed

## 📊 Power BI Dashboard

The included `AdventureWork.pbix` file contains a comprehensive dashboard with:
- Sales performance metrics
- Customer analytics
- Product analysis
- Territory insights
- Return analysis

A screenshot of the dashboard is available in `AdventureWork Dashboard.png`

## 📝 License

This dataset is based on the AdventureWorks sample database from Microsoft.

## 🤝 Contributing

Feel free to fork this repository and create your own analyses or improvements.

## 📧 Contact

For questions or suggestions, please open an issue in the GitHub repository.

---

**Last Updated**: June 2026
