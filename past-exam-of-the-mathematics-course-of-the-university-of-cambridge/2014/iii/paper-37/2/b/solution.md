<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The same [weak duality](../../../../../../weak-duality.md) certificate gives the upper bound $(27+3\epsilon_2+3\epsilon_3)/5$ for every feasible point. Keep $x_2=0$ and solve the tight second and third constraints:

$$
x_1=\frac{16+4\epsilon_2-\epsilon_3}{10},\qquad x_3=\frac{2-2\epsilon_2+3\epsilon_3}{10}.
$$

These are nonnegative precisely when their numerators are nonnegative. The remaining first-constraint slack is $4+\epsilon_1-\epsilon_3/2$. All three are positive for sufficiently small perturbations, so the point is feasible and attains the bound. This illustrates [linear programming sensitivity within a fixed optimal basis](../../../../../../linear-programming-sensitivity-within-a-fixed-optimal-basis.md):

$$
\boxed{\phi(\epsilon)=\frac{27+3\epsilon_2+3\epsilon_3}5\quad\text{near }0.}
$$

More generally this expression is valid throughout the region specified by those three feasibility inequalities.

With $\epsilon_1=\epsilon_2=0$, the conditions reduce to

$$
\boxed{-\frac23\le\epsilon_3\le8.}
$$

The endpoints are included. Outside this interval the bound cannot be attained: its equality conditions require exactly the point above, which then has a negative $x_3$ or violates the first constraint. Whenever feasible, the problem attains a maximum because the first constraint and nonnegativity bound all coordinates, so its value is strictly smaller outside the interval. For $\epsilon_3<-4$ it is infeasible. Thus the range is exact, not just a sufficient neighborhood.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
