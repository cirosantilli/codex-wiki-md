<h1 id="1/1/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Minimize $\|u\|_\Sigma^2$ subject to $\|u\|_2=1$. A minimizing sequence is bounded in $\Sigma$, and part 2 supplies a subsequence converging strongly in $L^2$ and weakly in $\Sigma$. The constraint survives the strong convergence, while [weak lower semicontinuity](../../../../../../../weak-lower-semicontinuity.md) of the norm shows that the limit $\psi$ attains the minimum. Since $\||\psi|\|_2=\|\psi\|_2$ and $|\nabla|\psi||\leq|\nabla\psi|$ [almost everywhere](../../../../../../../almost-everywhere.md), we may take $\psi\geq0$.

The [Lagrange multiplier](../../../../../../../lagrange-multiplier.md) equation is

$$
\int\nabla v\mathbin{\cdot}\nabla\psi+\int|x|^\alpha v\psi
=\lambda\int v\psi
\qquad(v\in\Sigma),
$$

where testing with $v=\psi$ shows that $\lambda=\|\psi\|_\Sigma^2>0$. Thus

$$
(-\Delta+|x|^\alpha)\psi=\lambda\psi
\quad\text{in }\mathcal D'(\mathbb R^d).
$$

This is the [ground-state eigenfunction of a confining Schrödinger operator](../../../../../../../ground-state-eigenfunction-of-a-confining-schrodinger-operator.md).

## ↑ Ancestors (12)

1. [5](../5.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 154](../../../../paper-154-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
