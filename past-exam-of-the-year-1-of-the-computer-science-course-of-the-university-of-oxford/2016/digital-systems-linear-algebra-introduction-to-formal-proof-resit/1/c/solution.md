<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use $w,x,y$ as the three select [bits](../../../../../bit.md) of the 8-to-1 [multiplexer](../../../../../multiplexer.md), so address $i=4w+2x+y$ selects data input $D_i$. Connect

$$
\boxed{(D_0,D_1,D_2,D_3,D_4,D_5,D_6,D_7)=(\bar z,1,z,\bar z,1,0,0,0).}
$$

A single [NOT gate](../../../../../not-gate.md) produces $\bar z$, shared by $D_0$ and $D_3$; the other connections are wires and constant logic levels. For each fixed select address the data input reproduces the corresponding two rows of the [truth table](../../../../../truth-table.md), including zeros for all invalid codes.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
