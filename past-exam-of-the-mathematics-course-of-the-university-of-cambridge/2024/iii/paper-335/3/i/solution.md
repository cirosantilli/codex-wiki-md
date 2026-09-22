<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $(\sigma_j,u_j,v_j)$ be a [singular system of a compact operator](../../../../../../singular-system-of-a-compact-operator.md) $A:X\to Y$, so

$$
Av_j=\sigma_ju_j,
\qquad
A^*u_j=\sigma_jv_j,
\qquad
\sigma_j>0.
$$

The [Moore–Penrose inverse of an operator](../../../../../../moore-penrose-inverse-of-an-operator.md) has domain

$$
\mathcal D(A^\dagger)
=\operatorname{ran}A\mathbin\oplus
(\operatorname{ran}A)^\perp
$$

and acts by

$$
\boxed{
A^\dagger y
=\sum_j\frac{\langle y,u_j\rangle}{\sigma_j}v_j},
$$

with the orthogonal component of $y$ sent to zero. Equivalently, its domain consists of the data satisfying the [Picard criterion](../../../../../../picard-criterion.md). It obeys

$$
AA^\dagger y=P_{\overline{\operatorname{ran}A}}y,
\qquad
A^\dagger Ax=P_{(\ker A)^\perp}x.
$$

If $Ax=y$ is exactly solvable, every solution is $x^\dagger+z$ with $z\in\ker A$, and

$$
\boxed{x^\dagger=A^\dagger y}
$$

is the unique [minimum-norm least-squares solution](../../../../../../minimum-norm-least-squares-solution.md). It recovers the component of the original $x$ orthogonal to the null space; no data can determine the null-space component.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
