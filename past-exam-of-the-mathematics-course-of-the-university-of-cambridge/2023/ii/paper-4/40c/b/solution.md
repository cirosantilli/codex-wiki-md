<h1 id="40c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiate the [eigenvalue](../../../../../../eigenvalue.md) equation

$$
A(t)v(t)=\lambda(t)v(t)
$$

at $t=0$, where $A'(0)=E$. Suppressing the argument $0$ gives

$$
Ev+Av'=\lambda'v+\lambda v'.
$$

Left-multiplication by the transpose of the unit [left eigenvector](../../../../../../left-eigenvector.md) $u$ and use of $u^TA=\lambda u^T$ cancel the terms involving $v'$:

$$
u^TEv=\lambda' u^Tv.
$$

Because the eigenvalue is [simple](../../../../../../simple-eigenvalue.md), $u^Tv\ne0$, and hence the [first-order perturbation of a simple eigenvalue](../../../../../../first-order-perturbation-of-a-simple-eigenvalue.md) is

$$
\lambda'(0)=\frac{u(0)^TEv(0)}{u(0)^Tv(0)}.
$$

The definition of the [operator norm](../../../../../../operator-norm.md), followed by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), gives

$$
|u^TEv|\leq\|u\|_2\|E\|_2\|v\|_2=\|E\|_2.
$$

Therefore

$$
\boxed{|\lambda'(0)|
\leq\frac{\|E\|_2}{|u(0)^Tv(0)|}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [40C](../../40c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
