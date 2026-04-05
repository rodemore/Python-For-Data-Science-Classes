# Python for Data Science - Course Materials

This repository contains comprehensive materials from my Python for Data Science bootcamp, including lectures, hands-on activities, homework assignments, and datasets. Each week focuses on different aspects of data analysis and customer analytics.

## Table of Contents
- [Course Overview](#course-overview)
- [Repository Structure](#repository-structure)
- [Week-by-Week Breakdown](#week-by-week-breakdown)
- [Datasets](#datasets)
- [How to Use This Repository](#how-to-use-this-repository)
- [Technologies Used](#technologies-used)

## Course Overview

This 4-week intensive bootcamp covers Python programming for data science with a focus on:
- Data manipulation with Pandas
- Exploratory Data Analysis (EDA)
- Customer segmentation and RFM analysis
- Data visualization with Matplotlib and Seaborn
- Data cleaning and preparation techniques
- Real-world business analytics applications

## Repository Structure

```
Python-For-Data-Science-Classes/
├── Week 1/                          # Introduction to Pandas & EDA
│   ├── Lectures/                    # Session notebooks
│   └── Activities/                  # Hands-on exercises (empty + solutions)
├── Week 2/                          # Customer Segmentation & RFM
│   ├── Lectures/                    # Session notebooks
│   ├── Activities/                  # Workshop exercises
│   └── Homework/                    # Assignments
├── Week 3/                          # Data Visualization & Analysis
│   ├── Lectures/                    # Session notebooks
│   └── Activities/                  # Workshop exercises
├── Week 4/                          # Data Cleaning & Preparation
│   ├── Lectures/                    # Session notebooks
│   └── Activities/                  # Workshop exercises
├── README.md                        # This file
├── DATA_SOURCES.md                  # Complete dataset documentation
└── .gitignore                       # Git ignore rules

Note: All datasets are hosted on AWS S3 and loaded directly in notebooks.
No local Data/ folders required!
```

## Week-by-Week Breakdown

### Week 1: Introduction to Pandas & EDA
**Topics Covered:**
- Python environment setup
- Pandas fundamentals (Series, DataFrames)
- Data loading and exploration
- Basic data manipulation

**Key Activities:**
- `DataCleaning_Activity.ipynb` - Data cleaning workshop (empty template)
- `DataCleaning_Activity_Solution.ipynb` - Solution with best practices

**Lectures:**
- `Init.ipynb` - Environment setup and introduction
- `IntroPandasI.ipynb` - Pandas basics
- `IntroPandasII.ipynb` - Intermediate Pandas operations
- `IntroPandasIII.ipynb` - Advanced Pandas techniques

**Datasets:** (All loaded from S3)
- `people.csv` - Sample people data
- `employees.csv` / `employees_workshop.csv` - Employee datasets for practice
- See [DATA_SOURCES.md](DATA_SOURCES.md) for download links

---

### Week 2: Customer Segmentation & RFM Analysis
**Topics Covered:**
- Customer segmentation strategies
- RFM (Recency, Frequency, Monetary) analysis
- Customer lifetime value
- Sales analytics
- Pareto analysis

**Key Activities:**
- `EDA_sales_drinks_Activity.ipynb` - Comprehensive sales EDA (empty template)
- `EDA_sales_drinks_Solution.ipynb` - Complete solution with visualizations
- `RFM_Segmentation_Activity.ipynb` - RFM analysis workshop (empty template)
- `RFM_Segmentation_Solution.ipynb` - Full RFM implementation
- `RFM_Sales_Analysis_Solution.ipynb` - Advanced RFM with sales data

**Homework:**
- `RFM_Homework.ipynb` - Apply RFM to new dataset (empty template)
- `RFM_Homework_Solution.ipynb` - Complete solution
- `Complete_Homework_Solution.ipynb` - Comprehensive assignment solution
- `Activity_Session4_Solution.ipynb` - Session 4 practice exercises

**Lectures:**
- `Segmentos.ipynb` - Customer segmentation fundamentals

**Datasets:** (All loaded from S3)
- `sales_drinks.csv` - **Main beverage sales dataset** (1.8M+ transactions)
- `Clients.csv` - Customer information
- `sales.csv` - Sales transactions
- `invoices.csv` - Invoice data
- `products.csv` - Product catalog
- `categories.csv` - Product categories
- `products.json` - Product data in JSON format
- See [DATA_SOURCES.md](DATA_SOURCES.md) for download links

---

### Week 3: Data Visualization & Advanced Analysis
**Topics Covered:**
- Advanced data visualization techniques
- Statistical analysis
- Outlier detection and handling
- Product profitability analysis
- Customer churn analysis
- Market basket analysis
- Discount impact analysis

**Key Activities:**
- `Product_Analysis_Activity.ipynb` - Product analysis workshop (empty template)
- `Product_Analysis_Solution.ipynb` - Complete product analysis
- `Discount_Impact_Activity.ipynb` - Discount effectiveness analysis (empty)
- `Discount_Impact_Solution.ipynb` - Full discount analysis with insights
- `Market_Basket_Activity.ipynb` - Association rules mining (empty template)
- `Market_Basket_Solution.ipynb` - Complete market basket analysis
- `Churn_Analysis_Solution.ipynb` - Customer churn prediction

**Lectures:**
- `sesion7.ipynb` - Advanced analytics session 7
- `sesion8.ipynb` - Advanced analytics session 8
- `visualizaciones.ipynb` - Data visualization best practices

**Datasets:** (All loaded from S3)
- `bank_transactions.csv` - Banking transaction data
- `sales_drinks.csv` - Beverage sales data
- `ventas_completo.csv` - Complete sales dataset
- See [DATA_SOURCES.md](DATA_SOURCES.md) for download links

---

### Week 4: Data Cleaning & Missing Values
**Topics Covered:**
- Missing value strategies and imputation
- Data quality assessment
- Data type conversions
- Outlier handling
- Data optimization techniques
- Marketing data preparation
- Exploratory Data Analysis with the Titanic dataset

**Key Activities:**
- `Data_Cleaning_Activity.ipynb` - Data cleaning workshop (empty template)
- `Marketing_Workshop_Solution.ipynb` - Marketing data cleaning solution
- `Analisis_Titanic_EDA_Activity.ipynb` - Complete EDA on Titanic dataset (empty template)
- `Analisis_Titanic_EDA_Solution.ipynb` - Fully worked solution

**Lectures:**
- `missing_values.ipynb` - Handling missing data
- `Titanic_prompts.ipynb` - Titanic dataset challenges

**Datasets:** (All loaded from S3)
- `employees_workshop.csv` - Employee data for cleaning practice
- `marketing_data_clean.csv` - Cleaned marketing dataset
- See [DATA_SOURCES.md](DATA_SOURCES.md) for download links

---

## Datasets

### 📊 Data Access - Cloud-Based Learning

**All datasets are hosted on AWS S3 for seamless access!**

The notebooks in this repository are configured to load data directly from AWS S3 - no manual downloads required. Simply run the notebooks and the data will be fetched automatically.

```python
# Example: Loading data from S3
url = 'https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/sales_drinks.csv'
df = pd.read_csv(url)
```

### Download Links (Optional)

If you prefer to download the datasets locally, use these direct links:

**Week 1 - Introduction to Pandas:**
- [people.csv](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/people.csv)
- [employees.csv](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/employees.csv)
- [employees_workshop.csv](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/employees_workshop.csv)

**Week 2 - Customer Segmentation & RFM:**
- [sales_drinks.csv](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/sales_drinks.csv) ⭐ **Main Dataset - 1.8M+ rows**
- [Clients.csv](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/Clients.csv)
- [sales.csv](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/sales.csv)
- [invoices.csv](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/invoices.csv)
- [products.csv](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/products.csv)
- [categories.csv](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/categories.csv)
- [products.json](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/products.json)

**Week 3 - Data Visualization:**
- [bank_transactions.csv](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/bank_transactions.csv)
- [sales_drinks.csv](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/sales_drinks.csv)
- [ventas_completo.csv](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/ventas_completo.csv)

**Week 4 - Data Cleaning:**
- [employees_workshop.csv](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/employees_workshop.csv)
- [marketing_data_clean.csv](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/marketing_data_clean.csv)

### Main Dataset Details

The primary dataset is the **Drinks Sales Dataset**, containing over 1.8 million beverage transactions.

**Also available on Kaggle:**
https://www.kaggle.com/datasets/holaholap/drinks-sales-dataset

**Dataset Features:**
- `invoice_id` - Unique transaction identifier
- `customer_id` - Customer identifier
- `purchase_datetime` - Date and time of purchase
- `sku` - Product SKU
- `quantity` - Items purchased
- `unit_price` - Price per unit
- `discount_pct` - Discount percentage applied
- `amount` - Total transaction amount
- `product_name` - Product description
- `brand` - Brand name
- `category` - Product category

**Additional Datasets:**
- Titanic dataset (via seaborn - no download needed)
- Customer data
- Invoice data
- Product catalogs
- Employee datasets
- Banking transactions
- Marketing campaign data

## How to Use This Repository

### For Students:
1. **Start with Activity notebooks** (empty templates) to practice independently
2. **Refer to Lecture notebooks** for concepts and examples
3. **Compare with Solution notebooks** after attempting exercises
4. **No data download required** - All datasets load automatically from AWS S3
5. **(Optional)** Download datasets locally using the links provided above

### Folder Naming Convention:
- `*_Activity.ipynb` - Empty template for practice
- `*_Solution.ipynb` - Complete solution with explanations
- `Lectures/` - Instructional content
- All datasets load automatically from AWS S3 (see [DATA_SOURCES.md](DATA_SOURCES.md))

### Recommended Learning Path:
1. Week 1: Master Pandas fundamentals
2. Week 2: Learn customer analytics and RFM
3. Week 3: Advanced visualization and analysis techniques
4. Week 4: Data cleaning and preparation best practices

## Technologies Used

- **Python 3.11+**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical data visualization
- **Jupyter Notebook** - Interactive development environment

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/Python-For-Data-Science-Classes.git

# Navigate to the directory
cd Python-For-Data-Science-Classes

# Install required packages
pip install pandas numpy matplotlib seaborn jupyter

# Launch Jupyter Notebook
jupyter notebook
```

**Note:** All datasets load automatically from AWS S3 - no manual data downloads required! Just run the notebooks and start learning.

## Course Outcomes

After completing this course, you will be able to:
- Manipulate and analyze data using Pandas
- Perform comprehensive exploratory data analysis
- Create impactful data visualizations
- Implement customer segmentation strategies
- Apply RFM analysis for customer analytics
- Clean and prepare data for analysis
- Build data-driven insights for business decisions

## Notes

- Each week builds upon previous concepts
- Practice with the empty activity notebooks before viewing solutions
- Datasets are included in respective week Data folders
- Solutions demonstrate best practices and multiple approaches

## License

This repository is for educational purposes. Datasets used are publicly available or synthetically generated for learning.

---

**Happy Learning!** 🎓📊
