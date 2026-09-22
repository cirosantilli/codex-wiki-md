<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A coarse-grained scalar [order parameter](../../../../../order-parameter.md) $\phi(\mathbf x)$ describes a short-range Ising-like transition with sign [symmetry](../../../../../symmetry-physics.md). Write the dimensionless Landau-Ginzburg functional as

$$
\mathcal H[\phi]=\frac{F[\phi]}{k_BT}
=\int d^dx\left[\frac c2(\nabla\phi)^2+\frac r2\phi^2+\frac u4\phi^4-h\phi\right],\qquad c,u>0.
$$

Here $r=a_t t$, with the relevant critical-mass shift understood when fluctuations are included. Higher local [powers](../../../../../power.md) and [gradients](../../../../../gradient.md) are negligible only within a justified long-distance expansion. The [partition function](../../../../../canonical-partition-function.md) is $Z=\int\mathcal D\phi\,e^{-\mathcal H}$ with a microscopic cutoff. The local functional is not already the fluctuation-integrated thermodynamic [free energy](../../../../../thermodynamic-free-energy.md).

[Mean-field theory](../../../../../mean-field-theory.md) replaces this integral by its stable uniform saddle, $r\phi_0+u\phi_0^3=h$. At $h=0$,

$$
\phi_0=0\quad(r>0),\qquad\phi_0=\pm\sqrt{|r|/u}\quad(r<0),\qquad
f_{\min}-f_0=\begin{cases}0&r>0,\\-r^2/(4u)&r<0.\end{cases}
$$

The branch curvature is $r_L=r+3u\phi_0^2$: it is $r$ above and $2|r|$ below. Hence

$$
\chi_+=r^{-1},\quad\chi_-=(2|r|)^{-1},\quad
\xi=\sqrt{c/r_L},\quad h=u\phi_0^3\text{ at }r=0.
$$

Together with the finite heat-capacity jump from $f_{\min}$, this yields

$$
\boxed{\beta_{\rm MF}=\tfrac12,\quad\gamma_{\rm MF}=1,\quad\delta_{\rm MF}=3,
\quad\nu_{\rm MF}=\tfrac12,\quad\eta_{\rm MF}=0,\quad\alpha_{\rm MF}=0.}
$$

The equal-$|t|$ susceptibility [amplitude](../../../../../wave-amplitude.md) ratio is two. Uniform saddles also miss [domain walls](../../../../../domain-wall.md) and spatial texture. For an $n$-component [order parameter](../../../../../order-parameter.md), [symmetry](../../../../../symmetry-physics.md) allows a vector generalization; ordered transverse directions additionally carry Goldstone fluctuations.

To include small fluctuations set $\phi=\phi_0+\delta\phi$. The [Gaussian](../../../../../normal-distribution.md) action is $\tfrac12\int[c(\nabla\delta\phi)^2+r_L(\delta\phi)^2]$, giving

$$
G(q)=\langle|\delta\phi_q|^2\rangle_{\rm spectral}=\frac1{cq^2+r_L},\qquad
\delta f=\frac12\int^{\Lambda}\frac{d^dq}{(2\pi)^d}\log(cq^2+r_L)+\text{normalization}.
$$

The displayed $G(q)$ is a spectral [covariance](../../../../../covariance.md) per Fourier delta, avoiding an extra [volume](../../../../../volume.md) factor. As $r_L\to0$, a growing [correlation length](../../../../../correlation-length.md) lets increasingly large correlated regions fluctuate. The singular [Gaussian](../../../../../normal-distribution.md) heat correction contains $\int d^dq/(cq^2+r_L)^2$, which is infrared singular for $d<4$ and logarithmic at four. This signals failure of a simple saddle expansion; the [Gaussian](../../../../../normal-distribution.md) heat exponent obtained by extrapolation is not the exact interacting [critical exponent](../../../../../critical-exponent.md).

The [Ginzburg criterion](../../../../../ginzburg-criterion.md) compares the fluctuation of a correlation-volume average with $\phi_0^2$, rather than using all ultraviolet fluctuations at a point. Keeping $q\lesssim\xi^{-1}$ below the transition gives, up to finite convention-dependent constants,

$$
\langle(\delta\phi)_\xi^2\rangle
\sim\int_{|q|\lesssim\xi^{-1}}\frac{d^dq}{(2\pi)^d}\frac1{cq^2+2|r|}
\sim c^{-d/2}|r|^{(d-2)/2}.
$$

Dividing by $\phi_0^2=|r|/u$ yields

$$
\boxed{\mathcal G\sim u c^{-d/2}|r|^{(d-4)/2}\ll1.}
$$

For $d<4$, writing $r=a_t t$ gives a nonuniversal [Ginzburg reduced-temperature window](../../../../../ginzburg-reduced-temperature-window.md)

$$
\boxed{|t|\gg\mathrm{Gi},\qquad
\mathrm{Gi}\sim\left[u c^{-d/2}a_t^{(d-4)/2}\right]^{2/(4-d)}.}
$$

Inside $|t|\lesssim\mathrm{Gi}$, interacting fluctuations must be treated. For example, in three dimensions $\mathrm{Gi}\sim u^2/(c^3a_t)$ in this normalization. Above four dimensions the long-wavelength ratio vanishes at criticality; at four it is marginal and interaction-generated logarithms require further analysis.

<a id="3/a/image-mean-field-wells-and-the-ginzburg-test"></a>
![](../../../../../past-exam-of-the-phase-transitions-and-collective-phenomena-course-of-the-university-of-cambridge/2012/paper-1-ptcp2012-ginzburg.png)

**[Figure 3](#3/a/image-mean-field-wells-and-the-ginzburg-test). Mean-field wells and the Ginzburg test**. Original scalar quartic potentials and dimensionless illustrative Ginzburg ratios. The three-dimensional ratio grows towards criticality, the four-dimensional power estimate is constant and the five-dimensional one falls. A unit-ratio line marks a chosen crossover convention, not measured material data.

The spatial [gradient](../../../../../gradient.md) term supplies [correlations](../../../../../pearson-correlation-coefficient.md) absent from uniform [Landau theory](../../../../../landau-theory.md). The Ginzburg test bounds where its mean-field saddle remains self-consistent; it does not compute nonclassical exponents or a universal material-independent window.[§2.2.3–§2.2.4: correlation length, upper critical dimension and limits of Gaussian fluctuations](../../../../../statistical-field-theory-by-david-tong.md)

## ↑ Ancestors (14)

1. [A](../a.md)
2. [3](../../3.md)
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
