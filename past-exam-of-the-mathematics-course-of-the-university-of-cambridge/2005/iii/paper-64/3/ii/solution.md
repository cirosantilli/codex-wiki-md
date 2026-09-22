<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

There is a conformal-time normalization error in the printed density parameter. For physical background density, $H=\mathcal H/a$, so the [cosmological density parameter](../../../../../../cosmological-density-parameter.md) is

$$
\Omega_c=\frac{8\pi G\bar\rho_c}{3H^2}
=\frac{8\pi G a^2\bar\rho_c}{3\mathcal H^2}.
$$

The printed definition lacks the numerator's $a^2$. The [scale factor in a conformal-time density parameter](../../../../../../scale-factor-in-a-conformal-time-density-parameter.md) is essential for $\Omega_c\simeq1$ in the intended flat matter-dominated approximation.

During matter domination, pressureless matter supplies both the expansion and the gravitational source: $a\propto\tau^2$, $\mathcal H=2/\tau$ and $\Omega_c\simeq1$ when CDM is taken to constitute that matter. Thus

$$
\delta_c''+\frac2\tau\delta_c'-\frac6{\tau^2}\delta_c=0.
$$

Try $\delta_c\propto\tau^p$. Its characteristic polynomial is $p(p-1)+2p-6=(p-2)(p+3)$, giving

$$
\boxed{\delta_c=C_g\tau^2+C_d\tau^{-3}=D_g a+D_d a^{-3/2}.}
$$

Radiation-era photon pressure and radiation perturbations affect the metric source, and matter alone does not dominate the expansion, so this matter-only closure and its power laws are inadequate before equality. At late acceleration the growth also ceases to follow $a\propto\tau^2$ and slows. The question's claim that the differential form itself is valid only in matter domination is too strong: for subhorizon pressureless matter with smooth dark energy it still applies with the correct time-dependent $\mathcal H$ and $\Omega_m$. Indeed, the pressureless growth equation in proper time is $\ddot\delta+2H\dot\delta-4\pi G\bar\rho_m\delta=0$ for smooth dark energy; substituting $d/dt_{\rm proper}=a^{-1}d/d\tau$ gives $\delta''+\mathcal H\delta'-4\pi Ga^2\bar\rho_m\delta=0$, the same conformal differential form. It is the matter-dominated coefficients and simple solutions that are restricted to the stated interval.

Outside the radiation-era horizon, the regular growing [adiabatic mode](../../../../../../adiabatic-mode.md) has nearly constant curvature, while its comoving-synchronous density perturbation begins at gradient order $k^2\tau^2$. Equivalently its metric trace grows as $\tau^2$ and the volume relation in (i) gives $\delta_c\propto\tau^2$. This is a relativistic superhorizon solution, not instantaneous Newtonian communication between causally disconnected regions. Inside the horizon, pressure makes the dominant radiation oscillate and its gravitational potential decay, while CDM self-gravity is still subdominant. CDM then grows only weakly, logarithmically in the more accurate [Mészáros effect](../../../../../../meszaros-effect.md); the stated freezing approximation replaces that slow growth by a constant.

Assume all modes being compared start outside the horizon at common $\tau_i$, and define $\tau_h=2\pi/k$, $k_{\rm eq}=2\pi/\tau_{\rm eq}$ and $G_0=(\tau_0/\tau_i)^2$. Modes with $k\leq k_{\rm eq}$ never undergo the radiation-era frozen interval, so their growth is $G_0$. For $k>k_{\rm eq}$, multiply growth before horizon entry, freezing until equality, and subsequent matter growth:

$$
T(k)=\left(\frac{\tau_h}{\tau_i}\right)^2\left(\frac{\tau_0}{\tau_{\rm eq}}\right)^2
=G_0\left(\frac{k_{\rm eq}}k\right)^2.
$$

Thus the [frozen-radiation approximation to the matter transfer function](../../../../../../frozen-radiation-approximation-to-the-matter-transfer-function.md) is

$$
\boxed{T(k)\simeq G_0\begin{cases}1,&k\leq k_{\rm eq},\\(k_{\rm eq}/k)^2,&k>k_{\rm eq}.\end{cases}}
$$

This $T$ includes total growth because the question defines it directly between two density contrasts. The usual transfer normalized to one on large scales is $T/G_0$.

Power is the variance of a Fourier amplitude, so $P_0=|T|^2P_i$. The prescribed primordial density spectrum gives

$$
\boxed{P_0(k)\simeq AG_0^2\begin{cases}k,&k\leq k_{\rm eq},\\k_{\rm eq}^4k^{-3},&k>k_{\rm eq}.\end{cases}}
$$

It turns over at the comoving equality-horizon scale $2\pi/k_{\rm eq}=\tau_{\rm eq}$. The turnover and reduced small-scale growth help organize the broad spectrum of galaxy clustering, clusters and superclusters; they do not select one unique object size. The dimensionless power $k^3P_0/(2\pi^2)$ is approximately flat above equality in this crude approximation, so a decreasing dimensional spectrum does not imply no small-scale structures. Restoring radiation-era logarithmic growth adds logarithmic corrections to the small-scale tail. Baryon acoustic features, a smooth equality transition, late growth suppression and nonlinear halo formation are absent from this simple linear broken-power approximation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
