<h1 id="18h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose an optimal feasible vector $x$ having as few positive coordinates as possible, and let

$$
S=\{i:x_i>0\}.
$$

If the columns $(A_i)_{i\in S}$ were linearly dependent, there would be a nonzero vector $h$, supported on $S$, such that $Ah=0$. For all sufficiently small positive $\varepsilon$, both

$$
x+\varepsilon h
\quad\hbox{and}\quad
x-\varepsilon h
$$

would remain feasible.

If $c^Th\ne0$, one of these two perturbations would increase the objective, contradicting optimality. Hence $c^Th=0$. We may then increase $\varepsilon$ in one of the two directions until at least one positive coordinate first becomes zero. The resulting vector is still feasible and optimal but has smaller positive support, contradicting the choice of $x$.

**Thus the active columns are linearly independent, so $x$ is basic. This proves the [Fundamental theorem of linear programming](../../../../../../fundamental-theorem-of-linear-programming.md): whenever the finite maximum is attained, an optimal basic feasible solution exists.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [18H](../../18h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
