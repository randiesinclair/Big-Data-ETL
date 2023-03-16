# Big Data ETL Challenge
-----

This assignment requires us to extract and transform two large Amazon customer review datasets and load them into a cloud database using PySpark. The goal is to perform the ETL process entirely in the cloud, as the datasets are too large to be handled on local machines. 

------
## Technical Skills
- Cloud Computing
- AWS RDS Database
- AWS S3 Buckets
- SQL
- ETL (Extract, Transform, Load)
- PySpark 

--------

## Project Parameters
### Extract
- Uses PySpark to connect to and load the AWS datasets into DataFrames.
- The correct parameters are used to read in the data into a DataFrame.
- The first 20 rows of each DataFrame is displayed.
- The number of rows for each DataFrame is displayed.

![Alt text](Images/Extract%20snapshot.JPG)

### Transform
- The "review_id_df" DataFrame is created with the appropriate columns and data types.

![Alt text](Images/Transform%20snapshot2.JPG)

- The "products_df" DataFrame is created and the the duplicate values are dropped.

![Alt text](Images/Transform%20snapshot3.JPG)

- The "customers_df" DataFrame is created and displays the number of times a customer reviewed a product grouped by the "customer_id".

![Alt text](Images/Transform%20snapshot4.JPG)

- The "vine_df" DataFrame is created that has the "review_id", "star_rating", "helpful_votes", "total_votes", and "vine" columns.

![Alt text](Images/Transform%20snapshot5.JPG)

### Load
- The four DataFrames for each dataset are successfully loaded into an RDS instance

![Alt text](Images/Load%20snapshot.JPG)