<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The assignment equalities parameterize every feasible [matrix](../../../../matrix.md) of the [linear programming relaxation](../../../../linear-programming-relaxation.md) as

$$
x(t)=\begin{pmatrix}t&1-t\\1-t&t\end{pmatrix},\qquad0\leq t\leq1.
$$

The side totals and objective become

$$
a\cdot x=3+t,\qquad b\cdot x=6-t,\qquad c\cdot x=8+2t.
$$

The first side constraint gives $t\leq1/2$ and the second gives $t\geq1/2$, so the relaxation has the unique [feasible point](../../../../feasible-point.md)

$$
\boxed{x_{ij}=1/2\quad\text{for all }i,j,\qquad z_{LP}=9.}
$$

Direct elimination of the assignment equalities has solved this one-dimensional [linear program](../../../../linear-programming-split.md). Its value matches the [Lagrangian dual problem](../../../../lagrangian-dual-problem.md) value because the retained assignment polytope is the [convex hull](../../../../convex-hull.md) of the two [integer](../../../../integer-split.md) assignments; it does not make the side-constrained [integer](../../../../integer-split.md) problem feasible.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the integer programming course of the University of Oxford](../../../split.md)
5. [Integer programming course of the University of Oxford](../../../../integer-programming-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
