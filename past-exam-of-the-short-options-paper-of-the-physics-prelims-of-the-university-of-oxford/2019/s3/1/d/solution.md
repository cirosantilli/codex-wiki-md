<h1 id="s3/1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First convert from a [spectral energy density](../../../../../spectral-energy-density.md) per unit [frequency](../../../../../frequency.md) to one per unit [wavelength](../../../../../wavelength.md), including the [Jacobian matrix and determinant](../../../../../jacobian-matrix-and-determinant.md):

$$
U_\lambda=U_\nu\left|\frac{d\nu}{d\lambda}\right|=\frac{8\pi hc}{\lambda^5}\frac1{e^{hc/(\lambda k_BT)}-1}.
$$

Set $dU_\lambda/d\lambda=0$ and define $x=hc/(\lambda k_BT)$. The nonzero maximum satisfies $5(1-e^{-x})=x$, with numerical root $x=4.96511$. Consequently

$$
\boxed{\lambda_{\max}T=\frac{hc}{4.96511k_B}=2.89777\times10^{-3}\,\mathrm{m\,K}.}
$$

This is [Wien's displacement law](../../../../../wien-s-displacement-law.md). One must maximize the wavelength density, rather than find the frequency maximum and merely put $\lambda=c/\nu_{\max}$: the [frequency and wavelength peaks of Planck's law](../../../../../frequency-and-wavelength-peaks-of-planck-s-law.md) are different because a spectral density changes under a change of coordinate.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [1](../../1.md)
3. [S3](../../../s3.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the short options paper of the physics Prelims of the University of Oxford](../../../../split.md)
6. [Short options paper of the physics Prelims of the University of Oxford](../../../../../short-options-paper-of-the-physics-prelims-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
