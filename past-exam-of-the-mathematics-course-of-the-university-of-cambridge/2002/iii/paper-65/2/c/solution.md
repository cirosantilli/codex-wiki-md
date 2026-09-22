<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the same [metric signature](../../../../../../metric-signature.md) as above and define the Minkowski [generating functional](../../../../../../generating-functional.md) by

$$
Z_0[J]=\int\mathcal D\phi\,
\exp\left(iS_0[\phi]+i\int d^dx\,J\phi\right).
$$

Here $\hbar=1$. [Integration by parts](../../../../../../integration-by-parts.md) writes the quadratic action as $S_0=\tfrac12\phi K\phi$ with $K=-\Box-m^2+i0$; the infinitesimal imaginary part damps the oscillatory [Gaussian functional integral](../../../../../../gaussian-functional-integral.md) and selects the vacuum [Feynman propagator](../../../../../../feynman-propagator.md). Abbreviating repeated spacetime integrations, [completing the square](../../../../../../completing-the-square.md) gives

$$
\frac12\phi K\phi+J\phi
=\frac12(\phi+K^{-1}J)K(\phi+K^{-1}J)-\frac12JK^{-1}J.
$$

Translation of the regulated integration variables therefore yields

$$
\boxed{Z_0[J]=Z_0[0]\exp\left[-\frac i2\int dx\,dy\,J(x)K^{-1}(x,y)J(y)\right].}
$$

The source-independent normalization contains the regulated [functional determinant](../../../../../../functional-determinant.md) and its oscillatory phase; it cancels in $Z_0[J]/Z_0[0]$. Define $\Delta_F=iK^{-1}$. The [Gaussian evaluation of a free scalar generating functional](../../../../../../gaussian-evaluation-of-a-free-scalar-generating-functional.md) is equivalently $Z_0[J]/Z_0[0]=\exp[-J\Delta_FJ/2]$.

With Fourier convention $e^{-ip\cdot x}$, $-\Box$ acts as $p^2$. The inverse-kernel equation $KK^{-1}=I$ then gives

$$
\boxed{\widetilde\Delta_F(p)=\frac{i}{p^2-m^2+i0},\qquad
\Delta_F(x-y)=\int\frac{d^dp}{(2\pi)^d}\,
\frac{i\,e^{-ip\cdot(x-y)}}{p^2-m^2+i0}.}
$$

This is the time-ordered free two-point [correlation function](../../../../../../correlation-function.md): differentiating twice with respect to $J$ and multiplying by $1/i^2$ recovers $\Delta_F$. It obeys $(\Box+m^2)\Delta_F=-i\delta^{(d)}$ in the distributional limit. The $i0$ is essential: the algebraic denominator alone would not distinguish Feynman, advanced and retarded [Green functions](../../../../../../green-s-function.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
