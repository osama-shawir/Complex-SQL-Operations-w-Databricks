
[![CI](https://github.com/nogibjj/Complex-SQL-Operations-w-Databricks/actions/workflows/cicd.yml/badge.svg)](https://github.com/nogibjj/Complex-SQL-Operations-w-Databricks/actions/workflows/cicd.yml)


# ETL Pipeline with Delta Lake in Databricks

## Overview
This project demonstrates the implementation of an ETL (Extract, Transform, Load) pipeline using Databricks, Delta Lake, and Spark SQL. The primary goal is to extract data from an external source, perform transformations, and load the transformed data into a Delta Lake table. The project includes proper error handling, data validation, visualization of the transformed data, and an automated trigger for pipeline initiation.


![Alt Text](pipeline.png)


- **Data**: This directory contains the input data files.

  - `Admissions.csv`: A CSV file containing personal information for individuals, including their Social Security Numbers (SSN), names, addresses, and other details.

<img width="509" alt="image" src="https://github.com/osama-shawir/Complex-SQL-Operations-w-Databricks/assets/89782802/a37e98b9-a1ab-4b6c-b793-7b4676ee1530">


## Project Components

### 1. Databricks Notebook
The Databricks notebook serves as the core of the ETL pipeline. It is responsible for the extraction, transformation, and loading of data. Spark SQL is leveraged for efficient and scalable data transformations.

<img width="677" alt="Screenshot 2023-11-28 220833" src="https://github.com/osama-shawir/Complex-SQL-Operations-w-Databricks/assets/89782802/9b21ac26-458c-4343-83f3-6d5d5a2c1abc">

<img width="594" alt="Screenshot 2023-11-28 220901" src="https://github.com/osama-shawir/Complex-SQL-Operations-w-Databricks/assets/89782802/e2fc8cc6-c2a7-4038-b6c4-7cdec6efdf38">

### 2. Delta Lake
Delta Lake is utilized as the data storage solution due to its ACID compliance and versioning capabilities. It ensures data integrity and provides efficient management of the data lake.

<img width="419" alt="image" src="https://github.com/osama-shawir/Complex-SQL-Operations-w-Databricks/assets/89782802/43400ca0-75b9-437a-847f-e5f71a1a9ea9">


### 3. Spark SQL
Spark SQL is employed for data transformations, allowing for flexible and scalable processing of large datasets.

<img width="490" alt="image" src="https://github.com/osama-shawir/Complex-SQL-Operations-w-Databricks/assets/89782802/e52af5cd-d08a-46ef-a532-3b0cd8209b3d">

<img width="651" alt="image" src="https://github.com/osama-shawir/Complex-SQL-Operations-w-Databricks/assets/89782802/c628fc00-4c03-40a8-b578-2bc114279555">

### 4. Error Handling and Data Validation
The ETL pipeline incorporates robust error handling mechanisms to gracefully handle exceptions during extraction, transformation, and loading phases. Additionally, data validation checks are implemented to ensure the quality of the processed data.

### 5. Data Visualization
The transformed data is visualized using Matplotlib and Seaborn in the Databricks notebook. This visualization provides insights into the relationships and distributions within the dataset.

<img width="749" alt="image" src="https://github.com/osama-shawir/Complex-SQL-Operations-w-Databricks/assets/89782802/2f913c51-e028-486c-aa4f-b96ddf1a019b">

### 6. Automated Trigger
An automated trigger initiates the ETL pipeline based on predefined schedules or events.

<img width="755" alt="image" src="https://github.com/osama-shawir/Complex-SQL-Operations-w-Databricks/assets/89782802/57e6a170-b387-4ae4-aaf3-2c83c3cbe2fc">

<img width="760" alt="image" src="https://github.com/osama-shawir/Complex-SQL-Operations-w-Databricks/assets/89782802/e2ccc698-c4c6-42bf-8bdf-2c31458b63cf">


## How to Run the Program
1. Open the Databricks notebook in your Databricks workspace.
2. Execute each cell in the notebook sequentially.
3. Ensure that the necessary dependencies are installed.
4. Review the output and visualizations generated in the notebook.

## Conclusion and Recommendations
The successful execution of this ETL pipeline demonstrates the capability to extract, transform, and load data efficiently using Databricks, Delta Lake, and Spark SQL. The Delta Lake storage solution ensures data integrity, version control, and easy management. The visualizations offer insights into key relationships within the data.

**Recommendation:** Based on the analysis, management may consider refining admission criteria or focusing on specific factors (e.g., Normalized CGPA) to improve the chances of successful admissions.

## Notes
- Adjust the notebook parameters and configurations based on your specific environment.
- Make sure to set up the automated trigger according to your desired schedule or event.

Enjoy exploring and analyzing your data with Delta Lake in Databricks!

## Data Source
The dataset used in this project is sourced from the [Admission dataset](https://github.com/selva86/datasets/blob/master/Admission.csv) available on GitHub.
