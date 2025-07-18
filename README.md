# Recipe Recommendation

## Project Overview
This project focuses on extracting features from a large recipe dataset and performing exploratory data analysis (EDA) to support recipe recommendation tasks. The workflow is implemented using PySpark for scalable data processing and includes steps for data cleaning, feature extraction, and statistical analysis.

## Key Components
1. **Feature Extraction (Part 1 & 2):**
   - Reads a raw recipes dataset (CSV format) from an S3 bucket.
   - Ensures correct data types for all columns.
   - Extracts and processes nutritional information into individual features.
   - Handles and transforms other recipe attributes for downstream analysis.

2. **Exploratory Data Analysis (EDA):**
   - Installs and uses libraries such as Plotly, Pandas, Numpy, and Matplotlib for visualization and analysis.
   - Analyzes distributions, quantiles, and relationships between recipe features.
   - Provides custom functions for statistical summaries and visualizations.

## Technologies Used
- PySpark (for distributed data processing)
- Pandas, Numpy, Matplotlib, Plotly (for EDA and visualization)
- Jupyter Notebooks (for interactive development)

## Data Source
- The main dataset is a cleaned CSV file of recipes, loaded from an S3 bucket:
  `s3://aws-emr-studio-735706911732-us-east-1/RAW_recipes_cleaned.csv`

## How to Run
- Open the Jupyter notebooks in order:
  1. `01_FeatureExtractionPart01-TemplateV4.0.ipynb`
  2. `03_FeatureExtractionPart02-CompleteSolution.ipynb`
  3. `02_EDA-CompleteSolution.ipynb`
- Ensure you have access to a Spark environment and the required Python libraries.
- Follow the instructions and complete the tasks in each notebook.

## Outputs
- Cleaned and feature-enriched recipe dataframes.
- Visualizations and statistical summaries of recipe features.

## Note
You may need AWS credentials and appropriate permissions to access the S3 data source.
