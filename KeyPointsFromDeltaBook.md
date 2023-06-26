# Key Points From Book -- O'Reilly Delta Lake: The Definitive Guide
- All the points covered in this book is also available from official website -- https://docs.delta.io/latest/index.html
- So taking notes from there

## Intro
- Delta Lake provides ACID transactions, scalable metadata handling, and unifies streaming and batch data processing on top of existing data lakes, such as S3, ADLS, GCS, and HDFS.

## [data lakehouse](https://www.databricks.com/blog/2021/08/30/frequently-asked-questions-about-the-data-lakehouse.html)
A data lakehouse is a combination of - Data Lake + Data Warehouse
- Lakehouse key features
    - Trasaction support
    - Schema enforcement and governance
    - BI support
    - Storage is decoupled from compute
    - Openness
    - Support for diverse data types ranging from unstructured to structured data
    - Support for diverse workloads: including data science, machine learning, and SQL and analytics
    - End-to-end streaming: real or batch
 
> Lakehouse tackles the fundamental issues that make data swamps out of data lakes. It adds ACID transactions to ensure consistency as multiple parties concurrently read or write data. It supports DW schema architectures like star/snowflake-schemas and provides robust governance and auditing mechanisms directly on the data lake. It also leverages various performance optimization techniques, such as caching, multi-dimensional clustering, and data skipping, using file statistics and data compaction to right-size the files enabling fast analytics. And it adds fine-grained security and auditing capabilities for data governance. By adding data management and performance optimizations to the open data lake, lakehouse can natively support BI and ML applications.

- Does the Data Lakehouse have to be centralized or can it be decentralized into a Data Mesh?
  - No, organizations do not need to centralize all their data in one Lakehouse. Many organizations using the Lakehouse architecture take a decentralized approach to store and process data but take a centralized approach to security, governance, and discovery. Depending on organizational structure and business needs, we see a few common approaches:
  - Each business unit builds its own Lakehouse to capture its business' complete view – from product development to customer acquisition to customer service.
  - Each functional area, such as product manufacturing, supply chain, sales, and marketing, could build its own Lakehouse to optimize operations within its business area.
  - Some organizations also spin up a new Lakehouse to tackle new cross-functional strategic initiatives such as customer 360 or unexpected crises like the COVID pandemic to drive fast, decisive action.
 
- How does the Data Mesh relate to the Data Lakehouse?
  - Domain-oriented decentralized data ownership and architecture
  - Data as a product
  - Self-serve data infrastructure as a platform
  - Federated computational governance

# Data lakes vs. data lakehouses vs. data warehouses
![image](https://github.com/neeraj-somani/spark-study/assets/25622536/813f5c63-eca6-4121-af8b-e38257220f0a)
