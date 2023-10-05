***
- [f] Deadlocks - How to solve?
- [b] Link: https://youtu.be/IR7rgByP8BI
- Debugging deadlocks: sp_BlitzLock <- Eric Darling, Open Source
- Debugging deadlocks: SentryOne Plan Explorer - reading deadlock_graph 
- [b] Link: https://www.youtube.com/watch?v=3EwDn9hqgkg
      
**Definition 1:** A deadlock is a situation where a set of processes are blocked because each process is holding a resource and waiting for another resource acquired by some other process. 

**Definition 2:** A deadlock is a situation in which two computer programs sharing the same resource are effectively preventing each other from accessing the resource, resulting in both programs ceasing(stopping) to function.

**Race condition:**
A race condition is an undesirable situation that occurs when a device or system attempts to perform two or more operations at the same time, but because of the nature of the device or system, the operations must be done in the proper sequence to be done correctly.

- Occur when two computer program processes, or threads, attempt to access the same resource at the same time and cause problems in the system. Race conditions are considered a common issue for multithreaded applications.

*Both are not the same. A race condition occurs when two threads use the same variable at a given time. Deadlock exists when two threads seek one lock simultaneously.*


Tags: #sql #deadlocks