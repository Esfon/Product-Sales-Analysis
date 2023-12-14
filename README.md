# Product Sales Analysis

## Table of Contents
- [Introduction](#introduction)
- [Data Source](#data-source)
- [Data Preparation and Cleaning Process](#data-preparation-and-cleaning-process)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Recommedation](#recommendation)

## Introduction
  The records of selling the products have been listed to keep an eye on sale transactions. These 
transactions were recorded from January 1, 2019 to December 31, 2019. This contains the details 
of the sale such as orders with different products, the price for that product, order quantity, date, 
and address. These transactions contain sale from various cities in the United States of America. 
In this project, I dove into analyzing the sales record from each month focusing only the sales in 
2019. The process of analyzing rows of information will also undergo data cleaning and ensuring 
the data integrity and quality.

## Data Source
  The datasets were downloaded on GitHub, which is a free source of finding datasets to collaborate 
and share insights with other users. I downloaded the datasets containing 12 CSV files which were 
the sales record separated in months. I loaded all 12 CSV files in Jupyter Notebook and did the 
whole project of cleaning, transforming, analyzing, and visualizing the data.

## Data Preparation and Cleaning Process
  I loaded all 12 CSV files and combined them into one single dataset by utilizing the Pandas library. 
I started the process by checking the data types of each column and taking advantage of the 
library’s functions specifically for transformation. I also filtered the data which only contains the 
sales record in the year 2019. Then I set into the contents of the datasets by cleaning each dataset’s 
columns. I performed such process like:

  1.Removing null values. <br />
  2.Dropping duplicated records. <br />
  3.Numeric columns into numeric data types (Price, Quantity Ordered). <br />
  4.Splitting the address and creating additional columns (City, State, ZIP code). <br />
  5.Fixing the abbreviation values in ‘State’ column and used the full name of the states in USA. <br />
  6.Creating a column ‘Sales’ based on existing columns. ‘Sales’ column was added by multiplying
  the ‘Price’ column and ‘Quantity Ordered’ column. <br />
  7.Transformed the ‘Order Date’ format by splitting the date and time into two separate columns. <br />
  8.Filtered the order date value with records only showing the year 2019. <br />
  9.Removed, reordered, and renamed columns. <br />


## Exploratory Data Analysis
- In the month of december, sales have achieved the highest total with an amount of $4,608,295.70.
- The total percentage change of total sales from month to month is 133.33%.
- San Francisco has the highest total sale of $8,252,258.67.
- AAA Batteries (4-pack) has the highest total quantity order of 30981 while not having a high price. The Macbook Pro Laptop has the highest price of $1,700 while having one of the fewest orders.
- On December 4, 2019, selling of products has achieved the highest total sales of different products with an amount of $166,577.69.
- From 10am - 9pm of sales, the products ordered by the customers have a total quantity of at least 11,000 products. This could explain that the sales in that time span are very active.

## Recommendation
- Promoting products and planning discounts especially on seasonal months like December.
- Prioritize noon time sales to increase chance of gaining more customers.
- Consider the success of the cities with high activity in sales like San Fransico and Los Angeles to take an opportunity of exploring new regions.

