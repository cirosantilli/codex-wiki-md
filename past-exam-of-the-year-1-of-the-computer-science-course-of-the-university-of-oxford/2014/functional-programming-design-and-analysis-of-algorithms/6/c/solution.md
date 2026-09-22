<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Dynamic programming](../../../../../dynamic-programming.md) solves related subproblems once, stores their results, and combines those results in an order consistent with their dependencies. The state must retain all information that determines the remaining choices and their costs. Here an adequate [dynamic programming state](../../../../../dynamic-programming-state.md) is the current [array](../../../../../array-data-structure.md) index, since future jumps depend only on that index and the fixed input.

The [principle of optimality](../../../../../principle-of-optimality.md) says that the remaining part of an optimal solution must be optimal for the residual problem defined by its state. Equivalently here, the prefix ending at a particular intermediate position of a shortest route must be a shortest route to that position: replacing it by a shorter prefix would shorten the entire route. This is the [optimal substructure](../../../../../optimal-substructure.md) needed by the [dynamic programming recurrence](../../../../../dynamic-programming-recurrence.md).

Thus $\boxed{\text{store an optimum for each state; combine previously solved states by an optimality recurrence}}$. Overlapping routes share states, so storing results avoids repeatedly solving the same subproblem.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
