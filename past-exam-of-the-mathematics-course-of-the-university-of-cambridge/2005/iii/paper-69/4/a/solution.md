<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The nodes are $c=(0,1/2,1)^T$. Their [Lagrange interpolation](../../../../../../lagrange-polynomial.md) basis on the normalized step is

$$
\ell_1(s)=2s^2-3s+1,\quad \ell_2(s)=4s-4s^2,\quad \ell_3(s)=2s^2-s.
$$

Integrating these polynomials from zero to each node gives $a_{ij}=\int_0^{c_i}\ell_j(s)ds$. At $c_1=0$ the row vanishes; at $c_2=1/2$ the integrals are $(5/24,1/3,-1/24)$; at $c_3=1$ they are $(1/6,2/3,1/6)$. The endpoint integrals also give $b=(1/6,2/3,1/6)^T$. These are exactly the coefficients in the original PDF.

Indeed, the degree-three polynomial $q$ determined by $q(0)=y_n$ and $q'(hs)=\sum_j\ell_j(s)f(q(hc_j))$ satisfies $q'(hc_i)=f(q(hc_i))$. Integrating it to the nodes gives precisely the stage equations, and integrating to the endpoint gives the update. This proves it is a [collocation Runge-Kutta method](../../../../../../collocation-runge-kutta-method.md), specifically the three-stage [Lobatto IIIA method](../../../../../../lobatto-iiia-method.md).

For an explicit order proof, the collocation integrals imply $A\mathbf1=c$, $Ac=c^2/2$ and $Ac^2=c^3/3$, with powers componentwise. The endpoint weights are Simpson weights, so $b^Tc^j=1/(j+1)$ for $j=0,1,2,3$. Therefore the eight [Butcher order conditions](../../../../../../butcher-order-condition.md) through order four are satisfied:

$$
\begin{gathered}
b^T\mathbf1=1,\quad b^Tc=\tfrac12,\quad b^Tc^2=\tfrac13,\quad b^TAc=\tfrac16,\\
b^Tc^3=\tfrac14,\quad b^T\operatorname{diag}(c)Ac=\tfrac18,\quad
b^TAc^2=\tfrac1{12},\quad b^TA^2c=\tfrac1{24}.
\end{gathered}
$$

For example the last expression is $b^Tc^3/6$, because $A^2c=Ac^2/2=c^3/6$. These conditions are obtained by matching all elementary differential terms through degree four in the exact and numerical [Taylor expansions](../../../../../../taylor-expansion.md), not just by testing a scalar linear equation. Nonautonomous equations are included by adjoining $t'=1$.

To exclude higher order, the scalar [stability function](../../../../../../stability-function.md) computed below satisfies $R(z)-e^z=-z^5/720+O(z^6)$. The local defect is therefore nonzero at degree five even on the scalar test equation. Hence **$\boxed{\text{the classical order is exactly }4}$**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
