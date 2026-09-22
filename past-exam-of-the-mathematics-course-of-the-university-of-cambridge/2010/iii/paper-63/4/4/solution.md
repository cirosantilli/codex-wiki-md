<h1 id="4/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**The tableau as printed is not a collocation tableau.** Its second stage row is $(3/4,3/4)$, whose sum is $3/2$, while the corresponding printed node is $1$. This violates the [collocation tableau row-sum identity](../../../../../../collocation-tableau-row-sum-identity.md). The original PDF confirms this coefficient; it is not only a TeX transcription defect.

The required integrated basis at nodes $1/3,1$ is

$$
\ell_1(\tau)=\tfrac32(1-\tau),\qquad \ell_2(\tau)=\tfrac12(3\tau-1),
$$

so direct integration gives

$$
A=\begin{pmatrix}5/12&-1/12\\3/4&1/4\end{pmatrix},\qquad
b=\begin{pmatrix}3/4\\1/4\end{pmatrix},\qquad
c=\begin{pmatrix}1/3\\1\end{pmatrix}.
$$

Thus **replacing the last stage coefficient by $1/4$ gives the intended two-stage Radau IIA collocation method**. Its quadrature moments are

$$
b^T\mathbf1=1,\quad b^Tc=\tfrac12,\quad b^Tc^2=\tfrac13,
\quad b^Tc^3=\tfrac5{18}\ne\tfrac14.
$$

It integrates quadratics exactly but not cubics, so the [collocation order theorem](../../../../../../collocation-order-theorem.md) gives **order three**. Independently, $b^TAc=1/6$, confirming the remaining third-order [Butcher order condition](../../../../../../butcher-order-condition.md).

For completeness the literal printed [Runge-Kutta method](../../../../../../runge-kutta-method.md) has only **order one**. For the autonomous equation $y'=y$, the [Taylor expansion](../../../../../../taylor-expansion.md) of its [stability function](../../../../../../stability-function.md) begins

$$
R(z)=1+z+(b^TA\mathbf1)z^2+O(z^3)
=1+z+\frac58z^2+O(z^3),
$$

whereas $e^z=1+z+z^2/2+O(z^3)$. Since $b^T\mathbf1=1$, it is consistent, but this discrepancy already rules out order two. Therefore neither the requested equivalence nor the third-order conclusion is true without the stated coefficient repair.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [4](../../4.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
