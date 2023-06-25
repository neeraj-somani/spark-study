The Lakehouse medallion architecture lets you easily combine multiple different technologies in a data stack.

Suppose you have a data engineering team that ingests and cleans a 10-terabyte dataset using Spark & Scala. They use the medallion model to generate reports on the large dataset and also create datasets for teams that like using different tools.

They ingest the data into the bronze tables, perform some lightweight cleanup like deduplication, periodically join the bronze tables, and apply business-level transformations to incrementally update a silver table.

The silver table is used to build business-level aggregates in the gold table. For example, one of the gold tables is reduced to be sufficiently small for a data science team that likes using pandas.

Delta Lake is the ideal format for this data science team. It lets them leverage file skipping for fast queries and also lets them fix their models to certain versions of the Delta table via time travel. They use time travel to discern if model result changes are a result of changes in the code or changes in the data.

The #lakehouse storage system (#deltalake in this case) is what helps the #dataengineering and #datascience teams to collaborate effectively. Delta Lake is an efficient Lakehouse storage system and lets the data scientists use with pandas, their query engine of choice, even on a gold table that contains 50 GB of data.

The Lakehouse architecture lets teams work with the tools that make them productive and helps drive business value creation.


https://www.linkedin.com/feed/update/urn:li:activity:7078832245116915712/
