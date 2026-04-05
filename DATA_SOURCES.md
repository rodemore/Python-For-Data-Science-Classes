# Dataset Sources

All datasets for this course are hosted on AWS S3 for easy, cloud-based access.

## 🚀 Quick Start

All notebooks are pre-configured to load data directly from S3. No downloads required!

```python
# Example usage in any notebook
import pandas as pd

# Load data directly from S3
url = 'https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/sales_drinks.csv'
df = pd.read_csv(url)
```

## 📦 Complete Dataset List

### Base URL
```
https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/
```

### Week 1 - Introduction to Pandas & EDA

| File Name | Size | Direct Link |
|-----------|------|-------------|
| `people.csv` | Small | [Download](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/people.csv) |
| `employees.csv` | Small | [Download](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/employees.csv) |
| `employees_workshop.csv` | Small | [Download](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/employees_workshop.csv) |

**Usage in notebooks:**
```python
df = pd.read_csv('https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/employees_workshop.csv')
```

---

### Week 2 - Customer Segmentation & RFM Analysis

| File Name | Size | Description | Direct Link |
|-----------|------|-------------|-------------|
| `sales_drinks.csv` | 251 MB | **Main dataset** - 1.8M+ transactions | [Download](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/sales_drinks.csv) |
| `Clients.csv` | Small | Customer information | [Download](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/Clients.csv) |
| `sales.csv` | 97 MB | Sales transactions | [Download](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/sales.csv) |
| `invoices.csv` | 13 MB | Invoice details | [Download](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/invoices.csv) |
| `products.csv` | Small | Product catalog | [Download](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/products.csv) |
| `categories.csv` | Small | Product categories | [Download](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/categories.csv) |
| `products.json` | Small | Products in JSON format | [Download](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/products.json) |

**Usage in notebooks:**
```python
# Load main dataset
df = pd.read_csv('https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/sales_drinks.csv')

# Load multiple datasets for RFM homework
base_url = 'https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/'
clients = pd.read_csv(base_url + 'Clients.csv')
sales = pd.read_csv(base_url + 'sales.csv')
invoices = pd.read_csv(base_url + 'invoices.csv')
products = pd.read_csv(base_url + 'products.csv')
```

---

### Week 3 - Data Visualization & Advanced Analysis

| File Name | Size | Description | Direct Link |
|-----------|------|-------------|-------------|
| `bank_transactions.csv` | Medium | Banking transaction data | [Download](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/bank_transactions.csv) |
| `sales_drinks.csv` | 251 MB | Beverage sales data | [Download](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/sales_drinks.csv) |
| `ventas_completo.csv` | 252 MB | Complete sales dataset | [Download](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/ventas_completo.csv) |

**Usage in notebooks:**
```python
df = pd.read_csv('https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/bank_transactions.csv')
```

---

### Week 4 - Data Cleaning & Missing Values

| File Name | Size | Description | Direct Link |
|-----------|------|-------------|-------------|
| `employees_workshop.csv` | Small | Employee data for cleaning practice | [Download](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/employees_workshop.csv) |
| `marketing_data_clean.csv` | Medium | Cleaned marketing dataset | [Download](https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/marketing_data_clean.csv) |

**Usage in notebooks:**
```python
df = pd.read_csv('https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/marketing_data_clean.csv')
```

---

## 📥 Alternative Data Source

The main **Drinks Sales Dataset** is also available on Kaggle:
- **Kaggle URL**: https://www.kaggle.com/datasets/holaholap/drinks-sales-dataset

---

## 💡 Tips for Working with Cloud Data

### Reading from S3
```python
import pandas as pd

# Direct URL approach (recommended)
url = 'https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/sales_drinks.csv'
df = pd.read_csv(url)
```

### Download Locally (Optional)
If you prefer to work with local files:

```python
import pandas as pd
import requests

# Download file
url = 'https://mysiterobert.s3.us-east-1.amazonaws.com/Dataframes/sales_drinks.csv'
response = requests.get(url)

# Save locally
with open('sales_drinks.csv', 'wb') as f:
    f.write(response.content)

# Read from local file
df = pd.read_csv('sales_drinks.csv')
```

Or simply click the download links above to save files to your computer.

---

## 🔍 Data Quality

All datasets have been:
- ✅ Cleaned and validated
- ✅ Formatted for educational use
- ✅ Optimized for performance
- ✅ Tested with all course notebooks

---

## 🆘 Troubleshooting

**Issue: "Unable to load data from URL"**
- Check your internet connection
- Verify the URL is correct
- Try downloading the file locally and reading from disk

**Issue: "File too large to load"**
- Use `nrows` parameter to load a subset: `pd.read_csv(url, nrows=10000)`
- Increase your system's available memory
- Use chunking for large files

**Issue: "SSL Certificate Error"**
```python
# Add this before reading
import ssl
ssl._create_default_https_context = ssl._create_unverified_context

df = pd.read_csv(url)
```

---

## 📞 Questions?

If you encounter any issues accessing the datasets, please open an issue in the GitHub repository.

**Happy Learning!** 🎓📊
