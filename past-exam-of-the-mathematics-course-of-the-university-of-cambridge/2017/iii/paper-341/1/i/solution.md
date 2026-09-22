<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Lagrange interpolation polynomials](../../../../../../lagrange-polynomial.md) at $c_1=1/3$ and $c_2=1$ are

$$
\ell_1(s)=\frac32(1-s),\qquad \ell_2(s)=\frac32s-\frac12.
$$

Their [integrals](../../../../../../integral.md) give

$$
\left(\int_0^{c_i}\ell_j(s)\,ds\right)_{ij}
=\begin{pmatrix}5/12&-1/12\\3/4&1/4\end{pmatrix},
\qquad
\left(\int_0^1\ell_j(s)\,ds\right)_j=(3/4,1/4).
$$

Thus the coefficients are exactly those of a [collocation Runge-Kutta method](../../../../../../collocation-runge-kutta-method.md). More explicitly, with stage slopes $F_j=f(t_n+c_jh,Y_j)$, the degree-two [polynomial](../../../../../../polynomial-split.md)

$$
p(t_n+sh)=y_n+h\sum_{j=1}^2F_j\int_0^s\ell_j(r)\,dr
$$

satisfies $p(t_n)=y_n$, $p(t_n+c_ih)=Y_i$, and $p'(t_n+c_ih)=F_i$. These are the [collocation Runge-Kutta method](../../../../../../collocation-runge-kutta-method.md) equations, and $y_{n+1}=p(t_n+h)$. For an [implicit Runge-Kutta method](../../../../../../implicit-runge-kutta-method.md), the nearby stages exist uniquely for sufficiently small $h$ under [Lipschitz continuity](../../../../../../lipschitz-continuity.md); see [stage solvability of an implicit Runge-Kutta method](../../../../../../stage-solvability-of-an-implicit-runge-kutta-method.md).

Write $e=(1,1)^T$, $c=Ae$, and interpret powers of $c$ componentwise. The [Butcher order conditions](../../../../../../butcher-order-condition.md) through degree three are verified directly:

$$
b^Te=1,\qquad b^Tc=\frac12,\qquad b^Tc^2=\frac13,\qquad b^TAc=\frac16.
$$

For the last equality, $Ac=(1/18,1/2)^T$. However, the necessary degree-four [Butcher order condition](../../../../../../butcher-order-condition.md) fails:

$$
b^Tc^3=\frac{5}{18}\ne\frac14.
$$

Consequently, for sufficiently smooth [ordinary differential equations](../../../../../../ordinary-differential-equation.md), the [local truncation error](../../../../../../local-truncation-error.md) is $O(h^4)$ and the [order of a Runge-Kutta method](../../../../../../order-of-a-runge-kutta-method.md) is exactly

$$
\boxed{p=3}.
$$

This is the two-stage [Radau IIA method](../../../../../../radau-iia-method.md); the conclusion follows from the explicit calculations rather than its name.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
