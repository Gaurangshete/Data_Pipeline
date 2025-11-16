Automated ETL Data Pipeline
Objective:
Create a Python-based automated pipeline for Extract, Transform, Load (ETL) operations to preprocess data for machine learning workflows.
Key Requirements:
1. Extract (Data Loading)

Support multiple data sources: CSV, Excel, JSON, Parquet, SQL databases
Handle various file formats and configurations
Log extraction metrics (rows, columns)

2. Transform (Data Preprocessing)

Cleaning:

Remove duplicate records
Handle missing values (multiple strategies: mean, median, mode, forward fill, drop)
Drop columns with excessive missing data (configurable threshold)

Feature Engineering:

Scale numeric features (StandardScaler, MinMaxScaler)
Encode categorical features (One-Hot Encoding, Label Encoding)
Auto-detect feature types

Data Splitting:

Split into training and testing sets
Support stratified splitting for classification tasks
Configurable test size and random state

3. Load (Data Export)

Export processed data to multiple formats (CSV, Parquet, Excel, JSON)
Save training and testing splits separately
Generate metadata file documenting all transformations
Track pipeline execution history

Technical Stack:

Pandas: Data manipulation and I/O operations
Scikit-learn: Preprocessing transformers, scaling, encoding, splitting
NumPy: Numerical operations
Python Standard Library: Logging, JSON handling, datetime tracking

Deliverable:
A complete Python script/Jupyter notebook that automates the entire ETL process with:

Modular, reusable DataPipeline class
Step-by-step execution capability
Configuration-based pipeline execution
Comprehensive logging and error handling
Metadata tracking for reproducibility
Example usage with sample dataset
