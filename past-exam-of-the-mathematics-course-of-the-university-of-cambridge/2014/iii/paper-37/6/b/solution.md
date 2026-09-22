<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The decision problem is in [NP](../../../../../../np-complexity.md): an assignment is a certificate, and counting its satisfied [clause](../../../../../../clause-of-a-boolean-formula.md) occurrences is polynomial in the input size.

Reduce [3-SAT](../../../../../../3-sat.md) to it. For each of the $m$ original [clauses](../../../../../../clause-of-a-boolean-formula.md), use the [seven-clause gadget for MAX-2SAT](../../../../../../seven-clause-gadget-for-max-2sat.md) with its three [literals](../../../../../../boolean-literal.md) in place of $a,b,c$ and with a fresh auxiliary variable. Keep all ten [clause](../../../../../../clause-of-a-boolean-formula.md) occurrences per gadget, including any repeated occurrences across gadgets. Set the target to $k=7m$.

If the original formula is satisfiable, choose each auxiliary value as in part (a), giving seven satisfied [clauses](../../../../../../clause-of-a-boolean-formula.md) per gadget. Conversely, no gadget can exceed seven. If an assignment satisfies at least $7m$ [clauses](../../../../../../clause-of-a-boolean-formula.md) in total, every gadget must reach seven, so every original [clause](../../../../../../clause-of-a-boolean-formula.md) is satisfied by the original-variable assignment. The construction has $10m$ [clauses](../../../../../../clause-of-a-boolean-formula.md) and $m$ auxiliary variables, so is polynomial. Consequently **the decision version of [MAX-2SAT](../../../../../../maximum-2-satisfiability.md) is [NP-complete](../../../../../../np-completeness.md).**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
