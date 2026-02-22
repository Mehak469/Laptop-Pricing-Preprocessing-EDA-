### Laptop Pricing(EDA)

A comprehensive exploratory data analysis project examining the factors that influence laptop pricing. This project uses statistical analysis and data visualization to identify key features that drive laptop prices.

###  Project Overview

This EDA project analyzes a dataset of 238 laptops to understand:
- Which features most significantly impact laptop pricing
- The relationship between technical specifications and price
- Statistical significance of various factors
- Market trends and pricing patterns

###  Dataset Information

- **Total Records**: 238 laptops
- **Features Analyzed**: 10 features
- **Price Range**: $527 - $3,810
- **Average Price**: $1,462 (Median: $1,333)

###  Key Findings

### Top Price Drivers (Statistically Significant)
1. **RAM (GB)** - Correlation: 0.549 (p<0.001) - **Most Important Factor**
2. **CPU Cores** - Correlation: 0.459 (p<0.001) - **Second Most Important**
3. **CPU Frequency** - Correlation: 0.367 (p<0.001) - **Third Most Important**

### Moderate Price Influencers
- **GPU Type** - Correlation: 0.288 (p<0.001)
- **Category** - Correlation: 0.286 (p<0.001)
- **Storage SSD** - Correlation: 0.243 (p<0.001)

### Weak/Non-Significant Factors
- **Screen Size** - Correlation: -0.111 (p=0.089) - Not statistically significant
- **Weight** - Correlation: -0.050 (p=0.440) - Not significant
- **OS** - Correlation: -0.222 (p<0.001) - Weak negative correlation

##  Technologies Used

- **Python 3.13.5**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib** - Basic plotting
- **Seaborn** - Statistical visualizations
- **SciPy** - Statistical tests and analysis
- **Jupyter Notebook** - Interactive development environment

**Note**: Make sure to update the file path in the notebook to point to your data file location.

