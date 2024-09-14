## Formula One Races Data Warehousing
### Project Description
The goal of this project is to built a scalable and efficient data pipeline to ingests, processes, and analyzes large volumes of data in near real-time, and stores the processed data in a scalable way.

The dataset consists of data for the <a href='https://en.wikipedia.org/wiki/Formula_One' method='Post'>Formula One</a> series, from the beginning of the world championships in 1950 until 2021 using <a href='http://ergast.com/mrd/'>Ergast API</a>. The data is formatted in JSON and CSV in different possible ways including single- and multi-line JSON and single- and multi-file CSVs.

### Solution Architect

![architecture](https://github.com/pranavkallem/Formula1_Azure_DataEngineering/blob/main/Architecture.png)

This architecture has three stages.
<ul>
  <li><b>Data ingestion</b>: in this stage, the raw data is ingested into the delta lake and stored in the raw layer.</li>
  <li><b>Data transformation</b>: in this stage, the data is cleaned and processed in a way that can be used for analysis.</li>
  <li><b>Analysis</b>: in this stage, the data is analyzed.</li>
</ul>

### Implementation
For the implementation of this solution, Azure Databricks, Data Factory, Storage services, and GitHub are used as follows:
 <ul>
  <li>Leveraged Azure Databricks to ingest, process, and analyze the data using Python and SQL notebooks.</li>
  <li>Used Azure Data Factory to create, schedule and manage data pipelines</li>
  <li>Used Azure Delta Lake to store the data</li>
  <li>Implemented incremental load to ensure that the data was up-to-date.</li>
  <li>Connected Power BI to Databricks to create interactive reports.</li>
  <li>Used GitHub for version control and collaboration</li>
 <ul>

### Some Visualizations of the Data
![dominant drivers](https://github.com/pranavkallem/Formula1_Azure_DataEngineering/blob/main/Dominant_drivers.png)
![dominant teams](https://github.com/pranavkallem/Formula1_Azure_DataEngineering/blob/main/Dominant_teams.png)

