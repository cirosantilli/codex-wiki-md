<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A useful additional mode is **base plus [scaled register indexing](../../../../../scaled-index-addressing.md)**, with effective address $B+(I\ll s)$. For an [array](../../../../../array-data-structure.md) of four-byte elements choose $s=2$, use its base address on the unshifted [ALU](../../../../../arithmetic-logic-unit.md) input and its index [processor register](../../../../../processor-register.md) on the [barrel shifter](../../../../../barrel-shifter.md) input, then add. This forms an indexed [machine word](../../../../../machine-word.md) address in one [datapath](../../../../../datapath.md) pass. An eight-byte element uses $s=3$.

With parallel [ALU](../../../../../arithmetic-logic-unit.md) and [barrel shifter](../../../../../barrel-shifter.md) outputs, shifting and adding require either separate instructions/cycles or another route from the [barrel shifter](../../../../../barrel-shifter.md) to the [ALU](../../../../../arithmetic-logic-unit.md). The new serial connection supplies that route. This is an [addressing mode](../../../../../addressing-mode.md) capability, not a claim that the old instruction encoding already contains the new mode.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
