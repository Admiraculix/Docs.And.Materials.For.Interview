***
- [f] Sync vs async (long-running operations) :

- [i] The differences between asynchronous and synchronous include:
- Async is multi-thread, which means operations or programs can run in parallel.
- Async is non-blocking, which means it will send multiple requests to a server.
- Async increases throughput because multiple operations can run at the same time.
- Sync is single-thread, so only one operation or program will run at a time.
- Sync is blocking — it will only send the server one request at a time and will wait for that request to be answered by the server.
- Sync is slower and more methodical.

- [b] Link: https://www.bytehide.com/blog/async-vs-sync-csharp
- [b] Link: https://devblogs.microsoft.com/visualstudio/how-do-i-debug-async-code-in-visual-studio/
 - asynchronous execution is suitable to avoid blocking the main thread.
Task.WhenAll to process multiple tasks concurrently

**PLINQ**
- [b] Link: https://learn.microsoft.com/en-us/dotnet/standard/parallel-programming/introduction-to-plinq
Parallel.ForEach
- [b] Link: https://learn.microsoft.com/en-us/dotnet/api/system.threading.tasks.parallel.foreach?view=net-5.0


Tags: #async #sync