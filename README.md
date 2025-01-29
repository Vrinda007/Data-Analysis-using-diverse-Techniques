# Data Analysis on Socioeconomic Data Using Diverse Technologies

## Project Overview
This project focuses on integrating and analyzing socioeconomic data from multiple sources using advanced data processing and visualization technologies. The primary goal is to uncover hidden patterns that influence loan approvals and demographic trends in India. The project employs Python along with MongoDB, PostgreSQL, and Dagster to process structured and semi-structured datasets effectively.

## Datasets
The project utilizes two datasets acquired from Kaggle:
1. **Loan Risk Dataset** (Semi-structured JSON):
   - Contains profiles of professionals with loan risk tags.
   - Includes attributes like income, age, experience, marital status, home/car ownership, profession, and location data.
   - Comprises ~252,000 records.
2. **Pan-India Demographic Dataset** (Structured CSV):
   - Provides demographic information such as age, gender, education, employment status, and income levels.
   - Contains over 10,000 individual records.

## Research Objectives
- Identifying high-paying professions and their spending patterns.
- Analyzing income vs. expenditure across states.
- Examining demographic-based spending behavior.
- Understanding asset ownership trends in relation to income levels.

## Technologies Used
- **MongoDB**: For handling semi-structured data efficiently.
- **PostgreSQL**: For structured data management and querying.
- **Dagster**: For building and managing ETL workflows.
- **Python**: Primary language for data processing, analysis, and visualization.
  - **Pandas, NumPy, Scikit-learn**: Data manipulation and statistical analysis.
  - **Matplotlib, Seaborn**: Data visualization.
  - **Dash, Plotly**: Interactive dashboards.

## Data Processing Pipeline
1. **Data Ingestion**:
   - JSON data is loaded into MongoDB using PyMongo.
   - CSV data is stored in PostgreSQL using SQLAlchemy.
2. **Data Transformation**:
   - ETL pipeline built with Dagster to clean and structure data.
   - Exploratory Data Analysis (EDA) performed to identify missing values, duplicates, and outliers.
3. **Data Analysis & Insights**:
   - Statistical modeling and visualizations to uncover patterns.
   - Comparative analysis between income groups and their spending behaviors.
4. **Visualization & Dashboard**:
   - Dynamic charts and graphs to showcase key findings.
   - Interactive dashboard built with Dash and Plotly.

## Key Insights
- High-income professionals (e.g., Petroleum Engineers, Psychologists) have significant asset ownership.
- Younger individuals (19-25) spend more on fashion, while older groups focus on healthcare and travel.
- States like Maharashtra and Uttar Pradesh show strong income-to-asset correlations.
- Delhi, Himachal Pradesh, and Jammu & Kashmir have the highest consumer spending.

## Limitations & Future Work
### Limitations
- Data accuracy depends on the sources and completeness of datasets.
- Static datasets may not reflect real-time socioeconomic shifts.

### Future Enhancements
- Integration of additional variables (education levels, employment types) for deeper insights.
- Implementation of machine learning models for predictive analysis.
- Expansion to real-time data updates for better decision-making.

## Setup & Execution
### Prerequisites
- Python 3.x
- MongoDB
- PostgreSQL
- Required Python libraries: Install using `pip install -r requirements.txt`

### Running the Project
1. Clone the repository: `git clone <repo-url>`
2. Set up databases:
   - Start MongoDB and PostgreSQL servers.
   - Import JSON data into MongoDB.
   - Load CSV data into PostgreSQL.
3. Run data processing scripts:
   ```sh
   python data_processing.py
   ```
4. Start the interactive dashboard:
   ```sh
   python dashboard.py
   ```


