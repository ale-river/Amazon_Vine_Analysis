# Amazon_Vine_Analysis :EMOJICODE:

This project helps to apply skills in:
- Importing data into a table for analysis.
- Applying filters, conditional formatting, and formulas.
- Generating and interpreting pivot tables.
- Calculating summary statistics such as measures of central tendency, standard deviation, and variance.
- Characterizing data to identify outliers in datasets.
- Performing an Excel analysis with visualizations.
- Interpreting common Excel visualizations

## Overview of Project

In this project, it is selected access to approximately one of 50 datasets available by Amazon. Each one contains reviews of a specific product, from clothing apparel to wireless products. By picking one of these datasets, it is used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. 
Using PySpark, Pandas, or SQL, it is determined if there is any bias toward favorable reviews from Vine members in your dataset.

## Analysis and Challenges

The dataframes show votes which are considered 50% helpful votes. 
In the `Perform_ETL_on_Amazon_Product_Reviews.ipynb` it is filtered the dataset with vine reviews. 
Additionally, the `Determine_Bias_of_Vine_Reviews.ipynb` shows the summary statistics where the "Star Ratings" are classified by quantities of "viner" and "non-viner" reviews. There were about 41,000 records that did not have vine reviews, and only 94 records that did have vine reviews.

## Results

The percentage of 5-star ratings for both groups. 51% of Amazon reviews that were part of the vine program gave a 5-star rating. 
38% of Amazon reviews that were not part of the vine program also gave a 5-star rating. 
In conclusion, there are less Amazon reviews that had "viners" than those do not have "viners". Therefore, there is a probable biased in the "Star Ratings".

SQL vine_table -> Connection between AWS and pgAdmin.
!(vine_table)[resources/vine_table.png]