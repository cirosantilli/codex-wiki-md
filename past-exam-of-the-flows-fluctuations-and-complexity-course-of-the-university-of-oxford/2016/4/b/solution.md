<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the source's noise terms consistently as $\eta_R,\eta_P$. Subtract the steady [mean](../../../../expected-value-split.md) to get $\dot{\delta R}=-\gamma_R\delta R+\eta_R$. Use the Fourier convention $f(t)=\int d\omega\,e^{-i\omega t}\widetilde f(\omega)/(2\pi)$. After initial transients decay,

$$
\widetilde{\delta R}(\omega)=\frac{\widetilde\eta_R(\omega)}{\gamma_R-i\omega}.
$$

Fourier transforming the stationary white-noise [covariance](../../../../covariance.md) gives

$$
\langle\widetilde\eta_R(\omega)\widetilde\eta_R(\omega')\rangle
=2\pi q_R\delta(\omega+\omega').
$$

Therefore the [RNA](../../../../ribonucleic-acid.md) fluctuation [power spectral density](../../../../power-spectral-density.md) is $S_R(\omega)=q_R/(\gamma_R^2+\omega^2)$. Its integral is the equal-time [variance](../../../../variance-split.md):

$$
\boxed{\langle\delta R^2\rangle=\int_{-\infty}^\infty\frac{d\omega}{2\pi}
\frac{q_R}{\gamma_R^2+\omega^2}=\frac{q_R}{2\gamma_R}.}
$$

The positivity of $\gamma_R$ ensures a stationary limit. The same calculation gives the [autocovariance](../../../../autocovariance.md) $\langle\delta R(t)\delta R(0)\rangle=[q_R/(2\gamma_R)]e^{-\gamma_R|t|}$: the decay rate filters the white forcing into a finite correlation time. Here the [covariance](../../../../covariance.md) convention is $q_R\delta(t-t')$; replacing it by $2D_R\delta(t-t')$ would identify $q_R=2D_R$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the flows, fluctuations and complexity course of the University of Oxford](../../../split.md)
5. [Flows, fluctuations and complexity course of the University of Oxford](../../../../flows-fluctuations-and-complexity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
