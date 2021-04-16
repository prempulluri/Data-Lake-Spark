# Data-Lake-Spark
• Built an ETL pipeline for a data lake.
• Data resides in S3, in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in the app.
• Loaded the data from Amazon S3.
• Processed the data into analytics tables using Apache Spark.
• Loaded the output tables into data lake (S3).
Tools used: Amazon S3, Python, Amazon EMR, Apache Spark


----------------------------------------------------------------------------------------------

A music streaming startup called Sparkify has grown their user base and song database and wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

In order to enable Sparkify to parse and analyze their data in a distributed manner, a Spark ETL Pipeline was created, which reads the data stored inside S3.
As their data engineer, I was tasked with building an ETL pipeline that extracts their data from S3, processes them using Spark, and loads the data back into S3 as a set of dimensional tables. This will allow their analytics team to continue finding insights in what songs their users are listening to.

In order to enable Sparkify to analyze their data,  Schema was created, which can be filled with an ETL pipeline.

The so-called star scheme enables the company to view the user behaviour over several dimensions. The fact table is used to store all user song activities that contain the category "NextSong". Using this table, the company can relate and analyze the dimensions users, songs, artists and time.

Fact Table: songplays
Dimension Tables: users, songs, artists and time.
