# sp-01 — C# Console Katas

> **Goal:** Get comfortable with C# fundamentals through short, focused console exercises.

## Project folder

`projects/small/sp-01-csharp-katas/`

## Katas

1. **FizzBuzz** — classic; focus on clean code and modern C# syntax.
2. **Fibonacci** — recursive vs iterative; benchmark with `Stopwatch`.
3. **LINQ pipeline** — transform a list of objects using LINQ (filter, map, sort, group).
4. **Async kata** — fetch data from a free public API using `HttpClient` and `async/await`.
5. **Nullable safety** — refactor a method with potential null-reference issues; use nullable annotations.

## Acceptance criteria (all katas)

- [ ] Code compiles and runs without warnings.
- [ ] Nullable reference types are enabled (`<Nullable>enable</Nullable>`).
- [ ] No `.Result` / `.Wait()` calls.
- [ ] At least one unit test per kata using xUnit.

## Branch convention

`exercise/sp-01-<kata-name>`
