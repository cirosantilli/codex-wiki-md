<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In the [first Born approximation](../../../../born-approximation.md), let $q=|\mathbf k'-\mathbf k|=2k\sin(\theta/2)$ be the transferred wave number. The angular [integral](../../../../integral-split.md) in the three-dimensional [Fourier transform](../../../../fourier-transform-split.md) is $4\pi\sin(qr)/(qr)$, so

$$
f_B(\theta)=-\frac{m}{2\pi\hbar^2}\int e^{-i\mathbf q\cdot\mathbf r}V_0\delta(r-R)\,d^3r
=-\frac{2mV_0R^2}{\hbar^2}\frac{\sin(qR)}{qR}.
$$

Writing $g=2mV_0R/\hbar^2$ and $\operatorname{sinc}u=\sin u/u$, with value one at zero, the [delta-shell Born amplitude](../../../../delta-shell-born-amplitude.md) gives

$$
\boxed{f_B=-gR\operatorname{sinc}[2kR\sin(\theta/2)],\qquad
\frac{d\sigma_B}{d\Omega}=g^2R^2\operatorname{sinc}^2[2kR\sin(\theta/2)].}
$$

For $kR\ll1$ the scattering is approximately isotropic, with total [cross section](../../../../cross-section-physics.md) $4\pi g^2R^2$. For $kR\gg1$ it has a forward lobe of angular width of order $(kR)^{-1}$ and oscillatory zeros where $2kR\sin(\theta/2)=n\pi$. At a fixed nonzero [scattering angle](../../../../scattering-angle.md), its envelope decreases as $k^{-2}$. The right-hand panel of the figure shows this angular dependence.

For real $V_0$ the first-order [scattering amplitude](../../../../scattering-amplitude.md) is real, so inserting it literally in the [optical theorem](../../../../optical-theorem.md) would predict zero total [cross section](../../../../cross-section-physics.md), contrary to its nonzero squared [modulus](../../../../modulus.md). **The first Born amplitude alone does not satisfy the optical theorem at order $V_0^2$.** This is an order-of-approximation issue: the squared first-order amplitude is already second order, and the second Born term supplies the required second-order imaginary forward amplitude. At first order both sides vanish. A weak-shell regime is needed for the Born truncation itself to be accurate.

## ↑ Ancestors (14)

1. [D](../d.md)
2. [2](../../2.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the theoretical physics II course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics II course of the University of Cambridge](../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
