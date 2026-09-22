<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If a vector $h$ gives the strict separation, a common point would satisfy $h^Tx<h^Tx$, which is impossible.

For the converse, construct a phase-I [linear program](../../../../../../linear-programming.md) with a common violation variable:

$$
\min_{u,t}t\quad\text{subject to }Au-t\mathbf1\leq b,\quad Cu-t\mathbf1\leq d,\quad t\geq0,
$$

where $u$ is unrestricted. This [linear program](../../../../../../linear-programming.md) is feasible for sufficiently large $t$, bounded below by zero, and attains its optimum. If the two [linear polyhedra](../../../../../../linear-polyhedron.md) are disjoint, its optimum $t^*$ is strictly positive: an attained zero optimum would give a common point.

For nonnegative vectors $\lambda,\mu$, its [optimization Lagrangian](../../../../../../optimization-lagrangian.md) is

$$
L=t(1-\mathbf1^T\lambda-\mathbf1^T\mu)+u^T(A^T\lambda+C^T\mu)-\lambda^Tb-\mu^Td.
$$

Taking the infimum over $u\in\mathbb R^n$ and $t\geq0$ gives the [Lagrangian dual problem](../../../../../../lagrangian-dual-problem.md)

$$
\max_{\lambda,\mu\geq0}(-\lambda^Tb-\mu^Td)\quad\text{subject to }A^T\lambda+C^T\mu=0,\quad \mathbf1^T\lambda+\mathbf1^T\mu\leq1.
$$

By [strong duality](../../../../../../strong-duality.md) for [linear programming](../../../../../../linear-programming.md), an optimal dual pair exists and has objective $t^*>0$. It supplies the infeasibility certificate

$$
\boxed{\lambda^TA+\mu^TC=0,\qquad \lambda^Tb+\mu^Td<0,\qquad \lambda,\mu\geq0.}
$$

Take $h=A^T\lambda=-C^T\mu$. Every $x\in P$ and $y\in Q$ obeys

$$
\boxed{h^Tx\leq\lambda^Tb<-\mu^Td\leq h^Ty.}
$$

The assumed nonemptiness of each [linear polyhedron](../../../../../../linear-polyhedron.md) also ensures $h\ne0$: if $h=0$, their feasibility would force both $\lambda^Tb$ and $\mu^Td$ to be nonnegative. This proves the [strict separation of disjoint linear polyhedra](../../../../../../strict-separation-of-disjoint-linear-polyhedra.md) using [Lagrangian duality](../../../../../../lagrangian-duality.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
