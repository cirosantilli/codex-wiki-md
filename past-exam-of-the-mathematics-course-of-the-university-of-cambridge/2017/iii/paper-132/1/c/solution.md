<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [Gaussian curvature](../../../../../../gaussian-curvature.md) $-1$ normalization

$$
ds^2=\frac{dx^2+dy^2}{y^2}
$$

of the [Poincaré half-plane model](../../../../../../poincare-half-plane-model.md). This is a complete [conformal metric](../../../../../../conformal-metric.md), invariant under real [Möbius transformations](../../../../../../mobius-transformation.md). Its quotient by the free effective [principal congruence subgroup](../../../../../../principal-congruence-subgroup.md) is again complete: a [geodesic](../../../../../../geodesic.md) lifts to the complete covering plane and extends there for all time. Transporting the quotient metric through the [biholomorphism](../../../../../../biholomorphism.md) supplies the required complete [conformal metric](../../../../../../conformal-metric.md).

A nonconstant closed [geodesic](../../../../../../geodesic.md) corresponds to a [hyperbolic Möbius transformation](../../../../../../hyperbolic-element-of-psl2-r.md) $A$ of $\Gamma(2)$, and its [hyperbolic translation length](../../../../../../hyperbolic-translation-length.md) is $2\operatorname{arcosh}(|\operatorname{tr}A|/2)$. Indeed its [eigenvalues](../../../../../../eigenvalue.md) have magnitudes $\lambda,\lambda^{-1}$ with $\lambda>1$, and its axis quotient has length $2\log\lambda$. For $A=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ in $\Gamma(2)$, $bc\equiv0\pmod4$ implies $ad\equiv1\pmod4$. The odd numbers $a,d$ therefore have the same residue modulo four, and

$$
\operatorname{tr}A=a+d\equiv2\pmod4.
$$

A [hyperbolic Möbius transformation](../../../../../../hyperbolic-element-of-psl2-r.md) must have $|\operatorname{tr}A|>2$, so its smallest possible absolute [trace](../../../../../../matrix-trace.md) is six. It is attained by

$$
\begin{pmatrix}1&2\\0&1\end{pmatrix}
\begin{pmatrix}1&0\\2&1\end{pmatrix}
=\begin{pmatrix}5&2\\2&1\end{pmatrix}.
$$

Consequently

$$
\boxed{\ell_{\min}=2\operatorname{arcosh}3=2\log(3+2\sqrt2).}
$$

This element is primitive: a proper power would have a shorter root represented by a [hyperbolic Möbius transformation](../../../../../../hyperbolic-element-of-psl2-r.md), contradicting the [trace](../../../../../../matrix-trace.md) bound. No essential simple closed [geodesic](../../../../../../geodesic.md) exists on the three-punctured sphere, since every essential simple loop is peripheral and corresponds to a [parabolic Möbius transformation](../../../../../../parabolic-element-of-psl2-r.md). The minimizing closed [geodesic](../../../../../../geodesic.md) is therefore nonsimple. Finally, the PDF leaves the numerical [Gaussian curvature](../../../../../../gaussian-curvature.md) unspecified: the displayed length uses [Gaussian curvature](../../../../../../gaussian-curvature.md) $-1$; for [Gaussian curvature](../../../../../../gaussian-curvature.md) $-\kappa^2$, it is divided by $\kappa$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 132](../../../paper-132-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
