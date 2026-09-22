<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the discrete inner product $\langle U,V\rangle_h=h\sum_{m=1}^{J-1}\overline U_mV_m$, with endpoints $U_0=U_J=0$. The centered first-difference [matrix](../../../../../../matrix.md) $D_x$ is skew-Hermitian, while [summation by parts](../../../../../../abel-s-summation-formula.md) gives

$$
\operatorname{Re}\langle U,D_{xx}U\rangle_h=-\frac1h\sum_{m=0}^{J-1}|U_{m+1}-U_m|^2.
$$

Since $\alpha$ is real, the centered advection contribution has zero real part. Therefore

$$
\boxed{\frac{d}{dt}\|U\|_h^2=-\frac2h\sum_{m=0}^{J-1}|U_{m+1}-U_m|^2\leq0.}
$$

This proves the [energy contraction for centered drift-diffusion](../../../../../../energy-contraction-for-centered-drift-diffusion.md), and hence [stability](../../../../../../stability-of-a-numerical-method.md) for every fixed real $\alpha$ and every mesh width, in the [discrete L2 norm](../../../../../../discrete-l2-norm.md). The extra inequality $|\alpha|h\leq2$ would make the off-diagonal coefficients nonnegative and support a discrete maximum principle, but is not needed for this energy proof. No time-stepping method is involved here.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
