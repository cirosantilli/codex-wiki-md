<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $s=\alpha^2+\pi^2$ and use modes satisfying all [boundary conditions](../../../../../../boundary-condition.md),

$$
\psi=a(t)\sin\alpha x\sin\pi z,\qquad
\theta=b(t)\cos\alpha x\sin\pi z+c(t)\sin2\pi z+\cdots.
$$

The quadratic [temperature](../../../../../../temperature.md) distortion $c$ is retained for the saturation calculation; it does not enter the linear onset. Substitution of the primary modes gives

$$
\frac d{dt}\begin{pmatrix}a\\b\end{pmatrix}
=\begin{pmatrix}-\sigma(s+Q\pi^2/s)&\sigma R\alpha/s\\\alpha&-s\end{pmatrix}
\begin{pmatrix}a\\b\end{pmatrix}.
$$

The [determinant](../../../../../../determinant.md) vanishes when

$$
\boxed{R_c(Q,\alpha)=\frac{s(s^2+Q\pi^2)}{\alpha^2}.}
$$

The [trace](../../../../../../matrix-trace.md) is $-[s+\sigma(s+Q\pi^2/s)]<0$. Thus no conjugate [eigenvalues](../../../../../../eigenvalue.md) can cross the imaginary axis away from zero, and **the initial instability is stationary, not oscillatory**. Indeed for $R\ge0$ the [discriminant](../../../../../../discriminant.md) is $[\sigma(s+Q\pi^2/s)-s]^2+4\sigma R\alpha^2/s>0$. This is [quasistatic vertical-field magnetoconvection](../../../../../../quasistatic-vertical-field-magnetoconvection.md): there is no independent magnetic evolution mode that could produce a magnetic-thermal [Hopf bifurcation](../../../../../../hopf-bifurcation.md) instability.

For a fixed box the other allowed horizontal [wavenumbers](../../../../../../wavenumber.md) are $n\pi/L$, and the actual first threshold is the minimum of their corresponding $R_c$ values. Vertical index $m$ replaces $\pi^2$ by $m^2\pi^2$ and strictly increases the threshold at fixed horizontal [wavenumber](../../../../../../wavenumber.md), so $m=1$ is selected. The displayed formula describes the prescribed fundamental roll; part (b) optimizes its width.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
