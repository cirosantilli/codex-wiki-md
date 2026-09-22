<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $S_0$ denote the entry state. A conventional meaning for the Boolean returned by `add` is whether the call changes the [set](../../../../../set-split.md):
```
// add(elem):
//   S' = S0 union {elem}
//   result == !S0.contains(elem)

// contains(elem):
//   S' = S0
//   result == S0.contains(elem)

// size:
//   S' = S0
//   result == cardinality(S0)
```
Initially $S=\varnothing$. In particular, re-adding an existing element returns false and does not increase the size. **All operations have the stated empty [precondition](../../../../../precondition.md)** at the abstract level. The comment that `add` adds an element does not itself completely specify its Boolean result; the explicit changed/not-changed convention above completes that contract. As with any `Int`-valued size operation, exact cardinalities are understood to be representable by that result type.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
