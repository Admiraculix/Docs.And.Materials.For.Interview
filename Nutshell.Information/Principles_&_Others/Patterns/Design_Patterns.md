**Design patterns:
https://www.dofactory.com/net/design-patterns
https://refactoring.guru/design-patterns/csharp
# Creational Patterns:
*Abstract Factory	Creates an instance of several families of classes.
			Abstract Factory is a creational design pattern, which solves the problem of creating 				entire product families without specifying their concrete classes.

*Builder		Separates object construction from its representation✔️.
			It’s especially useful when you need to create an object with lots of possible 					configuration options.

*Factory Method		Creates an instance of several derived classes✔️.
			It’s very useful when you need to provide a high level of flexibility for your code.
			Factory method is a creational design pattern which solves the problem of creating 				product objects without specifying their concrete classes.

*Prototype		A fully initialized instance to be copied or cloned.

*Singleton		A class of which only a single instance can exist✔️.
			Singleton is a creational design pattern, which ensures that only one object of its kind 			exists and provides a single point of access to it for any other code.

# Structural Patterns:	
*Adapter		Match interfaces of different classes.
			Adapter is a structural design pattern, which allows incompatible objects to collaborate.
			The Adapter acts as a wrapper between two objects. It catches calls for one object and 				transforms them to format and interface recognizable by the second object.

*Bridge			Separates an object’s interface from its implementation.

*Composite		A tree structure of simple and composite objects.

*Decorator		Add responsibilities to objects dynamically.
			Decorator is a structural pattern that allows adding new behaviors to objects dynamically 			by placing them inside special wrapper objects, called decorators.
			Using decorators you can wrap objects countless number of times since both target objects 			and decorators follow the same interface. The resulting object will get a stacking 				behavior of all wrappers.

*Facade			A single class that represents an entire subsystem.

*Flyweight		A fine-grained instance used for efficient sharing.

*Proxy			An object representing another object.

# Behavioral Patterns:	
*Chain of Resp.		A way of passing a request between a chain of objects.

*Command		Encapsulate a command request as an object.
			Command is behavioral design pattern that converts requests or simple operations into 				objects.
			The conversion allows deferred or remote execution of commands, storing command history, 			etc.

*Interpreter		A way to include language elements in a program.

*Iterator		Sequentially access the elements of a collection.

*Mediator		Defines simplified communication between classes.✔️?
			Mediator is a behavioral design pattern that reduces coupling between components of a 				program by making them communicate indirectly, through a special mediator object
			The Mediator makes it easy to modify, extend and reuse individual components because 				they’re no longer dependent on the dozens of other classes.
			The most popular usage of the Mediator pattern in C# code is facilitating communications 			between GUI components of an app. The synonym of the Mediator is the Controller part of 			MVC pattern.

*Memento			Capture and restore an object's internal state.

*Observer		A way of notifying change to a number of classes.

*State			Alter an object's behavior when its state changes✔️.
			State is a behavioral design pattern that allows an object to change the behavior when 				its internal state changes.
			The pattern extracts state-related behaviors into separate state classes and forces the 			original object to delegate the work to an instance of these classes, instead of acting 			on its own.

*Strategy		Encapsulates an algorithm inside a class✔️.
			Strategy is a behavioral design pattern that turns a set of behaviors into objects and 				makes them interchangeable inside original context object.
			It’s often used in various frameworks to provide users a way to change the behavior of a 			class without extending it.
			The original object, called context, holds a reference to a strategy object. The context 			delegates executing the behavior to the linked strategy object. In order to change the 				way the context performs its work, other objects may replace the currently linked 				strategy object with another one.

*Template Method		Defer the exact steps of an algorithm to a subclass.

*Visitor			Defines a new operation to a class without change.




PoEAA - Patterns of Enterprise Application Architecture
Gangs of Four (GoF) Design Patterns

Repository pattern
Unit of work