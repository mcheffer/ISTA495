1. Create a database, name it ISTA495.practicum.nosql, in Azure Cosmos DB.[Instructions](https://docs.microsoft.com/en-us/learn/modules/create-cosmos-db-for-scale/1-introduction)

Make sure you choose 'serverless' when setting the capacity mode of your database. [Here](https://docs.microsoft.com/en-us/azure/cosmos-db/throughput-serverless) you can find a short video on the difference between 'provisioned' and 'serverless'.

2. Populate the database with the data that is available in the csv file included in this folder.
Use Azure Data Factory to import your cvs file into your Cosmos DB database. [Here](https://www.youtube.com/watch?v=5-SRNiC_qOU) is a short video on how to import cvs files into Cosmos DB.
3. Query your Azure Cosmos database and output the population share (population of the country divided by the population of the world) of the countires.