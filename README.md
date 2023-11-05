# Yelp-Data-Analysis---Azure-Databricks-Project

Yelp is a community review site and an American multinational firm based in San Francisco, California. It publishes crowd-sourced reviews of local businesses as well as the online reservation service Yelp Reservations. Yelp has made a portion of their data available in order to launch a new activity called the Yelp Dataset Challenge, which allows anyone to do research or analysis to find what insights are buried in their data. 

Due to the bulk of the data, this project only selects a subset of Yelp data in a zip file named 'dataset.zip,' which comprises three JSON files, including 'business.json', which provides business data such as location data, attributes, and categories.

T𝗲𝗰𝗵 𝗦𝘁𝗮𝗰𝗸
Language: Python3
Services: Azure Data factory, Azure Databricks, Azure Data Lake Storage


𝗗𝗮𝘁𝗮 𝗔𝗻𝗮𝗹𝘆𝘀𝗶𝘀:
From the Yelp website, the academic dataset is downloaded containing business, checkin, review, tips and users.
The resource manager is created in Azure to categorise the resources required followed by Storage account for storing data required and the Creation of containers for uploading the dataset.
The pipeline is created to copy the data from Azure storage to Azure data lake storage in the Azure data factory.
The Databricks workspace and cluster is created, accessed and configured Azure data lake storage from databricks.
The conversion process is done by converting the Yelp academics data file from JSON format to Parquet format and further converting it to Delta format for smooth analysis.
In the transformation and load process, the uploaded dataset in Spark is read into Spark data frames.
Finally, data is analyzed into Spark in Databricks deducing recommendations and data are visualized using bar charts.

𝗖𝗼𝗻𝘃𝗲𝗿𝘀𝗶𝗼𝗻: During the conversion process, the Yelp academic dataset JSON file is converted to Parquet format and further Parquet format is converted to the Delta format for further data analysis in Databricks.

𝗧𝗿𝗮𝗻𝘀𝗳𝗼𝗿𝗺𝗮𝘁𝗶𝗼𝗻 𝗮𝗻𝗱 𝗟𝗼𝗮𝗱: During the transformation and load process, the uploaded dataset in Spark is read into Spark data frames. And dataset is finally analyzed in Databricks into Spark and further recommendations are deduced.


𝗔𝗽𝗽𝗿𝗼𝗮𝗰𝗵
1) Read yelp datasets in ADLS and convert JSON to parquet for better performance.
2) Convert JSON to Delta Format.
3) Total records in each dataset.
4) Partition tip dataset tip by a date column.
5) repartition() vs coalesce()
6) Find the top 3 users based on their total number of reviews.
7) Find the top 10 users with the most fans
8) Analyse the top 10 categories by a number of reviews.
9) Analyse top businesses which have over 1000 reviews.
10) Analyse Business Data: Number of restaurants per state.
11) Analyze the top 3 restaurants in each state.
12) List the top restaurants in a state by the number of reviews.
13) Numbers of restaurants in Arizona state per city.
14) Broadcast Join: restaurants as per review ratings in Pheonix city.
15) Most rated Italian restaurant in Pheonix.

**Architecture Diagram**
![image](https://github.com/srijamannam/Yelp-Data-Analysis---Azure-Databricks-Project/assets/92010369/67396792-6f3e-4860-861d-2a3776a00b6e)
