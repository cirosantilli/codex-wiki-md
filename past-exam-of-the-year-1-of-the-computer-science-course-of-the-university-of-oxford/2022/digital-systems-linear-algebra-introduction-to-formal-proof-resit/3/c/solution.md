<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Factor the common input before constructing the networks. Use an [NMOS transistor](../../../../../nmos-transistor.md) controlled by $b$ in series with parallel [NMOS transistors](../../../../../nmos-transistor.md) controlled by $a$ and $c$. Its conducting condition remains $b(a\lor c)$. The complementary upper network is a [PMOS transistor](../../../../../pmos-transistor.md) controlled by $b$ in parallel with a series chain of [PMOS transistors](../../../../../pmos-transistor.md) controlled by $a$ and $c$; its conducting condition is $\neg b\lor\neg a\neg c$.

This is the right panel in part (a). It uses **three lower plus three upper transistors, six in total instead of eight**, and needs no separate inverter or complemented external input. The [complementary CMOS network duality](../../../../../complementary-cmos-network-duality.md) ensures the same static [Boolean function](../../../../../boolean-function.md) and complementary rail connections.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
