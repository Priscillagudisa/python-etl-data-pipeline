# Python ETL Data Pipeline

## Project Overview

This project demonstrates the implementation of an Extract, Transform, Load (ETL) pipeline using Python and pandas.

The pipeline extracts structured data from multiple file formats (CSV, JSON, and XML), combines the records into a pandas DataFrame, transforms height and weight measurements into standardized units, and saves the processed dataset to a CSV file.

This project was developed as part of the IBM Data Engineering learning program.

## Technologies Used

- Python
- pandas
- XML ElementTree
- glob
- datetime
- Jupyter Notebook

## ETL Workflow

**1. Extract**

- Read CSV files using `pd.read_csv()`.
- Read JSON files using `pd.read_json()`.
- Parse XML files using `xml.etree.ElementTree`.
- Combine data from multiple sources using `pd.concat()`.

**2. Transform**

- Convert height from inches to meters.
- Convert weight from pounds to kilograms.
- Round measurements to two decimal places.

**3. Load**

- Export transformed records into `transformed_data.csv`.
- Prepare the output for downstream database integration.

**4. Logging**

- Record timestamps for the start and completion of ETL operations.
- Maintain an execution log for tracking pipeline progress.

## Project Files

| File | Description |
|---|---|
| `etl_code.py` | Python ETL implementation |
| `python_etl_pipeline.ipynb` | Interactive Jupyter Notebook |
| `transformed_data.csv` | Transformed output dataset |
| `requirements.txt` | Python dependencies |

## How to Run

1. Clone or download this repository.
2. Install dependencies:

   `pip install -r requirements.txt`

3. Place the original CSV, JSON, and XML source files in the project directory.
4. Execute the pipeline:

   `python etl_code.py`

5. Review `transformed_data.csv` and `log_file.txt`.

**Note:** The source data files are required to reproduce the ETL pipeline and are not currently included in this repository.

## Skills Demonstrated

Python Programming | ETL Development | Data Extraction | Data Transformation | Data Integration | pandas | Data Processing | Logging

## Future Enhancements

- Implement automated data validation and error handling.
- Integrate PostgreSQL for database loading.
- Automate pipeline execution using Apache Airflow.
- Explore AWS S3 and AWS Glue for cloud-based ETL.

## Acknowledgment

Based on an ETL lab from the IBM Data Engineering learning program, with further improvements planned as part of ongoing Data Engineering practice.
