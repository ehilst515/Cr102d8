# Dependency Injection & Repository Design Pattern

## [Dependency injection in ASP.NET Core](https://docs.microsoft.com/en-us/aspnet/core/fundamentals/dependency-injection?view=aspnetcore-3.1)

>A dependency is an object that another object depends on.
>
>Code dependencies, such as in the previous example, are problematic and should be avoided for the following reasons:
>
>- To replace MyDependency with a different implementation, the IndexModel class must be modified.
>- If MyDependency has dependencies, they must also be configured by the IndexModel class. In a large project with multiple classes depending on MyDependency, the configuration code becomes scattered across the app.
>- This implementation is difficult to unit test. The app should use a mock or stub MyDependency class, which isn't possible with this approach.
>
>Dependency injection addresses these problems through:
>
>- The use of an interface or base class to abstract the dependency implementation.
>- Registration of the dependency in a service container. ASP.NET Core provides a built-in service container, IServiceProvider. Services are typically registered in the app's `Startup.ConfigureServices` method.
>- Injection of the service into the constructor of the class where it's used. The framework takes on the responsibility of creating an instance of the dependency and disposing of it when it's no longer needed.

## [The Repository pattern](https://docs.microsoft.com/en-us/dotnet/architecture/microservices/microservice-ddd-cqrs-patterns/infrastructure-persistence-layer-design#the-repository-pattern) / [Repository Design Pattern](https://medium.com/@pererikbergman/repository-design-pattern-e28c0f3e4a30)

The repository pattern abstracts the data layer and centralizes handling domain objects.

>Repositories are classes or components that encapsulate the logic required to access data sources. They centralize common data access functionality, providing better maintainability and decoupling the infrastructure or technology used to access databases from the domain model layer. If you use an Object-Relational Mapper (ORM) like Entity Framework, the code that must be implemented is simplified, thanks to LINQ and strong typing. This lets you focus on the data persistence logic rather than on data access plumbing.

## [SOLID Principles](https://www.telerik.com/blogs/30-days-of-tdd-day-five-make-your-code-solid) / [Why SOLID Matters](https://www.telerik.com/blogs/why-solid-matters)

The 5 SOLID Principles are:

***S**ingle Responsibility Principle* - A class should have a single responsibility

***O**pen Closed Principle* - Classes should be open for extension, but closed for modification

***L**iskov Substitution Principle* - If S is a subtype of T, then objects of type T in a program may be replaced with objects of type S without altering any of the desirable properties of that program.

***I**nterface Segregation Principle* - Clients should not be forced to depend on methods that they do not use.

***D**ependency Inversion Principle* -  High-level modules should not depend on low-level modules. Both should depend on the abstraction. Abstractions should not depend on details. Details should depend on abstractions.

*[The S.O.L.I.D Principles in Pictures](https://medium.com/backticks-tildes/the-s-o-l-i-d-principles-in-pictures-b34ce2f1e898)*
