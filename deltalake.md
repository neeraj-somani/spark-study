# Top links to understand basics of Delta lake:
- Apache Hudi, Apache Iceberg, and Delta Lake [here](https://chat.openai.com/share/ccbdd232-c646-42e8-ac0d-7fd5947c7d7b)
- Copy on Write(CoW) and Merge On Read(MoR)

## few delta related spark settings
- MERGE operations support generated columns when you set spark.databricks.delta.schema.autoMerge.enabled to true.
- to set the delta.appendOnly = true property for all new Delta Lake tables created in a session -- SET spark.databricks.delta.properties.defaults.appendOnly = true
