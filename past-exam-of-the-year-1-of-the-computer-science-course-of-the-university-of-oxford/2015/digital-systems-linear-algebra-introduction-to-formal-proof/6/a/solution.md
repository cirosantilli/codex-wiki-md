<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [zero-address instruction](../../../../../zero-address-instruction.md) has no explicit operand addresses, so its operands and result location must be implicit in the [instruction set architecture](../../../../../instruction-set-architecture.md). A [stack machine](../../../../../stack-machine.md) supplies these naturally: operations remove their inputs from the top of an operand [stack](../../../../../stack-data-structure.md) and push the result. A fixed-[processor register](../../../../../processor-register.md) design is logically possible, so “almost certainly” is appropriately weaker than a proof that only a [stack machine](../../../../../stack-machine.md) could work.

Write the [stack](../../../../../stack-data-structure.md) from bottom to top, with its top on the right. Let $S$ stand for any unchanged prefix. Suitable effects are

$$
\boxed{\mathrm{add}:S,u,v\mapsto S,u+v,\qquad\mathrm{const}\ c:S\mapsto S,c.}
$$

Thus `add` pops two operands and pushes one [sum](../../../../../sum.md), reducing [stack](../../../../../stack-data-structure.md) occupancy by one. The special `const c` instruction pushes its immediate constant and increases occupancy by one. Only `const` needs an explicit value in its encoding.

## ↑ Ancestors (12)

1. [A](../a.md)
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
