<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The differential operator without its potential is the [diffusion generator](../../../../../../diffusion-generator.md) of the d-dimensional [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md)

$$
dX_s=dB_s-\lambda X_sds,\qquad X_0=x.
$$

Its explicit solution $X_s=e^{-\lambda s}x+\int_0^se^{-\lambda(s-r)}dB_r$ defines its path law $\mathbb P^x$ on $C([0,t];\mathbb R^d)$. For the potential $V(x)=\lambda^2|x|^2/2$ and initial function one, the [Feynman-Kac formula](../../../../../../feynman-kac-formula.md) gives the nonnegative path integral

$$
\boxed{u(t,x)=\int\exp\!\left(\frac{\lambda^2}{2}\int_0^t|\omega_s|^2ds\right)\mathbb P^x(d\omega).}
$$

The sign in the exponential is positive, because the PDE contains $+Vu$. One can first stop the diffusion in bounded balls, where the usual localized Feynman-Kac argument applies, and then examine finiteness of the resulting [expectation](../../../../../../expected-value.md). The [critical quadratic potential for the Ornstein-Uhlenbeck generator](../../../../../../critical-quadratic-potential-for-the-ornstein-uhlenbeck-generator.md) below supplies that finiteness check.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
