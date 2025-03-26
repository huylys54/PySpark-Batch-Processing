# PySpark Batch Processing - Learning and Practice

This repository contains PySpark notebooks and scripts for learning and practicing batch processing concepts. The focus is on working with large datasets, performing transformations, and generating insights using PySpark.
Note: Some of the notebooks already have download cells so you don't need to download all the datas by yourself :)
## Folder Structure

```
PySpark_Practice
├─ data/
├─ lib
│  └─ gcs-connector-hadoop3-latest.jar
├─ notebooks
│  ├─ pyspark_dataframe.ipynb
│  ├─ pyspark_test.ipynb
│  ├─ spark_gcp.ipynb
│  ├─ spark_groupby_join.ipynb
│  ├─ spark_rdd.ipynb
│  ├─ spark_sql.ipynb
│  ├─ spark_sql_localcluster.ipynb
│  └─ taxi_schema.ipynb
├─ README.md
├─ scripts
│  ├─ download_data.sh
│  └─ spark_sql_localcluster.py
```

### Key Components

- **notebooks/**: Contains Jupyter notebooks for hands-on PySpark practice, covering various topics like schema definitions, joins, aggregations, and RDD transformations.
- **data/**: Stores input and output datasets, including Parquet files and reports generated during processing.
- **scripts/**: Contains Bash script for downloading data and Python script for revenue calculations and writes results to Parquet.

---

## Prerequisites

To run the notebooks and scripts, ensure you have the following installed:

- Python 3.8+
- Apache Spark (3.x recommended)
- Jupyter Notebook
- Required Python libraries (see [Installation](#installation))

---

## Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/huylys54/PySpark_Practice.git
   cd PySpark_Practice
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Set up PySpark:

   - Download and install Apache Spark from [Spark Downloads](https://spark.apache.org/downloads.html).
   - Set the `SPARK_HOME` environment variable and add it to your `PATH`.

4. Start Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

---

## Usage

### Notebooks

- **`taxi_schema.ipynb`**: Defines schemas for green and yellow taxi datasets and processes data iteratively by month.
- **`spark_groupby_join.ipynb`**: Performs joins and aggregations on green and yellow taxi revenue data.
- **`spark_sql_localcluster.ipynb`**: Uses Spark SQL for revenue calculations and writes results to Parquet.
- **`spark_rdd.ipynb`**: Demonstrates RDD-based transformations for revenue calculations.
- **`pyspark_dataframe.ipynb`**: Explores DataFrame operations and schema definitions.
- **`spark_gcp.ipynb`**: Configures Spark to work with Google Cloud Storage and processes data stored in GCS.
- **`pyspark_test.ipynb`**: Contains test code for loading and processing smaller datasets.

### Data

- Input data is expected in the `data/` folder, organized by type (e.g., `pq/green/`, `pq/yellow/`).
- Processed data and reports are written to `data/report/revenue/`.

---

## Topics Covered

- PySpark Basics
- DataFrames and Transformations
- Batch Processing with PySpark
- Working with Parquet, CSV, and JSON files
- Aggregations and Joins
- RDD Transformations
- Spark SQL
- Google Cloud Storage Integration
- Performance Optimization

---

## Troubleshooting

- **Missing Input Files**: Ensure the required datasets are placed in the `data/` folder.
- **Schema Mismatches**: Verify that the schemas for green and yellow taxi datasets are consistent.
- **Performance Issues**: Use repartitioning and caching to optimize large dataset processing.

---


## License

This project is licensed under the MIT License.

---

## Acknowledgments

This repository is part of the **DE Zoomcamp** program. Special thanks to the instructors and contributors for their guidance and resources.
