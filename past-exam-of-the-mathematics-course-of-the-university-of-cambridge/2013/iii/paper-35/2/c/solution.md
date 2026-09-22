<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Start with six program sequences: $ABCABC$, $ACBACB$, $BACBAC$, $BCABCA$, $CABCAB$ and $CBACBA$. This gives two appearances of each program per row and per column. It also balances transitions: each ordered pair of distinct programs occurs five times across all adjacent sessions.

Apply [restricted randomization](../../../../../../restricted-randomization.md) by randomly assigning the six sequences to the six volunteers and independently permuting the three program labels. Using the supplied numbers, rank the first six from smallest to largest: the sequence indices are $(4,1,5,2,3,6)$. Assign these, in order, to volunteers 1 through 6. Rank the next three numbers attached to symbols $(A,B,C)$: their order is $(B,C,A)$. Assign actual program labels $(A,B,C)$ to these ordered symbols, so base $A\mapsto C$, base $B\mapsto A$, base $C\mapsto B$. The final **ready-to-use randomized [row-column design](../../../../../../row-column-design.md)** is:

| Volunteer | Wednesday 1 | Wednesday 2 | Wednesday 3 | Wednesday 4 | Wednesday 5 | Wednesday 6 |
| --- | --- | --- | --- | --- | --- | --- |
| 1 | A | B | C | A | B | C |
| 2 | C | A | B | C | A | B |
| 3 | B | C | A | B | C | A |
| 4 | C | B | A | C | B | A |
| 5 | A | C | B | A | C | B |
| 6 | B | A | C | B | A | C |

Programs retain their real identities after this label permutation. The researcher should follow the table across chronological afternoons; arbitrary column permutations are deliberately excluded so that transition balance survives. Each program receives twelve sessions and occurs twice in every block. Under the additive block model, the [analysis of variance](../../../../../../analysis-of-variance.md) has row, column, program and residual [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md) $5,5,2,23$, respectively, besides the grand mean. Transition balance is useful against differential [carryover effects](../../../../../../carryover-effect.md), but is not a proof that they are absent.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
