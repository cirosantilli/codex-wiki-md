<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply [flow conservation](../../../../../flow-conservation.md) at the four junctions, using the directions in the original diagram:

$$
\begin{array}{rcll}
F_4+150&=&F_1& (A),\\
F_1&=&F_2+200& (B),\\
F_2+100&=&F_3& (C),\\
F_3&=&F_4+50& (D).
\end{array}
$$

The total external inflow and outflow are both 250 cars per hour. Accordingly one of these [linear equations](../../../../../linear-equation.md) is redundant. Put $F_2=t$. Successive substitution yields

$$
\boxed{(F_1,F_2,F_3,F_4)=(200+t,t,100+t,50+t),\qquad t\ge0,}
$$

in cars per hour. The [nonnegativity](../../../../../nonnegativity.md) restriction expresses clockwise traffic on every arc. Conversely, every $t\ge0$ gives nonnegative flows satisfying all four conservation equations, so this is the whole physically allowable family. Increasing $t$ adds a common [network circulation](../../../../../circulation-in-a-flow-network.md) around the roundabout without changing any external inflow or outflow.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
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
