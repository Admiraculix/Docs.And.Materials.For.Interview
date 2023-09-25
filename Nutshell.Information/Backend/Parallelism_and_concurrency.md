***
- [f] Parallelism and concurrency handling (threads, locks, race conditions, deadlocks):

- [i] Always use *.ConfigureAwait(false)* when you don’t need to resume on the original context to avoid potential deadlocks

- Concurrency is when multiple tasks can run in overlapping periods. It’s an illusion of multiple tasks running in parallel because of a very fast switching by the CPU. Two tasks can’t run at the same time in a single-core CPU. Parallelism is when tasks actually run in parallel in multiple CPUs.

- Concurrency is about managing multiple instruction sequences at the same time, while parallelism is running multiple instruction sequences at the same time.

- [b] Link: https://www.geeksforgeeks.org/difference-between-concurrency-and-parallelism/
- [b] Link: https://freecontent.manning.com/concurrency-vs-parallelism

- ["] *As Rob Pike pointed out “Concurrency is about dealing with lots of things at once. Parallelism is about doing lots of things at once.”*

- An application can be concurrent but not parallel, which means that it processes more than one task at the same time, but no two tasks are executing at the same time instant.
- An application can be parallel but not concurrent, which means that it processes multiple sub-tasks of a single task at the same time.
- An application can be neither parallel nor concurrent, which means that it processes one task at a time, sequentially, and the task is never broken into subtasks.
- An application can be both parallel and concurrent, which means that it processes multiple tasks or subtasks of a single task concurrently at the same time (executing them in parallel)

 *Example: Imagine you have a program that inserts values into a hash table. If you spread the insert operation between multiple cores, that’s parallelism. But coordinating access to the hash table is concurrency.
 
 Tags: #parallelism #concurrency