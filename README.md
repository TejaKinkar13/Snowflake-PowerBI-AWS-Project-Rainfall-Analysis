
# Rainfall-Agriculture-Analysis

### Dashboard Link : [Power BI Dashboard](YOUR_POWER_BI_LINK_HERE)

## Problem Statement

This project focuses on analyzing agricultural and weather-related data to understand rainfall, humidity, temperature, and crop yield.

The dashboard helps analyze these factors based on different years, locations, seasons, and crops. The project uses Amazon S3 for storing the dataset, Snowflake for data loading and transformation, and Power BI for visualization and analysis.

The complete flow of the project is:

**Amazon S3 → Snowflake → SQL Transformations → Power BI → Power BI Service**

---

## Steps followed

- Step 1 : Learned the basic architecture of Snowflake as a prerequisite for the project.

- Step 2 : Created an Amazon S3 bucket and uploaded the `session.csv` dataset.

- Step 3 : Created an AWS IAM Role and provided the required S3 access.

- Step 4 : Created a Snowflake Storage Integration using Amazon S3 as the storage provider.

- Step 5 : Added the AWS IAM Role ARN and S3 bucket location to the Storage Integration.

- Step 6 : Updated the IAM Role Trust Policy using the Snowflake IAM principal and External ID.

- Step 7 : Created the required database, schema, table and external stage in Snowflake.

- Step 8 : Loaded the data from Amazon S3 into Snowflake using `COPY INTO`.

- Step 9 : Created a separate Agriculture table for data transformation and analysis.

- Step 10 : Rainfall values were increased by 10% using:

        Rainfall * 1.1

- Step 11 : Area values were decreased by 10% using:

        Area * 0.9

- Step 12 : A new Rainfall Group column was created and rainfall was divided into:

        Low
        Medium
        High

- Step 13 : A Year Group column was created and the years were divided into three groups:

        Y1
        Y2
        Y3

- Step 14 : Snowflake was connected to Power BI and the Agriculture table was imported into Power Query.

- Step 15 : Appropriate data types were assigned to the columns in Power Query Editor.

- Step 16 : Four pages were created in Power BI for analysis:

        1. Rainfall Analysis
        2. Humidity Analysis
        3. Temperature Analysis
        4. Yield Analysis

- Step 17 : The completed Power BI report was published to Power BI Service.

---

# Project Architecture

![Project Architecture](https://github.com/user-attachments/assets/e8f47c9b-36ca-41aa-b2c4-a8ff4f3ff6ae)



# AWS S3

The `session.csv` dataset was uploaded to an Amazon S3 bucket and used as the source for the Snowflake data loading process.

![AWS S3](screenshots/aws-s3.png)


# Snowflake

Snowflake was used to load the data from Amazon S3 and perform SQL-based transformations before connecting the data to Power BI.

![Snowflake](screenshots/snowflake.png)


# Power BI Report

## 1. Rainfall Analysis

Rainfall was analyzed by:

- Year
- Location
- Season
- Crop

![Rainfall Analysis](screenshots/rainfall-analysis.png)


## 2. Humidity Analysis

Humidity was analyzed by:

- Year
- Location
- Season
- Crop

![Humidity Analysis](screenshots/humidity-analysis.png)


## 3. Temperature Analysis

Temperature was analyzed by:

- Year
- Location
- Season
- Crop

![Temperature Analysis](screenshots/temperature-analysis.png)


## 4. Yield Analysis

Yield was analyzed by:

- Year
- Location
- Season
- Crop

![Yield Analysis](screenshots/yield-analysis.png)


# Insights

The report was created to analyze the following:

### Rainfall

- Rainfall by year
- Rainfall by location
- Rainfall by season
- Rainfall by crop

### Humidity

- Humidity by year
- Humidity by location
- Humidity by season
- Humidity by crop

### Temperature

- Temperature by year
- Temperature by location
- Temperature by season
- Temperature by crop

### Yield

- Yield by year
- Yield by location
- Yield by season
- Yield by crop


# Power BI Service

The completed report was published to Power BI Service.

### Dashboard Link : [View Dashboard](YOUR_POWER_BI_LINK_HERE)


# Tools & Technologies

- Amazon S3
- AWS IAM
- Snowflake
- Snowflake SQL
- Power Query
- Power BI
- Power BI Service

