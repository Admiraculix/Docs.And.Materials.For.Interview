***
- [f] Command Query Responsibility Segregation
- [b] Link: https://learn.microsoft.com/en-us/azure/architecture/patterns/cqrs

- [i] CQRS:
    is an architectural pattern that separates the handling of commands (actions that change the system state) from the handling of queries (actions that retrieve data without modifying the system state). In the CQRS pattern, you maintain separate models for reading and writing data. This separation allows you to optimize each model for its specific purpose. CQRS is often used in complex systems where the read and write requirements diverge significantly.
       
	In the context of CQRS, commands are used to update the write model, while queries are used to retrieve data from the read model. The write model is responsible for handling commands that result in changes to the system state, while the read model is designed to efficiently serve queries without affecting the write operations.


**MediatR nugget:** 
- [b] Link: https://github.com/jbogard/MediatR
- In-process messaging with no dependencies.
- Supports request/response, commands, queries, notifications and events, synchronous and async with intelligent dispatching via C# generic variance.
  


Tags: #nugget #architecture #oop #cqrs