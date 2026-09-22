<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an [infrared-regulated phase covariance](../../../../../infrared-regulated-phase-covariance.md), fix the uniform [order-parameter phase](../../../../../order-parameter-phase.md) zero mode and introduce ultraviolet and [infrared cutoffs](../../../../../infrared-cutoff.md) before taking limits. With the Fourier convention

$$
\theta(\mathbf x)=\int\frac{d^dq}{(2\pi)^d}\,\theta_{\mathbf q}e^{i\mathbf q\cdot\mathbf x},
$$

the dimensionless quadratic [Hamiltonian](../../../../../hamiltonian.md) diagonalizes as

$$
\beta H=\frac{\bar K}{2}\int\frac{d^dq}{(2\pi)^d}q^2\theta_{\mathbf q}\theta_{-\mathbf q}.
$$

Completing the square with a source gives $Z[J]/Z[0]=\exp[\tfrac12\int JGJ]$, with inverse kernel

$$
\langle\theta_{\mathbf q}\theta_{\mathbf q'}\rangle
=\frac{(2\pi)^d\delta^{(d)}(\mathbf q+\mathbf q')}{\bar Kq^2},\qquad
G(\mathbf x)=\frac1{\bar K}\int\frac{d^dq}{(2\pi)^d}\frac{e^{i\mathbf q\cdot\mathbf x}}{q^2}.
$$

There is no additional $k_BT$ factor: it is already included in $\bar K$ because the supplied [Hamiltonian](../../../../../hamiltonian.md) is $\beta H$.

It is simplest to evaluate the real-space dependence by its defining Green equation, $-\bar K\nabla^2G=\delta^{(d)}$. Rotational invariance gives $r^{d-1}G'(r)=$ constant for $r>0$. Integrating over a small [sphere](../../../../../sphere.md) fixes $-\bar KS_dr^{d-1}G'(r)=1$, where $S_d=2\pi^{d/2}/\Gamma(d/2)$. Integrating once more,

$$
\boxed{G(r)=-\frac{r^{2-d}}{(2-d)S_d\bar K}+C,\qquad d\ne2.}
$$

In two dimensions, take the limit after absorbing the divergent $r$-independent piece into $C$:

$$
\boxed{G(r)=-\frac1{2\pi\bar K}\log(r/a)+C.}
$$

For $d\le2$, $G$ itself has an infrared-divergent constant in the infinite system; it is not a finite thermodynamic [covariance](../../../../../covariance.md) without a regulator. The physical [phase-difference variance](../../../../../phase-difference-variance.md) is finite at fixed separation and cancels that constant. These are smooth [spin wave](../../../../../spin-wave.md) [correlations](../../../../../pearson-correlation-coefficient.md); compact-field [vortex](../../../../../phase-vortex.md) sectors are considered separately below.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the phase transitions and collective phenomena course of the University of Cambridge](../../../../split.md)
6. [Phase Transitions and Collective Phenomena course of the University of Cambridge](../../../../../phase-transitions-and-collective-phenomena-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
