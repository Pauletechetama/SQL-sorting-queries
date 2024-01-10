# SQL-sorting-queries
This repository shows how I sorted data with SQL.
# About the project and data
In this project,i sorted data by using SQL queries with ORDER BY and WHERE clauses. I will be querying the CDC Births Data Summary public dataset. The queries will help obtain some answers about which counties in the United States have the most and least births in the years 2016-2018. 
# Description
I logged into BigQuery and clicked the Add button at the top of the explorer pane to call up the Add menu for various types of public repositories since i will be using a public dataset. In the marketplace search bar for public dataset options i searched for 'sdoh_cdc_wonder_natality' and in the resulting window, I click the 'CDC Births Data Summary', the dataset i will be working with. Viewed the datset which brought me the bigquery-public-data drop-down list in the Explorer menu where i can further browse the datasets and tables. Under the drop down list i will be working with 'county_natality dataset'. I opened this up and ran the first query to display the first 1,000 rows of the county_natality table. Below is the link to the query, when the query is ran it brings out the first 1000 rows.
# https://console.cloud.google.com/bigquery?sq=909859753623:2aa8993d04b24116b6025c463e8da6b0
The manager wants to figure out which 10 counties had the lowest birth count for 2016-2018. I did this by modifying the query to use the ORDER BY clause. Below is the link to the query,when ran it shows the proper result in acsending order.
# https://console.cloud.google.com/bigquery?sq=909859753623:d6a26451cd3048edb0b17ad218b43a8d
For the highest birth rate, i modified the query to sort in the other direction, returning the top 10 counties with the highest yearly birth counts. Below is the link, when ran it shows the proper result in descending order.
# https://console.cloud.google.com/bigquery?sq=909859753623:d70522f77fc24d3693baa1c887c90dea
Next, i modified the query so that it returns the top 10 counties with the highest birth counts for 2018 only. To do this, i added a WHERE clause to the query that specifies only rows that have a Year value equal to 2018-01-01. Below is the link, when ran it shows the proper result.
# https://console.cloud.google.com/bigquery?sq=909859753623:ced5aece1c9142bda9ff334033c29078
# Summary
When sorted in ascending order Tompkins County, NY, had just 735 births in 2018—the lowest birth count of any county in the US between 2016-2018. When sorted in decending order the query returns the 10 rows with the largest values in the Birth column. Los Angeles County takes up the top three spots.   
