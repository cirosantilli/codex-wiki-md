<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Observer pattern](../../../../../observer-pattern.md) participants are:

- `Service`: the subject abstraction, owning the current value and registered `Company` references, and providing registration and notification operations.
- `SomeService`: the concrete subject, making `updateValue` notify after establishing the new subject state.
- `Company`: the observer [object interface](../../../../../object-interface.md), declaring the `meth()` callback.
- `PrivateCompany` and `PublicCompany`, together with the extension `NonProfit`: concrete observers, registering themselves, retaining their subject, and updating their own values on notification.

The printed `PrivateCompany` starts with factor $1$ but uses factor $1.1$ in its callback; `PublicCompany` starts with factor $0.8$ but later uses $0.9$. These are the actual source behaviors, not a uniform pricing rule inferred from their names. The subject stores a [list](../../../../../list-abstract-data-type.md) and prepends new subscriptions, so notification occurs in reverse registration order. **Dependence on the `Company` interface lets the subject notify new observer types without naming their concrete classes.** The omitted `...` portions in the printed figure do not prevent identifying these roles or implementing the added observer.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
