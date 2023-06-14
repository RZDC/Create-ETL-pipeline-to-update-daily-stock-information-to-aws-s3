# Create-ETL-pipeline-to-update-daily-stock-information-to-aws-s3-and-local

This Is a project that can update daily stock price information to docker file and s3, then will start glue job to conver csv file to parquet file in s3.
To Start this project you will need: 
  1. Create apikey from https://www.alphavantage.co/support/#api-key
  2. Aws account that can set up S3, glue and Athena.
  3. Download VScode and docker desktop extension

Second, setup docker by using docker for stock/docker-compose.yaml and type: docker-compose up. Wait for few minute then open browser type http://localhost:8080 and Username: airflow, Password: airflow, to use airflow UI.

Third, setup csv folder and parquet folder in s3 Buckets, add tables using crawler and create job for crawler.

Fourth, Input your api key, aws access_key and secret_access_key in AMZN_TIME_SERIES_DAILY_ADJUSTED.py
