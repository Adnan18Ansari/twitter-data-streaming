## Twitter Data Streaming
The goal of this project is to create a multi-purpose platform that acquires data from the Twitter developers API (in real-time), based on certain keywords of interest. Once the data is collected, the platform wil perform data filtering, cleansing and enrichment to perform analytical operations for the organizational and business purposes and to transform raw data into knowledge.
![alt text](Architecture.png "Platform Design")

## Usage
- Run notebook HDFS_DB_Init.ipynb from start to end. This will create HDFS directories and HIVE tables  
- Run notebook twitter_Producer.ipynb from start to end. It will start receiveing tweets from twitter API and sending them to Kafka topic.  
- Run notebook Spark_Consumer.ipynb. It will start processing data in Spark, writing it to HDFS and refreshing HIVE tables. 
- Run notebook Dashboard.ipynb to see some graphs and distributions of data being collected



