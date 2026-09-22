<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply $1-\phi B$ to the observed process and call the result $V_t$. Then

$$
V_t=Z_t+W_t-\phi W_{t-1}.
$$

Its only nonzero [covariance](../../../../../../covariance.md) lags are

$$
A=\gamma_V(0)=\sigma_z^2+(1+\phi^2)\sigma_w^2,\qquad C=\gamma_V(1)=-\phi\sigma_w^2.
$$

Seek an invertible moving-average factor $V_t=\varepsilon_t+\vartheta\varepsilon_{t-1}$ with $\operatorname{Var}(\varepsilon_t)=\nu$. Matching these covariances requires $\nu(1+\vartheta^2)=A$ and $\nu\vartheta=C$. Solving gives

$$
\boxed{\nu=\frac{A+\sqrt{A^2-4\phi^2\sigma_w^4}}2,\qquad
\vartheta=-\frac{\phi\sigma_w^2}{\nu},\qquad\phi_{\rm AR}=\phi.}
$$

These are the three requested parameters in the positive-sign moving-average convention. For nonzero total noise [variance](../../../../../../variance-split.md),

$$
A-2|C|=\sigma_z^2+(1-|\phi|)^2\sigma_w^2>0,
$$

so $|\vartheta|<1$ and the larger quadratic root gives the invertible factor.

[Covariance](../../../../../../covariance.md) matching alone would not identify arbitrary processes in distribution. To obtain an actual representation on the given space, define

$$
\varepsilon_t=(1+\vartheta B)^{-1}V_t=\sum_{j\geq0}(-\vartheta)^jV_{t-j}.
$$

The series converges in L2. The spectrum of $V$ is $(A+2C\cos\omega)/(2\pi)=\nu|1+\vartheta e^{-i\omega}|^2/(2\pi)$, so this filtered process has constant spectrum $\nu/(2\pi)$ and is [white noise](../../../../../../white-noise.md). Thus

$$
\boxed{(1-\phi B)Y_t=(1+\vartheta B)\varepsilon_t,\qquad\varepsilon\sim\operatorname{WN}(0,\nu).}
$$

This is the [invertible ARMA factorization of an AR(1)-plus-noise process](../../../../../../invertible-arma-factorization-of-an-ar-1-plus-noise-process.md). If $\sigma_w^2=0$, it reduces to AR(1); if $\phi=0$, it reduces to [white noise](../../../../../../white-noise.md). If $\sigma_z^2=0$ and $\sigma_w^2>0$, then $\vartheta=-\phi$, the common factor cancels and $Y=W$. Therefore the orders are at most (1,1); no unnecessarily minimal-order claim is made in those degenerate cases.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
