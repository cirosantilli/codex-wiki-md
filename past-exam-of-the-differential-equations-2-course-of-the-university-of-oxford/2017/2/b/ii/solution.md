<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Match the coefficient of $y'$ with the [derivative](../../../../../derivative.md) of the coefficient of $y''$. For [Sturm-Liouville form](../../../../../sturm-liouville-form.md) this requires

$$
(rx^2)'=-rx,\qquad x^2r'+3xr=0.
$$

A positive [integrating factor](../../../../../integrating-factor.md) is therefore $r(x)=x^{-3}$, with any positive constant multiple equally valid. Direct calculation gives

$$
\boxed{r=x^{-3},\qquad\widehat Ly=(x^{-1}y')'+x^{-3}y.}
$$

This uses the plus-divergence sign convention of the question. The usual minus-divergence [Sturm-Liouville operator](../../../../../sturm-liouville-operator.md) is its negative; no extra sign is inserted into the requested [eigenvalue](../../../../../eigenvalue.md) equation.

Because $r$ never vanishes on the [interval](../../../../../interval-mathematics.md), multiplying the original [eigenvalue](../../../../../eigenvalue.md) equation by $r$ leaves the requested weighted [eigenvalue](../../../../../eigenvalue.md) problem unchanged:

$$
\boxed{\widehat\lambda_k=-k^2\pi^2,\qquad\widehat y_k=x\sin(k\pi\log x).}
$$

The weight in the [inner product](../../../../../inner-product-split.md) is essential. The substitution $t=\log x$ gives

$$
\int_1^e r\widehat y_j\widehat y_k\,dx
=\int_0^1\sin(j\pi t)\sin(k\pi t)\,dt
=\begin{cases}\tfrac12,&j=k,\\0,&j\ne k.\end{cases}
$$

Thus [orthogonality of Sturm-Liouville eigenfunctions](../../../../../orthogonality-of-sturm-liouville-eigenfunctions.md) holds for the [weighted inner product](../../../../../weighted-inner-product.md) with weight $x^{-3}$, and the squared [norm](../../../../../norm.md) is $N_k=1/2$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
