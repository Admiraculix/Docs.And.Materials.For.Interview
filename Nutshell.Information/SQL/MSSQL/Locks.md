***
- [f] Exclusive lock vs Shared lock; (Update lock, Intent locks)
      
- [b] Link: https://www.youtube.com/watch?v=nuBi2XbHH18
- [b] Link: https://www.sqlshack.com/locking-sql-serve
- [b] Link: https://www.geeksforgeeks.org/difference-between-shared-lock-and-exclusive-lock/

- One of the method to ensure isolation property in transaction is to require data items be accessed in a mutually exclusive manner. That means, while one transaction is accessing a data item, no other transaction can modify that data item. So, the most common method used to implement requirement is to allow a transaction to access a data item only if it is currently holding a lock on that item. Thus, the lock on operation is required to ensure isolation of transaction. 

**Shared lock (S):**
- Another transaction that tries to read the same data is permitted to read, but a transaction that tries to update the data will be prevented from doing so until the shared lock is released.
- Shared lock is also called read lock, used for reading data items only.
- Shared locks support read integrity. They ensure that a record is not in process of being updated during a read-only request.
- Shared locks can also be used to prevent any kind of updates of record.
- It is denoted by Lock-S.
- S-lock is requested using Lock-S instruction.

> [!note] For example, consider a case where initially A=100 and there are two transactions which are reading A. If one of transaction wants to update A, in that case other transaction would be reading wrong value. However, Shared lock prevents it from updating until it has finished reading. 

**Exclusive Lock (X):**
- When a statement modifies data, its transaction holds an exclusive lock on data that prevents other transactions from accessing the data.
- This lock remains in place until the transaction holding the lock issues a commit or rollback.
- They can be owned by only one transaction at a time.
- With the Exclusive Lock, a data item can be read as well as written. Also called write lock.
- Any transaction that requires an exclusive lock must wait if another transaction currently owns an exclusive lock or a shared lock against the requested resource.
- They can be owned by only one transaction at a time.
- It is denoted as Lock-X.
- X-lock is requested using Lock-X instruction.

> [!note] For example, consider a case where initially A=100 when a transaction needs to deduct 50 from A. We can allow this transaction by placing X lock on it. Therefore, when the any other transaction wants to read or write, exclusive lock prevent it


Tags: #sql #locks