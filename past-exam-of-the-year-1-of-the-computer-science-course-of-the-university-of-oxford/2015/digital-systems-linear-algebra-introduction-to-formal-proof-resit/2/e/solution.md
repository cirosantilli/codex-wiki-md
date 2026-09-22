<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The custom [CMOS](../../../../../cmos.md) circuit uses eight [NMOS transistors](../../../../../nmos-transistor.md) and eight [PMOS transistors](../../../../../pmos-transistor.md) in the output networks, plus eight [transistors](../../../../../transistor.md) in the four input [CMOS inverters](../../../../../cmos-inverter.md):

$$
\boxed{N=8+8+4\cdot2=24\text{ transistors}.}
$$

The complementary types give an actively driven output at either supply rail. An [NMOS transistor](../../../../../nmos-transistor.md) provides a strong connection to ground; a [PMOS transistor](../../../../../pmos-transistor.md) provides a strong connection to $V_{DD}$. An [NMOS transistor](../../../../../nmos-transistor.md) used alone to pass a high level loses gate overdrive as the output rises, giving a threshold-degraded high level; the complementary problem affects a [PMOS transistor](../../../../../pmos-transistor.md) passing a low level. Complementary networks avoid these degraded levels and, ideally, have no direct supply-to-ground conducting path for a stable input. Physical leakage and switching current remain, but a resistive load and its continuous static current are unnecessary.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
