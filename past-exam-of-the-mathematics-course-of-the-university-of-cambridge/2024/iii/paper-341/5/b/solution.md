<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The centered spatial second difference has error $O(\Delta x^2)$. The symmetric composition

$$
e^{-i(\Delta t/2)T_h}
e^{-i\Delta t V_h}
e^{-i(\Delta t/2)T_h}
$$

is [Strang splitting](../../../../../../strang-splitting.md), so its local splitting error is $O(\Delta t^3)$ and its global time order is two. Because both semidiscrete subproblems are solved exactly, the total global error is

$$
\boxed{O(\Delta t^2+\Delta x^2).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
