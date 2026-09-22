<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use two [zero-address instructions](../../../../../zero-address-instruction.md) for indirect access to [computer memory](../../../../../computer-memory-split.md). Define `load` to replace the top [memory address](../../../../../memory-address.md) by the value at that address, and define `store` to pop a value followed by the address just beneath it:

$$
\mathrm{load}:S,p\mapsto S,M[p],\qquad\mathrm{store}:S,p,v\mapsto S\quad\text{with }M[p]\gets v.
$$

Both have no encoded address operand; the [stack](../../../../../stack-data-structure.md) supplies it. If the known fixed [memory addresses](../../../../../memory-address.md) of the variables are $p_x,p_y$, implement the assignment with
```
const p_x
const p_y
load
store
```
The successive [stack](../../../../../stack-data-structure.md) suffixes are $p_x$, then $p_x,p_y$, then $p_x,M[p_y]$, then empty. Hence

$$
\boxed{M[p_x]\gets M[p_y].}
$$

The surrounding [stack](../../../../../stack-data-structure.md) is restored. Other `store` conventions are possible, but the operand order must be stated and used consistently.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
