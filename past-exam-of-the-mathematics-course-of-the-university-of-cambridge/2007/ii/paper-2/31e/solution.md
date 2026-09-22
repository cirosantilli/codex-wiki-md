<h1 id="31e/solution">Solution</h1>

↑ **Parent:** [31E](../31e.md)

Orient the unit circle counterclockwise and use the standard principal-value Cauchy operator

$$
K\phi(t)=\frac1{\pi i}\operatorname{PV}\int_C\frac{\phi(\tau)}{\tau-t}\,d\tau.
$$

For a Fourier/Laurent mode $t^n$ it gives $+t^n$ when $n\ge0$ and $-t^n$ when $n<0$. This follows from the interior/exterior Cauchy projections, or by direct indentation of the pole. Decompose $\phi=\phi_++\phi_-$ into its nonnegative and negative modes, so $K\phi=\phi_+-\phi_-$. Let

$$
J=\frac1{2\pi i}\int_C(\tau+2\tau^{-1})\phi(\tau)\,d\tau=c_{-2}+2c_0.
$$

The printed equation reduces to

$$
2t\phi_++2t^{-1}\phi_--J(t+t^{-1})=2t^{-1}.
$$

Positive-power coefficients force $\phi_+=J/2$, a constant; powers at most $-2$ force $\phi_-=0$. The $t^{-1}$ coefficient then gives $-J=2$, and the integral definition is consistent with $c_0=-1$. Thus

$$
\boxed{\phi(t)=-1\quad(t\in C).}
$$

Direct substitution has $K\phi=-1$, $J=-2$ and gives $2t^{-1}$ as required. The same projection argument on the homogeneous equation forces $J=0$ and both components zero, proving uniqueness in the usual Hölder or $L^2$ class for this singular-integral problem.

## ↑ Ancestors (10)

1. [31E](../31e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
