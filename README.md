# Movies ETL

## Overview
For this challenge, we're helping Britta prepare databases on a weekly basis for the company Amazing Prime. We have data from Wikipedia, metadata from Kaggle, and ratings also from Kaggle, and it all needs to be read, cleaned, and put together into an SQL database efficiently.

### Purpose
The purpose of this challenge is to do the ETL process within a few functions that can be run easily each week. 

## Results

### Deliverable 1
To start, we practiced reading the files into dataframes.

### Deliverable 2
Then, we cleaned the Wikipedia data so that it was usable and comparable to the Kaggle metadata.

### Deliverable 3
After that, we cleaned the Kaggle metadata and the ratings data, and merged them with the Wikipedia data in an interative process. We had to figure out where redundancies were between the Kaggle data and the Wikipedia data and what to do about it in the Modules, and we enacted that plan again in this challenge. The ratings data needed to be reduced because it was too long, then it was pivoted and merged to the other two databases.

### Deliverable 4 
Lastly, we had to move the dataframe to SQL. We did this by making an engine to communicate with SQL. Then we added the movies_with_ratings_df data easily. The ratings data had to be added in chunks because it was so large. 

Once that was complete, we could enter pgAdmin and make a query to check if we have the correct number of rows. 

![Movies Query looks good](https://github.com/saramcel/Movies-ETL/blob/50bf9b2113a0b368b22f6b84b92e62c3f1f34be7/Resources/movies_query.png)

There are 6,052 rows in the movies table.

![Ratings Query looks good](https://github.com/saramcel/Movies-ETL/blob/50bf9b2113a0b368b22f6b84b92e62c3f1f34be7/Resources/ratings_query.png)

There are 26,024,289 rows in the ratings table. 

## Conclusion

This refactoring of the module code is much more succinct and it will allow us to run only a few cells to get the desired results. It is good to see it come together after all the exploration in the modules. 
