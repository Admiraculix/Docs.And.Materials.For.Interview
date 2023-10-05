***
- [f] ACID SQL (atomicity, consistency, isolation, durability)
      
- [b] Link: https://youtu.be/yaQ5YMWkxq4
- [b] Link: https://blog.sqlauthority.com/i/c/acid.png
- [b] Link: https://blog.sqlauthority.com/2007/12/09/sql-server-acid-atomicity-consistency-isolation-durability/
**Atomicity** -> The transaction should be atomic. If some steps fail. Everything fails and should be rollback.
**Consistency** -> Help ensure the data to be in the CORRECT state. Data integrity constraints must be followed (Constraints/ Cascades/ Triggers)
**Isolation levels** ->
Problems: Dirty Read, Nonrepeatable Read, Phantom 
Solutions: (Read uncommited, read commited, Repeatable read, Serializable)
- [b] Link: https://www.youtube.com/watch?v=dGMSrvWjyvM&list=PLS2xabqmZjj0YFdhA56XsoM4gN1fmNp8e
- [b] Link: https://www.youtube.com/watch?v=ZtPj09tJjnQ
- [b] Link:https://www.youtube.com/watch?v=-gxyut1VLcs
- [I] *Optimistic vs Pessimistic concurrency control*
**Durability** -> Committed transactions to be persisted in non-volatile memory or storage so
that even if crash happens or something wrong happens with the DB the data must be there and
not be corrupted.

Tags: #sql #acid