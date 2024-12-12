
# Project Overview

This project aims to perform **data analysis**, **statistical interpretation**, and **visualization** on 10 years of demographic data (births, deaths, marriages, divorces, etc.) provided by Statistics Korea. Through this process, we seek to identify domestic population trends, social changes, and derive meaningful insights from the data.

## Collaborators
- **fueguito03**: Data preprocessing and project management
- **Roh37Chef**: Exploratory Data Analysis
- **rrrtyi**: Regression Analysis and visualization

## Main Objectives

- **Data Preprocessing**: Transform the raw data into a more manageable format  
- **Exploratory Data Analysis (EDA)**: Understand the dataset through basic statistical measures and visualizations  
- **Statistical Analysis**: Identify population change trends, correlations, and perform relevant statistical interpretations  
- **Visualization**: Utilize Matplotlib to visualize trends and patterns in demographic changes for easier understanding

## Data Used

- **Data Source**:  
  - Statistics Korea, "Vital Statistics Survey," 2023, 2024.12.11, Trends in the Number and Rates of Vital Events (Births, Deaths, Marriages, Divorces)  
  - Link: [KOSIS National Statistics Portal](https://kosis.kr/statHtml/statHtml.do?orgId=101&tblId=DT_1B8000F&conn_path=I2)
  - https://for-my-wealthy-life.tistory.com/8 (For Regression Learning)
  - https://giveme-happyending.tistory.com/168 (Korean font matplotlib)
- **Data Overview**: 10 years of demographic data, including birth rates, death rates, marriage rates, and divorce rates  
- **Data Format**: CSV files stored in the `data/` directory

## Technologies & Libraries

- **Language**: Python 3.12.1  
- **Libraries**:
  - **NumPy**: Numerical computations and array operations  
  - **Pandas**: Dataframe-based data manipulation and exploration  
  - **Matplotlib**: Data visualization
  - **Statsmodels**: Statistical modeling and regression analysis

## Directory Structure

```plaintext
project-root/
├─ data/                                  # Original and preprocessed data files
│  ├─ population_trends_cleaned.csv       # Cleaned and processed dataset for analysis
│  └─ 인구동태건수_및_동태율_추이_출생_사망_혼인_이혼__.xlsx  # Raw demographic data
│
├─ results/                               # Analysis results and visualizations
│  ├─ Trends_in_Population_Dynamic.png    # Line chart showing population trends
│  ├─ regression_analysis_results1.png   # Regression analysis result visualization 1
│  └─ regression_analysis_results2.png   # Regression analysis result visualization 2
│
├─ data_processing.ipynb                  # Data preprocessing steps
├─ eda.ipynb                              # Exploratory Data Analysis (EDA)
├─ regression_analysis.ipynb              # Regression analysis and modeling
└─ README.md                              # Project overview and documentation

```

## Exploratory Data Analysis (EDA)

The Exploratory Data Analysis (EDA) was conducted to gain insights into the population trends, focusing on key variables such as birth counts, death counts, and natural population growth.

### Key Findings
1. **Birth Counts**:
   - Birth counts show a consistent decline over the years, with a notable decrease starting from 2015.
   - The rate of decline appears to accelerate in more recent years.

2. **Death Counts**:
   - Death counts have steadily increased over the years, likely due to aging population demographics.
   - The increase in death counts correlates with the decreasing natural population growth.

3. **Natural Population Growth**:
   - Natural population growth (births - deaths) has shifted from positive to negative in recent years.
   - This transition highlights the growing issue of population decline.

4. **Outliers**:
   - No significant outliers were detected in the data; trends were consistent over time.

### Visualizations
1. **Line Charts**:
   - Birth counts, death counts, and natural population growth were plotted over time to visualize their trends.

   ![Trends in Population Dynamic](https://github.com/fueguito03/Population-Trends-Analysis/blob/main/results/Trends_in_Population_Dynamic.png)

## How to Run

-**1. Set up the enviroment**: install the required libraries using requirements.txt.

pip install -r requirements.txt

-**2. Check the data**: Ensure that the target CSV file is available in the data/ directory.

-**3. Run the notebooks**: Launch the Jupyter Notebooks in the notebooks/ directory to proceed with preprocessing, EDA, modeling, and any additional steps.

jupyter notebook

Open the desired .ipynb file in your browser and execute the cells in order.

-**4. View the results**: Check the results/ directory for generated charts, graphs, and summary metrics.

## Results

### Regression Analysis Results

Below are the results of the regression analysis conducted as part of this project. The analysis examines the relationship between various factors influencing population trends.

#### Linear Regression Result
![Regression Analysis Result 1](https://github.com/fueguito03/Population-Trends-Analysis/blob/main/results/regression_analysis_results1.png)

#### Linear Regression Visualisation
![Regression Analysis Result 2](https://github.com/fueguito03/Population-Trends-Analysis/blob/main/results/regression_analysis_results2.png)

### Model Summary
- **Dependent Variable**: Birth counts
- **Independent Variable**: Year

### Key Results
1. **R-squared**: 0.966 (96.6%)
   - The model explains 96.6% of the variation in birth counts.
2. **Regression Coefficients**:
   - Intercept (const): 51,490,000
   - Slope (Year): -25,350
3. **Statistical Significance**:
   - The p-value for the independent variable (Year) is < 0.001, indicating a statistically significant relationship.

### Interpretation
- Birth counts have shown a decreasing trend over the years.
- Each year, birth counts are predicted to decrease by approximately 25,350.
- This trend highlights the ongoing issue of declining birth rates, which may be influenced by social and economic factors.
