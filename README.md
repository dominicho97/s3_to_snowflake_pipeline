# s3_to_snowflake_pipeline
##ETL pipeline from AWS s3 to snowflake

Uploading unstructured data to an S3 bucket and extracting, transforming and loading the data <br> with SQL queries inside snowflake to store it in a snowflake data warehouse. 
![etls3snowflake](https://github.com/dominicho97/s3_to_snowflake_pipeline/assets/43000003/23076ce4-b3da-43e3-a80f-e61f14d4b387)

## Access rights
To have the correct access rights to move the data from s3 to snowflake:<br>
- We need to make a new **Role** using the aws **Identity and Access Management(IAM)**
- The IAM role is configured with the **policy** that grants access to S3
- Then we need to make a **storage integration objecct** that is linked to the s3 bucket
- A **trust relationships** from the IAM role has to be formed with the right credentials (Storage IAM user ARN and External ID)
![etl3snowflake_access](https://github.com/dominicho97/s3_to_snowflake_pipeline/assets/43000003/14e38528-b250-4f6c-9573-12096e5696f8)
