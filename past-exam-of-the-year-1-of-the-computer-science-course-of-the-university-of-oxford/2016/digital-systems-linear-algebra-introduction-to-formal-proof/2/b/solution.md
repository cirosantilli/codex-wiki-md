<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Split the four-[bit](../../../../../bit.md) unsigned inputs into two-[bit](../../../../../bit.md) halves: $X=4X_H+X_L$ and $Y=4Y_H+Y_L$. Use four copies of the two-[bit](../../../../../bit.md) [binary multiplier](../../../../../binary-multiplier.md) to compute $P_{LL}=X_LY_L$, $P_{HL}=X_HY_L$, $P_{LH}=X_LY_H$, and $P_{HH}=X_HY_H$. Then

$$
\boxed{XY=P_{LL}+4P_{HL}+4P_{LH}+16P_{HH}.}
$$

The extreme terms occupy disjoint output positions: $P_{LL}$ uses positions zero to three and $16P_{HH}$ uses positions four to seven. Form $W$ by concatenating their four-[bit](../../../../../bit.md) outputs, with $P_{HH}$ in the upper half and $P_{LL}$ in the lower half. This needs wiring alone, so $W=16P_{HH}+P_{LL}$ without an [adder](../../../../../adder.md).

Use the first eight-[bit](../../../../../bit.md) [adder](../../../../../adder.md) to form $R=P_{HL}+P_{LH}$ after zero-extension, and the second to form $Z=W+(R\ll2)$. Thus **four two-[bit](../../../../../bit.md) [binary multipliers](../../../../../binary-multiplier.md) and two eight-[bit](../../../../../bit.md) [adders](../../../../../adder.md) suffice**. The fixed [left bit shift](../../../../../left-bit-shift.md) is also wiring alone.

The middle sum can reach $9+9=18$, so preserve all five of its potentially nonzero [bits](../../../../../bit.md); retaining only four would be wrong. Its shifted value is at most 72. The final result is at most $15\times15=225$, so both additions fit in eight [bits](../../../../../bit.md). Concatenating the disjoint extreme terms is what saves an addition.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
