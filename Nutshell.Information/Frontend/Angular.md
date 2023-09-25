***
- [f] Angular architecture
- [b] Link: https://angular.io/guide/architecture

*Modules -> NgModules*
The architecture of an Angular application relies on certain fundamental concepts. The basic building blocks of the Angular framework are Angular components that are organized into NgModules. NgModules collect related code into functional sets; an Angular application is defined by a set of NgModules. An application always has at least a root module that enables bootstrapping, and typically has many more feature modules.

*Components -> @Component()*
-Components define views, which are sets of screen elements that Angular can choose among and modify according to your program logic and data
-Components use services, which provide specific functionality not directly related to views. Service providers can be injected into components as dependencies, making your code modular, reusable, and efficient.

Modules, components and services are classes that use decorators. These decorators mark their type and provide metadata that tells Angular how to use them.
-The metadata for a component class associates it with a template that defines a view. A template combines ordinary HTML with Angular directives and binding markup that allow Angular to modify the HTML before rendering it for display.
-The metadata for a service class provides the information Angular needs to make it available to components through dependency injection (DI)

*Templates, directives, and data binding directives provide program logic, and binding*

*Services and dependency injection*
@Injectable() decorator
-Routing -> is ngModule:
Enter a URL in the address bar and the browser navigates to a corresponding page
Click links on the page and the browser navigates to a new page
Click the browser's back and forward buttons and the browser navigates backward and forward through the history of pages you've seen


Tags: #menu #frontend
