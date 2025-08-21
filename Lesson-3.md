## 3. Domain-Driven Design: Tackling Complexity in the Heart of Software (Eric Evans)

### Book Context
Strategic approach to software design that places the business domain and domain experts at the center of the design process, using tactical patterns to implement complex business logic effectively.

### Key Principles
- **Ubiquitous Language**: Develop a shared vocabulary between technical and business teams that is reflected in the code
- **Domain-Centric Design**: Structure software around business concepts and processes rather than technical concerns
- **Bounded Context**: Define clear boundaries where domain models apply and manage relationships between contexts
- **Continuous Learning**: Treat domain modeling as an ongoing learning process that deepens understanding over time
- **Context Mapping**: Explicitly define relationships and integration patterns between different bounded contexts

### Key Practices
- **Collaborative modeling**: Work directly with domain experts to develop and refine the domain model
- **Model refinement**: Continuously refine the domain model based on new insights and changing requirements
- **Context boundary definition**: Clearly define and enforce boundaries between different business contexts
- **Strategic design**: Make deliberate decisions about how different parts of the system relate and integrate
- **Tactical pattern application**: Use DDD tactical patterns to implement complex domain logic effectively

### Key Patterns/Models
- **Strategic**: Bounded Context, Context Map, Shared Kernel, Customer-Supplier, Anticorruption Layer
- **Tactical**: Entity, Value Object, Domain Service, Repository, Aggregate, Factory
- **Architecture**: Layered Architecture, Hexagonal Architecture, Domain Events, Application Service
- **Integration**: Published Language, Open Host Service, Separate Ways, Big Ball of Mud

### Architectural Relevance
Critical for systems with complex business logic where the primary challenge is understanding and modeling the business domain rather than technical complexity.

### Quick Examples
- **Banking**: Account aggregate with business rules, Customer context separate from Loan context
- **E-commerce**: Order aggregate managing business invariants, Product Catalog context vs. Inventory context
- **Insurance**: Policy aggregate with underwriting rules, Claims context with separate bounded context
- **Healthcare**: Patient aggregate with privacy rules, separate contexts for billing, treatment, and records

### Reflection Questions
How can you identify and define the bounded contexts in your business domain? What ubiquitous language exists or needs to be developed with your domain experts?

---
