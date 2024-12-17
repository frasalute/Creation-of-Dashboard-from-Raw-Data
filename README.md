# Creation of Dashboard from Raw Data

(Done in a university setting as project part of a Data Management and Visualization class together with other three students.)

This repository contains Python scripts for **data cleaning, preprocessing, exploratory data analysis (EDA)**, and **dashboard creation** using Airbnb listing data. The project integrates **PostgreSQL** for scalable data storage and **Python** for analysis and visualization.

---

## **Project Overview**

The project focuses on building an **interactive dashboard** to analyze Airbnb guest preferences and provide actionable insights. Key tasks include:

1. **Data Cleaning**: Preparing raw data by handling missing values, transforming attributes, and eliminating redundancies.  
2. **Data Export to SQL**: Storing cleaned data in PostgreSQL relational tables for scalability.  
3. **Exploratory Data Analysis (EDA)**: Conducting correlation analysis and visualizing pricing, host performance, and location-based trends.  
4. **Dashboard Design**: Creating tailored visualizations for management, focusing on guest satisfaction, pricing, and availability.

---

## **Tech Stack**

- **Programming Language**: Python  
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Missingno, SQLAlchemy  
- **Database**: PostgreSQL  
- **Environment**: Google Colab  

---

## **How to Run the Project**

### **1. Clone the Repository**
```bash
git clone https://github.com/yourusername/Creation-of-Dashboard-from-Raw-Data.git
cd Creation-of-Dashboard-from-Raw-Data
```

### **2. Set Up the Environment**
Ensure Python 3.7+ is installed, and install required libraries:

```bash
pip install -r requirements.txt
```

### **3. Connect to PostgreSQL**
Update your database credentials in the `export_to_sql.py` script:

```python
DATABASE = {
    'user': 'your_username',
    'password': 'your_password',
    'host': 'localhost',
    'port': '5432',
    'database': 'airbnb_data'
}
```

### **4. Run the Scripts**
**Data Cleaning and Preprocessing:**
```bash
python data_cleaning.py
```

**Export to PostgreSQL:**
```bash
python export_to_sql.py
```

**Exploratory Data Analysis:**
```bash
python exploratory_analysis.py
```

---

## **Folder Structure**
```plaintext
Creation-of-Dashboard-from-Raw-Data/
│
├── data_cleaning.py             # Data cleaning and preprocessing script
├── export_to_sql.py             # Script for exporting data to PostgreSQL
├── exploratory_analysis.py      # Exploratory Data Analysis (EDA) script
├── requirements.txt             # Python libraries required
├── Dashboard.ipynb              # Jupyter Notebook for dashboard creation
├── raw_data/                    # Folder containing raw Airbnb dataset
└── README.md                    # Project documentation
```

---

## **Key Features**

- **Interactive Dashboard**: Visualizations for quick decision-making.  
- **Data Scalability**: Integration with PostgreSQL for relational data storage.  
- **Custom Features**: Derived attributes (e.g., binary amenities) for better insights.  

---

## **Results**

- Improved understanding of Airbnb guest preferences through EDA.  
- Enhanced management decision-making via a streamlined dashboard.