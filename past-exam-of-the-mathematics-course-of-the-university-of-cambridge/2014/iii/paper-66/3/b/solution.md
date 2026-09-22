<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Lagrange interpolation](../../../../../../lagrange-polynomial.md) polynomials for these nodes are

$$
\ell_1(\tau)=2\tau^2-3\tau+1,\qquad
\ell_2(\tau)=4\tau-4\tau^2,\qquad
\ell_3(\tau)=2\tau^2-\tau.
$$

Their integrals give the [Lobatto IIIA method](../../../../../../lobatto-iiia-method.md) tableau

$$
\boxed{\begin{array}{c|ccc}
0&0&0&0\\
1/2&5/24&1/3&-1/24\\
1&1/6&2/3&1/6\\ \hline
&1/6&2/3&1/6
\end{array}.}
$$

To verify its nonlinear order, not just its scalar linear order, set $e=(1,1,1)^T$, $c=Ae$ and $C=\operatorname{diag}(c)$. Direct multiplication verifies the [fourth-order conditions for a Runge-Kutta method](../../../../../../fourth-order-conditions-for-a-runge-kutta-method.md):

$$
b^Te=1,\quad b^Tc=\frac12,\quad b^Tc^2=\frac13,\quad
b^TAc=\frac16,\quad b^Tc^3=\frac14,\quad
b^TCAc=\frac18,\quad b^TAc^2=\frac1{12},\quad
b^TA^2c=\frac1{24}.
$$

Powers of $c$ are componentwise. These eight [Butcher order conditions](../../../../../../butcher-order-condition.md) establish order at least four for general smooth ODEs. On the [Dahlquist test equation](../../../../../../dahlquist-test-equation.md), elimination of the stages gives

$$
R(z)=\frac{1+z/2+z^2/12}{1-z/2+z^2/12},\qquad
R(z)-e^z=-\frac{z^5}{720}+O(z^6).
$$

A nonzero fifth-order step defect rules out order five. Thus **the method has exactly order four**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
