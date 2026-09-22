<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Gauss collocation coefficient construction](../../../../../../gauss-collocation-coefficient-construction.md). Find the $\nu$ [polynomial roots](../../../../../../root-of-a-polynomial.md) $c_1,\ldots,c_\nu$ of the shifted [Legendre polynomial](../../../../../../legendre-polynomial.md) $P_\nu(2c-1)$ in $(0,1)$, and form

$$
\ell_j(s)=\prod_{m\ne j}\frac{s-c_m}{c_j-c_m}.
$$

Then set

$$
\boxed{a_{ij}=\int_0^{c_i}\ell_j(s)ds,\qquad b_j=\int_0^1\ell_j(s)ds.}
$$

These are explicit [polynomial](../../../../../../polynomial-split.md) [integrals](../../../../../../integral.md). For example, if $\ell_j(s)=\sum_{r=0}^{\nu-1}d_{jr}s^r$, calculate $a_{ij}=\sum_rd_{jr}c_i^{r+1}/(r+1)$ and $b_j=\sum_rd_{jr}/(r+1)$. The resulting implicit [Gauss collocation method](../../../../../../gauss-legendre-method.md) has order $2\nu$; its [Gaussian quadrature](../../../../../../gaussian-quadrature.md) nodes integrate [polynomials](../../../../../../polynomial-split.md) through degree $2\nu-1$ exactly. The one-stage example is the [implicit midpoint rule](../../../../../../implicit-midpoint-rule.md), with $c_1=a_{11}=1/2$ and $b_1=1$. No search over nonlinear [Runge-Kutta order conditions](../../../../../../butcher-order-condition.md) systems is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
