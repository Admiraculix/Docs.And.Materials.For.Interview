***
- [b] Link: https://tech.tamara.co/ddd-in-a-nutshell-3852b0a6155a

*The strategic pattern: 
Ubiquitous language - all steakholders speak same lang
This will help your teams align and agree on the same terms hence bringing in the same understanding of the definition or business. I would emphasize that this is needed and should be done from the beginning and keep going during the development period.

Bounded context -> Upstream and downstream (U or D) -> ACL -> Anti-corruption leayer pattern
- [b] Link: https://www.martinfowler.com/bliki/BoundedContext.html
 tool will assist you in defining primary and subdomains and the dependencies between them (upstream and downstream). Then, based on that, you would structure your application in terms of components or services. And last but not least, organizing your teams will be responsible for building and maintaining those services.

ACL: Translation from some 3th party. Implement a façade or adapter layer between different subsystems. 
* added latency
- [b] Link: https://learn.microsoft.com/en-us/azure/architecture/patterns/anti-corruption-layer


*The tactical pattern:
Aggregates -> 2 tactical standards (E & VO).  cluster of one or more entities and can contain Value obj. The parrent Entity of this cluster is Agreegate root
Entities -> a potentially changeable object, compare by Id, which has a unique identifier.
Value Objects -> compare by value, Immutable, not have a unique identity

Services -> stateless. domain-specific operations, which can involve multiple domain objects.
Repositories -> deal with storage. They are responsible for persisting Aggregates.
Factories -> provide abstraction in the construction of an Object > A,E,VO
Events -> It is common for Aggregates to publish events. > Domain Events, Integration events 
Modules -> defined as a package or a namespace depending on the programming languages, and always follow the Ubiquitous Language.

Combining the above building blocks, the Tactical Design also comes with many valuable patterns such as CQRS — Event Sourcing, Layered Architecture…