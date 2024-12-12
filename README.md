
# Project Overview

This project aims to perform **data analysis**, **statistical interpretation**, and **visualization** on 10 years of demographic data (births, deaths, marriages, divorces, etc.) provided by Statistics Korea. Through this process, we seek to identify domestic population trends, social changes, and derive meaningful insights from the data.

## Main Objectives

- **Data Preprocessing**: Transform the raw data into a more manageable format  
- **Exploratory Data Analysis (EDA)**: Understand the dataset through basic statistical measures and visualizations  
- **Statistical Analysis**: Identify population change trends, correlations, and perform relevant statistical interpretations  
- **Visualization**: Utilize Matplotlib to visualize trends and patterns in demographic changes for easier understanding

## Data Used

- **Data Source**:  
  - Statistics Korea, "Vital Statistics Survey," 2023, 2024.12.11, Trends in the Number and Rates of Vital Events (Births, Deaths, Marriages, Divorces)  
  - Link: [KOSIS National Statistics Portal](https://kosis.kr/statHtml/statHtml.do?orgId=101&tblId=DT_1B8000F&conn_path=I2)
- **Data Overview**: 10 years of demographic data, including birth rates, death rates, marriage rates, and divorce rates  
- **Data Format**: CSV files stored in the `data/` directory

## Technologies & Libraries

- **Language**: Python 3.x  
- **Libraries**:
  - **NumPy**: Numerical computations and array operations  
  - **Pandas**: Dataframe-based data manipulation and exploration  
  - **Matplotlib**: Data visualization  
- **Environment**: Before running the project, install the required libraries listed in `requirements.txt`

## Directory Structure

```plaintext
project-root/
├─ data/                      # Original and preprocessed data files
│  └─ population_data.csv     # Example: 10-year demographic data from Statistics Korea
│
├─ notebooks/                 # Jupyter Notebooks
│  ├─ data_preprocessing.ipynb   # Data preprocessing
│  ├─ eda.ipynb                  # Exploratory Data Analysis (EDA)
│  ├─ modeling.ipynb             # Modeling and evaluation (if needed)
│  └─ final_analysis.ipynb       # Final summary of analysis results
│
├─ src/                       # Python scripts
│  ├─ preprocess.py           # Data preprocessing functions
│  ├─ model.py                # Modeling functions (if needed)
│  └─ evaluate.py             # Model evaluation functions (if needed)
│
├─ results/                   # Output files (visualizations, metrics, etc.)
│  ├─ figures/                # Graphs and charts
│  └─ metrics.txt             # Summary of statistical results and key indicators
│
├─ README.md                  # Project overview and documentation
└─ requirements.txt           # Required libraries

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

#### Result 1
![Regression Analysis Result 1](https://github.com/fueguito03/Population-Trends-Analysis/blob/main/results/regression_analysis_results1.png)

#### Result 2
![Regression Analysis Result 2](https://github.com/fueguito03/Population-Trends-Analysis/blob/main/results/regression_analysis_results2.png)

These charts illustrate the key outcomes and statistical relationships identified during the regression analysis. For further details, refer to the documentation or code files in this repository.

## License

The project’s results and source code follow a separate licensing policy (specify if needed).

## Contact

For project-related inquiries, please use the GitHub Issues tab.

