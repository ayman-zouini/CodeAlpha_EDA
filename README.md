# Titanic Dataset - Exploratory Data Analysis (EDA)

## 📊 Project Overview

This project performs a comprehensive **Exploratory Data Analysis (EDA)** on the famous Titanic dataset to uncover insights about passenger survival patterns during the tragic 1912 disaster. Through statistical analysis and data visualization, we explore the factors that influenced survival rates and validate historical accounts of the "women and children first" evacuation protocol.

## 🎯 Objectives

- Analyze passenger survival patterns and identify key factors
- Explore relationships between demographics and survival rates  
- Validate historical assumptions about the Titanic disaster
- Detect data quality issues and anomalies
- Generate actionable insights through statistical testing and visualization

## 📁 Project Structure

```
CodeAlpha_EDA/
│
├── data/
│   └── titanic.csv              # Raw Titanic dataset
│
├── notebooks/
│   └── EDA_Titanic.ipynb        # Main analysis notebook
│
├── requirements.txt             # Python dependencies
├── README.md                    # Project documentation
└── .gitignore                   # Git ignore file
```

## 📈 Dataset Information

**Source**: Classic Titanic passenger dataset  
**Records**: 891 passengers  
**Features**: 8 columns including:

| Column | Description | Type |
|--------|-------------|------|
| Survived | Survival status (0=No, 1=Yes) | Binary |
| Pclass | Passenger class (1st, 2nd, 3rd) | Categorical |
| Name | Passenger name | Text |
| Sex | Gender | Categorical |
| Age | Age in years | Numerical |
| Siblings/Spouses Aboard | Number of siblings/spouses | Numerical |
| Parents/Children Aboard | Number of parents/children | Numerical |
| Fare | Ticket price in dollars | Numerical |

## 🔍 Key Analysis Steps

### 1. **Data Structure Exploration**
- Dataset dimensions and data types
- Missing values analysis and visualization
- Descriptive statistics for all variables

### 2. **Survival Analysis**
- Overall survival rate calculation
- Survival patterns by demographics
- Statistical significance testing

### 3. **Feature Engineering**
- Title extraction from passenger names
- Family size calculation
- Passenger categorization (alone vs. with family)

### 4. **Statistical Analysis**
- Correlation matrix analysis
- Cross-tabulation and chi-square tests
- Anomaly detection using IQR method

### 5. **Data Visualization**
- Distribution plots and histograms
- Survival heatmaps and cross-analysis
- Boxplots for outlier identification

## 🎯 Key Findings

### 📊 **Survival Statistics**
- **Overall survival rate**: 38% (342 out of 891 passengers)
- **Gender impact**: Women had 3.9x better survival chances
  - Female survival: 74%
  - Male survival: 19%

### 🏛️ **Class Analysis**
| Class | Survival Rate | Key Insights |
|-------|--------------|--------------|
| 1st Class | 63% | Highest survival rate, access to lifeboats |
| 2nd Class | 47% | Moderate survival rate |
| 3rd Class | 24% | Lowest survival rate, deck access limitations |

### 👶 **Age Factors**
- **Children (<16 years)**: 58% survival rate
- **Adults**: Lower survival rates, especially men
- **Elderly passengers**: Some outliers detected (70+ years)

### 👨‍👩‍👧‍👦 **Family Impact**
- **Passengers with family**: 45% survival rate
- **Solo travelers**: 30% survival rate
- **Optimal family size**: 2-3 members had highest survival rates

## 🔬 Data Quality Assessment

### Missing Values
- **Age**: ~20% missing values (177 passengers)
- **Other columns**: Complete data available

### Anomalies Detected
- **Fare outliers**: Some passengers paid >$500 (luxury suites)
- **Free tickets**: Several passengers with $0 fare (likely crew)
- **Age extremes**: Passengers over 70 years old

## 📋 Requirements

```
pandas>=1.3.0
numpy>=1.21.0
matplotlib>=3.4.0
seaborn>=0.11.0
jupyter>=1.0.0
```

## 🚀 How to Run

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd CodeAlpha_EDA
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook notebooks/EDA_Titanic.ipynb
   ```

4. **Run all cells** to reproduce the complete analysis

## 📊 Visualizations Included

- **Survival distribution** (bar charts and pie charts)
- **Demographic analysis** (gender, age, class breakdowns)
- **Correlation heatmaps** for numerical variables
- **Missing values visualization**
- **Family size impact analysis**
- **Fare distribution and outlier detection**
- **Cross-analysis charts** (multi-variable relationships)

## 🎓 Historical Validation

The analysis confirms several historical aspects of the Titanic disaster:

✅ **"Women and children first" protocol** clearly implemented  
✅ **Class-based evacuation** - higher classes had priority  
✅ **Social status impact** - titles reflect survival patterns  
✅ **Age discrimination** - children prioritized over adults  

## 🔮 Future Enhancements

- [ ] Machine learning model development for survival prediction
- [ ] Advanced feature engineering (cabin location, embarkation port)
- [ ] Interactive dashboard creation with Plotly/Streamlit
- [ ] Comparison with other maritime disasters
- [ ] Text analysis of passenger names and origins

## 📝 Methodology

This EDA follows a systematic approach:

1. **Question formulation** before analysis
2. **Data structure exploration** and profiling  
3. **Hypothesis generation** and testing
4. **Pattern identification** through visualization
5. **Statistical validation** of findings
6. **Insight synthesis** and reporting

## 🤝 Contributing

Feel free to fork this project and submit pull requests for improvements such as:
- Additional visualizations
- Statistical tests
- Data preprocessing techniques
- Documentation enhancements

## 👨‍💻 Author

**ZOUINI Ayman**  
📧 Email: zouiniayman321@gmail.com  
💼 Data Analytics

## 📧 Contact

For questions or suggestions about this analysis, please feel free to:
- Open an issue in the repository
- Contact me directly at: zouiniayman321@gmail.com

---

**Dataset Source**: The Titanic dataset is publicly available and commonly used for data science education and practice.

**Analysis Date**: August 2025  
**Author**: ZOUINI Ayman  
**Tools Used**: Python, Pandas, numpy, Matplotlib, Seaborn, Jupyter Notebook
