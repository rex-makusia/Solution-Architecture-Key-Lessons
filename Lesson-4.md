## 4. Clean Architecture (Robert C. Martin)

### Book Context
Architectural philosophy emphasizing separation of concerns, dependency management, and business logic independence from frameworks, databases, and external systems.

### Key Principles
- **Independence**: Architecture should be independent of frameworks, UI, databases, and external agencies
- **Testability**: Business rules can be tested without UI, databases, web servers, or external elements
- **UI Independence**: The UI can change without changing the rest of the system
- **Database Independence**: Business rules are not bound to any particular database
- **External Agency Independence**: Business rules don't know anything about the outside world

### Key Practices
- **Dependency inversion**: Make dependencies point inward toward business logic, not outward toward infrastructure
- **Interface segregation**: Create focused interfaces that serve specific client needs
- **Separation of concerns**: Keep business logic separate from presentation, persistence, and external integrations
- **Screaming architecture**: Make the architecture clearly express what the system does, not what frameworks it uses
- **Plugin architecture**: Treat databases, web frameworks, and external services as plugins to the core business logic

### Key Patterns/Models
- **Clean Architecture Layers**: Entities (Enterprise Business Rules), Use Cases (Application Business Rules), Interface Adapters, Frameworks & Drivers
- **Dependency Rule**: Dependencies can only point inward, toward higher-level policies
- **Boundaries**: Clear separations between different levels of abstraction and concern
- **Controllers and Presenters**: Interface adapters that convert data between use cases and external interfaces
- **Gateways and Repositories**: Abstractions for external data sources and services

### Architectural Relevance
Provides a framework for building systems that are maintainable, testable, and independent of external dependencies, crucial for long-lived enterprise systems.

### Quick Examples
- **Banking**: Core banking logic independent of web interface, database choice, or external payment processors
- **E-commerce**: Order processing use cases that work regardless of whether accessed via web, mobile, or API
- **Microservices**: Each service following clean architecture with business logic independent of HTTP, messaging, or database choices
- **Cloud Migration**: Business logic that can easily migrate between cloud providers or deployment models

### Reflection Questions
How can you restructure your architecture so that business rules are completely independent of delivery mechanisms and data sources? What would it take to swap out your database or web framework?

---
