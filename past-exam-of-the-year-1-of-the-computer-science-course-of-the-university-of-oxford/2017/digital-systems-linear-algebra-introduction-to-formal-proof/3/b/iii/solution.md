<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For **`add`**, select `rd` and the [arithmetic logic unit](../../../../../../arithmetic-logic-unit.md) result. For **`sw`**, select destination zero while retaining the memory-store controls and source-register reads. For **`jal`**, select register 31 and the return-address data. These are the same actual register writes as before, with `sw` using destination zero in place of disabling RegWrite.

The link value is determined by the particular [MIPS architecture](../../../../../../mips-architecture.md) datapath convention: $\mathrm{PC}+4$ for the usual teaching datapath without a delay slot, or $\mathrm{PC}+8$ for classic delayed-branch MIPS. This write-enable change does not alter whichever link convention the original machine implements.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
