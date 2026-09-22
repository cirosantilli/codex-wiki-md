<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The required time separation is $\tau\ll t_{\mathrm{sec}}$, where $t_{\mathrm{sec}}$ is the evolution timescale of $f_0$, together with $t_{\mathrm{peak}}\gg\tau$ and an observation time well after the pulse. The first condition permits freezing $f_0(\mathbf J,t')$ at its pre-pulse value; its neglected change would enter beyond the retained second order. The second makes the original initial time lie in a negligible tail of the [Gaussian function](../../../../gaussian-function.md), permitting replacement of the lower time limits by $-\infty$. Short duration alone would not justify that replacement for a pulse centered at the initial time.

Integrate the [continuity equation](../../../../continuity-equation.md) in [c](../c.md) over the whole pulse. For fixed $\mathbf J$, the time factor is the [ordered Gaussian response integral](../../../../ordered-gaussian-response-integral.md)

$$
\mathcal I(\omega)=\int_{-\infty}^{\infty}dt\int_{-\infty}^{t}dt'\,e^{-i\omega(t-t')}g(t)g(t').
$$

A common translation by $t_{\mathrm{peak}}$ removes the peak time. Pair the positive and negative azimuthal harmonics: $(-m,-k_R)$ is paired with $(m,k_R)$. Both $k_\varphi$ and $\mathbf k\cdot\partial_{\mathbf J}f_0$ change sign, so their product does not; $\omega_{-\mathbf k}=-\omega_{\mathbf k}$ makes the two time factors complex conjugates. Hence the pair contributes $2\operatorname{Re}\mathcal I$.

For completeness, the real part of the integrand is symmetric under $t\leftrightarrow t'$. The triangular time domain therefore gives half of the full plane, and the [Fourier transform](../../../../fourier-transform-split.md) of a [Gaussian function](../../../../gaussian-function.md) gives

$$
\operatorname{Re}\mathcal I(\omega)=\frac12\left|\int_{-\infty}^{\infty}g(t)e^{-i\omega t}\,dt\right|^2=\pi\tau^2e^{-\omega^2\tau^2}.
$$

This derives the supplied identity rather than requiring a separate time-ordering calculation.

Define

$$
D_{mk_R}=m\frac{\partial f_0}{\partial J_\varphi}+k_R\frac{\partial f_0}{\partial J_R}.
$$

Using the paired harmonics and $\Delta F_0=-\partial_{J_\varphi}\int Q_0\,dt$ now yields

$$
\Delta F_0=4\pi^2m\tau^2\frac{\partial}{\partial J_\varphi}\sum_{k_R}\int_0^\infty dJ_R\,|u_{mk_R}|^2D_{mk_R}e^{-\omega_{mk_R}^2\tau^2}.
$$

By the stated assumption, $\omega_{mk_R}$ is independent of $J_R$, so its exponential can be taken outside the radial [integral](../../../../integral-split.md). Put $\Gamma=(\sqrt2\tau)^{-1}$ and use

$$
\mathcal R_\Gamma(\omega)=\frac{e^{-\omega^2/(2\Gamma^2)}}{\sqrt{2\pi}\Gamma},\qquad 4\pi^2\tau^2e^{-\omega^2\tau^2}=\frac{\sqrt{8\pi^5}}{\Gamma}\mathcal R_\Gamma(\omega).
$$

Therefore

$$
\boxed{\Delta F_0=\frac{\sqrt{8\pi^5}\,m}{\Gamma}\frac{\partial}{\partial J_\varphi}\sum_{k_R}\mathcal R_\Gamma(\omega_{mk_R})\int_0^\infty dJ_R\,|u_{mk_R}|^2\left(m\frac{\partial f_0}{\partial J_\varphi}+k_R\frac{\partial f_0}{\partial J_R}\right).}
$$

The outer derivative acts on the [Gaussian resonance broadening](../../../../gaussian-resonance-broadening.md) factor as well as on the radial [integral](../../../../integral-split.md). The result describes [quasilinear diffusion in action space](../../../../quasilinear-diffusion-in-action-space.md) weighted by the squared pulse amplitude, with a detuning width $\Gamma$. A shorter pulse has broader frequency selectivity, while a longer pulse selects narrower [orbital resonances](../../../../orbital-resonance.md). If the action-space boundary flux vanishes, integrating $\Delta F_0$ over $J_\varphi$ gives zero, as required by [conservation of mass](../../../../mass-conservation.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
