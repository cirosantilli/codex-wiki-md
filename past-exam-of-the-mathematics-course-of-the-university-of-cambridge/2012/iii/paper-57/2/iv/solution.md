<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For $R\gg1$, $3\widetilde c_s^2\simeq1$, and the baryon-inertia corrections to the common Euler equation vanish. Differentiating the photon continuity equation gives

$$
\delta_\gamma''=\tfrac43k^2(-\delta_\gamma/4+\sigma_\gamma)-\tfrac23h'',\qquad
\boxed{\delta_\gamma''-\tfrac43k^2\sigma_\gamma+\tfrac13k^2\delta_\gamma=-\tfrac23h''.}
$$

Set aside the gravitational driving terms and balance the quadrupole streaming source against [Thomson scattering](../../../../../../thomson-scattering.md). With $\tau_c=\Gamma_T^{-1}$ and $\sigma_\gamma'\simeq0$,

$$
\sigma_\gamma\simeq-\tfrac4{15}\tau_ck^2\theta_\gamma=-\tfrac15\tau_c\delta_\gamma',\qquad
\boxed{\delta_\gamma''+\tfrac4{15}\tau_ck^2\delta_\gamma'+\tfrac13k^2\delta_\gamma=0.}
$$

The positive friction is [Silk damping](../../../../../../cosmic-microwave-background-diffusion-damping.md); this particular truncation gives [shear-only photon diffusion damping](../../../../../../shear-only-photon-diffusion-damping.md). Its coefficient follows the supplied simplified quadrupole equation; adding polarization and the full velocity-slip correction changes that coefficient, as in the general [photon-baryon diffusion damping equation](../../../../../../photon-baryon-diffusion-damping-equation.md).

For completeness, put $\omega_0=k/\sqrt3$, $b=4k^2\tau_c/15$ and $D=\tfrac12\int_{\tau_0}^\tau b(s)ds$. Substitution $\delta_\gamma=e^{-D}y$ gives the exact transformed equation

$$
y''+\left(\omega_0^2-\tfrac12b'-\tfrac14b^2\right)y=0.
$$

For constant $\tau_c$ the two independent solutions are $e^{-b(\tau-\tau_0)/2}\cos[\sqrt{\omega_0^2-b^2/4}(\tau-\tau_0)]$ and the corresponding sine. Their frequency correction begins at second order in $\tau_c$. For variable $\tau_c$, retaining first order alone does not automatically remove $b'/2$: a general first-order representation is

$$
y(\tau)=y_0(\tau)+\frac1{2\omega_0}\int_{\tau_0}^{\tau}\sin[\omega_0(\tau-s)]b'(s)y_0(s)ds+O(\tau_c^2),\quad y_0=A\cos[\omega_0(\tau-\tau_0)]+B\sin[\omega_0(\tau-\tau_0)].
$$

The intended cosmological approximation additionally uses slow variation on an acoustic period, $\mathcal H/k\ll1$, with tight coupling $k\tau_c\ll1$. Then the $b'$ correction to the frequency is subleading and the two independent [photon-baryon acoustic oscillator](../../../../../../photon-baryon-acoustic-oscillator.md) solutions take the resummed damping form

$$
\boxed{\delta_\gamma(\mathbf k,\tau)\simeq[A(\mathbf k)\cos(k\tau/\sqrt3)+B(\mathbf k)\sin(k\tau/\sqrt3)]e^{-k^2/k_D^2(\tau)},\qquad k_D^{-2}(\tau)=\frac2{15}\int_{\tau_0}^{\tau}\tau_c(s)ds.}
$$

A shift of the time origin is absorbed in $A,B$. If the ionization fraction is constant, $n_e\propto a^{-3}$ gives $\tau_c\propto a^2\propto\tau^4$ during matter domination, and an initial origin at zero gives $k_D^{-2}=2\tau\tau_c/75$. Across recombination the ionization fraction varies, so the integral is the general answer. The PDF prints $O(\tau_c^{-2})$, while the TeX aid prints $O(\tau_c^2)$; the small-mean-free-time expansion requires the latter interpretation.

The intrinsic photon temperature fluctuation is $\delta T/T=\delta_\gamma/4$. The cosine and sine produce the [Cosmic microwave background acoustic peaks](../../../../../../cosmic-microwave-background-acoustic-peak.md); the envelope suppresses their small-scale amplitudes. The corresponding contribution to the [Cosmic microwave background power spectrum](../../../../../../cosmic-microwave-background-power-spectrum.md) contains $e^{-2k^2/k_D^2}$, before angular projection and the other temperature sources are included. Thus [Silk damping](../../../../../../cosmic-microwave-background-diffusion-damping.md) erases the high-multipole acoustic structure progressively rather than shifting every peak to a new frequency.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
