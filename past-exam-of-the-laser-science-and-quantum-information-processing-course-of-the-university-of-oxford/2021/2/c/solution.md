<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume equal excess [electron](../../../../electron.md) and [electron hole](../../../../electron-hole.md) [number densities](../../../../number-density.md) $N_t$, with no additional doping imbalance. At zero [temperature](../../../../temperature-split.md), both occupied carrier spheres have the same [Fermi wavevector](../../../../fermi-wavevector.md) $k_F$ because their spin counting is the same:

$$
N_t=\int_0^{k_F}\frac{k^2}{\pi^2}\,dk
=\frac{k_F^3}{3\pi^2},\qquad k_F=(3\pi^2N_t)^{1/3}.
$$

For $k<k_F$, the [conduction band](../../../../conduction-band.md) is occupied and the [valence band](../../../../valence-band.md) has [electron holes](../../../../electron-hole.md), so $f_c-f_v=1$. Beyond $k_F$ the occupations reverse and the medium absorbs. Thus the upper edge of the positive-[optical gain](../../../../optical-gain.md) interval is the supremum

$$
\boxed{\hbar\omega_{\max}=E_g+\frac{\hbar^2}{2m_r}(3\pi^2N_t)^{2/3},\qquad
\beta=1+\frac{\hbar^2(3\pi^2N_t)^{2/3}}{2m_rE_g}.}
$$

Equivalently $E_{\rm Fc}=E_g+\hbar^2k_F^2/(2m_c^*)$ and $E_{\rm Fv}=-\hbar^2k_F^2/(2m_v^*)$. With the supplied [effective masses](../../../../band-effective-mass.md),

$$
\begin{aligned}
m_r&=0.0587934\,m_e,\quad k_F=3.09367\times10^8\,\mathrm{m}^{-1},\\
\hbar\omega_{\max}-E_g&\simeq0.0620214\,\mathrm{eV},\\
&\boxed{\beta\simeq1.04368,\qquad \hbar\omega_{\max}\simeq1.48202\,\mathrm{eV}.}
\end{aligned}
$$

Using the [vacuum](../../../../vacuum.md) [wavelength](../../../../wavelength.md) $\lambda=hc/(\hbar\omega)$ reverses the endpoints:

$$
\boxed{836.59\,\mathrm{nm}<\lambda<873.13\,\mathrm{nm}.}
$$

These boundaries are idealized and open: the lower-[energy](../../../../energy-split.md) edge has zero [joint density of states](../../../../joint-density-of-states.md), and the upper edge is the zero-[temperature](../../../../temperature-split.md) occupation discontinuity, not a finite-width gain peak. The calculation gives positive material [optical gain](../../../../optical-gain.md), not the stronger requirement of exceeding the losses at [laser threshold](../../../../laser-threshold.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
