<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Joining the two middle nodes makes the upper lower-network transistors, controlled by $a,c$, parallel with each other. The lower transistors, controlled by $b,d$, are also parallel. These two parallel groups are in series, so the lower conducting condition becomes $(a\lor c)\land(b\lor d)$.

Its dual upper network must be **two parallel branches, one containing the series [PMOS transistor](../../../../../pmos-transistor.md) pair $a,c$, the other the series pair $b,d$**. This is the right panel of the original drawing. Its condition is $(\neg a\land\neg c)\lor(\neg b\land\neg d)$. Merely leaving the old upper network unchanged would break [CMOS](../../../../../cmos.md) complementarity for some inputs, allowing a supply short rather than defining the required logic.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
