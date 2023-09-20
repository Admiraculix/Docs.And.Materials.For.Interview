 Indexes - cluster / none-cluster
https://www.geeksforgeeks.org/difference-between-clustered-and-non-clustered-index/
https://youtu.be/ITcOiLSfVJQ

https://learn.microsoft.com/en-us/sql/relational-databases/indexes/clustered-and-nonclustered-indexes-described?view=sql-server-ver16
SQL Server documentation uses the term B-tree generally in reference to indexes. In rowstore indexes, SQL Server implements a B+ tree. This does not apply to columnstore indexes or in-memory data stores.

Clustered Index: DEFAULT value TSQL PRIMARY KEY is CLSUTERED INDEX
Definition: A clustered index determines the physical order of data in a table. Each table can have only one clustered index.
Data Storage: When a clustered index is defined, the actual data rows in the table are stored in the order of the clustered index key.
Performance: As the data is physically ordered, it is often faster to retrieve data through a clustered index for certain types of queries, especially range-based queries.
Table Reorganization: Adding or modifying a clustered index can require more time and resources as it may lead to the reorganization of the entire table's data.
Key Columns: The columns used in the clustered index are also referred to as the clustering key.

Non-Clustered Index: DEFAULT value TSQL UNIQUE KEY is NON-CLSUTERED INDEX
Definition: A non-clustered index is a separate structure from the table that contains a copy of the indexed columns and a pointer to the actual data row.
Data Storage: The data rows are not physically ordered based on the non-clustered index key; instead, they are organized separately from the table.
Performance: Non-clustered indexes are typically beneficial for speeding up queries involving columns not covered by the clustered index, as they provide efficient access to specific data subsets.
Table Reorganization: Creating or modifying non-clustered indexes usually requires less time and resources compared to clustered indexes.
Key Columns: Non-clustered indexes can be created on one or multiple columns to optimize different types of queries.