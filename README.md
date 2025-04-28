# Nashville_datacleaning_sql
This project demonstrates data cleaning using SQL queries on a housing dataset (NashvilleHousing table). The queries focus on preparing raw real estate data into a more usable, structured, and standardized form.

🛠 Project Details

    Dataset/Table:

        PortfolioProject.dbo.NashvilleHousing

        Likely contains housing data such as addresses, dates, ownership details, and sales information.

    Major Tasks Performed in SQL:

        Standardizing the Date Format:

            Converts SaleDate into a proper DATE type.

            Handles issues if direct updates don't work by creating a new column (SaleDateConverted).

        Handling Missing Property Addresses:

            Populates missing PropertyAddress values by matching ParcelID between different rows.

        Breaking Out Address Components:

            Likely splits fields like PropertyAddress into:

                Street Address

                City

                State

        Standardizing Text Data:

            Example: Cleaning up OwnerName or other fields for consistent formatting.

        Removing Duplicates:

            Identifies and deletes duplicate records.

        Handling Unnecessary Columns:

            Removes redundant fields after cleaning.

            🧹 Data Cleaning Portfolio Project (SQL)

This project showcases how to clean raw real estate data using SQL techniques.
The focus is on preparing the NashvilleHousing dataset for better usability by handling missing values, fixing formats, and improving data quality.
📋 Dataset

    Source Table: PortfolioProject.dbo.NashvilleHousing

    Content: Real estate transactions including sale dates, addresses, owner names, parcel IDs, and property values.

🛠 Key Cleaning Steps

    Standardized date formats for SaleDate

    Populated missing property addresses using self-joins

    Separated address fields into street, city, and state

    Standardized ownership and other textual fields

    Removed duplicate records

    Dropped unnecessary columns to streamline the dataset

🛠 Technologies Used

    SQL Server

    SQL (DDL & DML commands)

    Functions like CONVERT(), ISNULL(), JOIN, ALTER TABLE, etc.

🚀 How to Run

    Open the SQL file (Data Cleaning Portfolio Project Queries.sql) in your SQL editor (e.g., SSMS, Azure Data Studio).

    Connect to your database and ensure the NashvilleHousing table exists.

    Run the queries step-by-step to clean the data.

📢 Notes

    Make sure to back up your data before running UPDATE or DELETE queries.

    Some queries are dependent on others (e.g., adding a column before updating it).


