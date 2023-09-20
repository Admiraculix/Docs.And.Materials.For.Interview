ACID SQL (atomicity, consistency, isolation, durability)
https://youtu.be/yaQ5YMWkxq4
https://blog.sqlauthority.com/i/c/acid.png
https://blog.sqlauthority.com/2007/12/09/sql-server-acid-atomicity-consistency-isolation-durability/
4.1 Atomicity -> The transaction should be atomic. If some steps fail. Everything fails and should be rollback.
4.2 Consistency -> Help ensure the data to be in the CORRECT state. Data integrity constraints must be followed (Constraints/ Cascades/ Triggers)
*4.3 Isolation levels
Problems: Dirty Read, Nonrepeatable Read, Phantom 
Solutions: (Read uncommited, read commited, Repeatable read, Serializable)
https://www.youtube.com/watch?v=dGMSrvWjyvM&list=PLS2xabqmZjj0YFdhA56XsoM4gN1fmNp8e
https://www.youtube.com/watch?v=ZtPj09tJjnQ
https://www.youtube.com/watch?v=-gxyut1VLcs
Optimistic vs Pessimistic concurrency control
4.4 Durability -> Committed transactions to be persisted in non-volatile memory or storage so
that even if crash happens or something wrong happens with the DB the data must be there and
not be corrupted.