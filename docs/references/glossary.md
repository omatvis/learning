# Glossary

> Short definitions of terms used throughout this learning path.

| Term | Definition |
|------|-----------|
| **CQRS** | Command Query Responsibility Segregation — separating read and write operations |
| **Clean Architecture** | Layered architecture with strict dependency rules: Domain ← Application ← Infrastructure / Api |
| **DTO** | Data Transfer Object — a plain object used to carry data between layers or over the wire |
| **DI** | Dependency Injection — providing dependencies to a class rather than constructing them inside it |
| **EF Core** | Entity Framework Core — .NET ORM for database access |
| **Minimal API** | ASP.NET Core feature for defining HTTP endpoints without controllers |
| **N+1** | A query pattern where 1 query fetches a list and then N queries fetch related data for each item |
| **ORM** | Object-Relational Mapper — maps database rows to in-memory objects |
| **PR** | Pull Request — a request to merge a branch; used here as an exercise review mechanism |
| **Parameterised query** | A SQL query where user input is passed as a parameter, not concatenated into the string |
| **Soft delete** | Marking a record as deleted (e.g. `IsDeleted = true`) without removing it from the database |
| **SPA** | Single-Page Application — a web app that renders in the browser (e.g. React) |
| **Use-case** | An application-layer class that orchestrates one specific business action |
