<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Every [AND gate](../../../../../and-gate.md) and [OR gate](../../../../../or-gate.md) is a [monotone Boolean function](../../../../../monotone-boolean-function.md): changing an input from zero to one while leaving all other inputs unchanged cannot change the output from one to zero. By [structural induction](../../../../../structural-induction.md) over a [Boolean circuit](../../../../../boolean-circuit.md), a composition of these gates is also a [monotone Boolean function](../../../../../monotone-boolean-function.md). Constant inputs do not alter that conclusion.

**[Logical negation](../../../../../negation.md) cannot be implemented**, since it sends $0$ to $1$ and $1$ to $0$, violating the defining order property. Hence these two gate types alone cannot implement every [Boolean function](../../../../../boolean-function.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
