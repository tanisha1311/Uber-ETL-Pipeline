# Uber-ETL-Pipeline
The goal of this project is to perform data analytics on Uber data using various tools and technologies, including GCP Storage, Python, Compute Instance, Mage Data Pipeline Tool, BigQuery, and Looker Studio.

# Architecture
![architecture](https://github.com/user-attachments/assets/f0d09b55-688c-489b-91c0-5ef8c822652d)

# Technology Used
- Programming Language - Python
- Google Cloud Platform : 
Google Storage, 
Compute Instance, 
BigQuery, 
Looker Studio
- Modern Data Pipeine Tool - https://www.mage.ai/

# Dataset Used
TLC Trip Record Data Yellow and green taxi trip records include fields capturing pick-up and drop-off dates/times, pick-up and drop-off locations, trip distances, itemized fares, rate types, payment types, and driver-reported passenger counts.
- Website - https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page
- Data Dictionary - https://www.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_yellow.pdf

# Data Model
![data_model](https://github.com/user-attachments/assets/65a4b83b-8ba7-4da8-9ac9-2cefde1b9327)

# Workflow
# Step 1 
- Activated an e2-standard-4 virtual machine on Google Cloud Platform to handle data processing and execute Mage pipelines.
- Configured the instance to ensure sufficient resources for managing large datasets and running complex transformations.
- Installed necessary tools and libraries on the instance, including Mage, Python, and required data processing dependencies.

# Step 2
- Uploaded the data to GCP Storage for centralized storage and seamless access.
- Configured Mage to connect to the GCP bucket and fetch the raw data.
- Validated the data in Mage to ensure there were no missing or corrupted files.

# Step 3
- Cleaned the data to remove duplicates, null values, and irrelevant columns.
- Standardized data formats, such as datetime, latitude, and longitude.
- Modeled the data into dimension tables (e.g., passenger and trip details) and fact tables (e.g., revenue and distance metrics).
- Exported the transformed data to BigQuery in the form of a dictionary, ensuring structured and easy-to-query data.

# Step 4
- Connected Mage-exported datasets to BigQuery and validated the schema.
- Conducted Exploratory Data Analysis (EDA) using SQL to identify trends:
  - Total revenue by day or week.
  - Popular pickup and drop-off zones based on latitude and longitude.
  - Average trip distance and duration.

# Step 5
Integrated Looker Studio with BigQuery to access the analyzed data directly.
<img width="1226" alt="image" src="https://github.com/user-attachments/assets/0aa7d22d-6694-452c-981b-34c1cb0a3946" />
<img width="1242" alt="image" src="https://github.com/user-attachments/assets/d24598eb-7135-4bfa-9f60-c0682dc324f7" />



