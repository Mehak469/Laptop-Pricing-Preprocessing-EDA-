# 💻 Laptop Pricing – Data Preprocessing Project

A basic data preprocessing project that demonstrates essential data wrangling techniques using Python on a laptop pricing dataset.

## 📌 Overview
This project focuses on cleaning and preparing raw data for analysis or machine learning by handling missing values, standardizing units, normalizing features, and creating new variables.


## ✨ Features

- **Missing Value Imputation**: Handles missing values using mode (for categorical-like continuous variables) and mean (for continuous variables)
- **Unit Standardization**: Converts measurements to commonly used units (inches for screen size, pounds for weight)
- **Data Normalization**: Normalizes CPU frequency to a 0-1 scale
- **Binning**: Creates categorical price ranges (Low, Medium, High)
- **Feature Engineering**: Creates indicator variables from categorical features
- **Data Visualization**: Includes visualizations for price distribution

## 📊 Dataset

### Input Dataset
- **File**: `laptop_pricing_dataset.csv`
- **Records**: 238 laptops
- **Original Columns**: 13 columns including manufacturer, category, screen type, GPU, OS, CPU specs, screen size, RAM, storage, weight, and price


### Dataset Attributes
- `Manufacturer`: Laptop brand (Acer, Dell, HP, Lenovo, Toshiba, etc.)
- `Category`: Laptop category code
- `Screen`: Screen type (Full HD, IPS Panel)
- `GPU`: Graphics processing unit code
- `OS`: Operating system code
- `CPU_core`: Number of CPU cores
- `Screen_Size_cm`: Screen size in centimeters
- `CPU_frequency`: CPU frequency in GHz
- `RAM_GB`: RAM in gigabytes
- `Storage_GB_SSD`: SSD storage in gigabytes
- `Weight_kg`: Weight in kilograms
- `Price`: Price in local currency

## 🔧 Techniques Used

### 1. Data Cleaning
- **Removed unnecessary columns**: Dropped duplicate index column
- **Rounded values**: Standardized decimal precision
- **Missing value imputation**:
  - Screen Size: Imputed with mode (most common value)
  - Weight: Imputed with mean value

### 2. Unit Conversion
- Screen size: Centimeters → Inches (division by 2.54)
- Weight: Kilograms → Pounds (multiplication by 2.205)

### 3. Data Normalization
- CPU Frequency: Normalized to 0-1 range (divided by maximum value)

### 4. Binning
- Price: Converted continuous values to categorical bins (Low, Medium, High) using equal-width binning

### 5. Feature Engineering
- Created indicator variables (dummy variables) for Screen type:
  - `Screen_Full_HD`: Binary indicator for Full HD screens
  - `Screen_IPS_Panel`: Binary indicator for IPS Panel screens

## 📁 Project Structure

```
github_project/
│
├── cleaning.ipynb                    # Main Jupyter notebook with data wrangling code
├── laptop_pricing_dataset_mod1.csv   # Raw input dataset
├── Wraggled_Laptops_Data.csv         # Cleaned output dataset
├── requirements.txt                  # Python package dependencies
└── README.md                         # Project documentation (this file)
```

## 🚀 Installation

### Prerequisites
- Python 3.7 or higher
- Jupyter Notebook or JupyterLab

### Setup

1. **Clone or download this repository**

2. **Create a virtual environment (recommended)**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install required packages**
   ```bash
   pip install -r requirements.txt
   ```

## 💻 Usage

1. **Open Jupyter Notebook**
   ```bash
   jupyter notebook cleaning.ipynb
   ```

2. **Run all cells** (or run cells sequentially):
   - The notebook will load the raw dataset
   - Perform all data wrangling operations
   - Generate visualizations
   - Export the cleaned dataset

3. **Output**
   - The cleaned dataset will be saved as `Wraggled_Laptops_Data.csv`
   - All transformations are documented in the notebook cells


## 📤 Output

The cleaned dataset (`Wraggled_Laptops_Data.csv`) contains:

- **238 rows** (all records preserved)
- **14 columns**:
  - Original columns (with standardized units and names)
  - `Price_Binned`: Categorical price ranges (Low, Medium, High)
  - `Screen_Full_HD`: Binary indicator (0 or 1)
  - `Screen_IPS_Panel`: Binary indicator (0 or 1)
- **No missing values**
- **Standardized units**: Screen size in inches, weight in pounds
- **Normalized features**: CPU frequency normalized to 0-1 range

## 🛠 Technologies Used

- **Python 3.x**: Programming language
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical operations
- **Matplotlib**: Data visualization
- **Jupyter Notebook**: Interactive development environment

## 📚 Key Learnings

This project demonstrates:
- Best practices in data cleaning and preprocessing
- Appropriate handling of missing values
- Unit conversion and standardization
- Feature engineering techniques
- Data transformation workflows
- Documentation and code organization


**Note**: This project is intended for educational purposes to demonstrate data wrangling techniques. The dataset used is a sample dataset for learning purposes.So,suggestions and improvements are welcome!


