<h1 id="a/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [cosine](../../../../../cosine.md) mode in the question, the [Laplacian](../../../../../laplacian.md) acts by multiplication by $-s$, where

$$
s=k_{n,m}^2=\pi^2\left(\frac{n^2}{L_1^2}+\frac{m^2}{L_2^2}\right).
$$

These modes obey the [Neumann boundary conditions](../../../../../neumann-boundary-condition.md). In the [chemotactic](../../../../../chemotaxis.md) term, put $q=1+u$, $c=\eta+v$. Then $\nabla c=\nabla v$, and $q\nabla c=\nabla v+u\nabla v$; the second product is a [quadratic polynomial](../../../../../quadratic-polynomial.md) in [perturbation](../../../../../perturbation.md) amplitude. Thus the [linearized equations](../../../../../linearized-equation.md) are

$$
u_t=\alpha\nabla^2u-\beta\nabla^2v-u,\qquad
v_t=\nabla^2v+\kappa\eta u-\kappa v.
$$

Substituting the modal time dependence gives

$$
\lambda\begin{pmatrix}q_{n,m}\\c_{n,m}\end{pmatrix}
=\begin{pmatrix}-1-\alpha s&\beta s\\\kappa\eta&-\kappa-s\end{pmatrix}
\begin{pmatrix}q_{n,m}\\c_{n,m}\end{pmatrix}.
$$

Separating this [matrix](../../../../../matrix.md) into its transport part and the reaction [Jacobian matrix](../../../../../jacobian-matrix.md) gives the required form, with the same $J$ as above.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../split.md)
6. [Topics in applied mathematics course of the University of Oxford](../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
