<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $S_*(\mathbf x)=(\Theta_0+\psi)(\eta_*,\mathbf x)$ and $E=e^{-\tau_{\rm re}}$. Under the stated matter-era growing-mode approximation, $\dot\phi+\dot\psi=0$, and ignoring velocities removes the [Doppler CMB anisotropy](../../../../../../doppler-cmb-anisotropy.md). The two peaks of the [cosmological visibility function](../../../../../../cosmological-visibility-function.md) give the [Cosmic microwave background line-of-sight solution](../../../../../../cosmic-microwave-background-line-of-sight-solution.md)

$$
Y_{\rm obs}(\mathbf e)=E S_*(\mathbf x_0-\chi_*\mathbf e)
+(1-E)(\Theta_0+\psi)(\eta_{\rm re},\mathbf x_0-\chi_{\rm re}\mathbf e),
\quad Y=\Theta+\psi.
$$

Apply the same solution with observation time $\eta_{\rm re}$, just before the thin [reionization](../../../../../../reionization.md) screen. Between recombination and that screen there is no further scattering, so free propagation gives

$$
Y(\eta_{\rm re},\mathbf x,\hat{\mathbf m})=S_*(\mathbf x-\Delta\chi\hat{\mathbf m}),
\qquad\Delta\chi=\eta_{\rm re}-\eta_*.
$$

A direction-independent potential commutes with the angular average. Thus the incoming [photon monopole](../../../../../../photon-monopole.md) plus the potential at the screen is

$$
(\Theta_0+\psi)(\eta_{\rm re},\mathbf x)
=\int\frac{d\hat{\mathbf m}}{4\pi}S_*(\mathbf x-\Delta\chi\hat{\mathbf m}).
$$

Substitution gives

$$
\boxed{Y_{\rm obs}(\mathbf e)=E S_*(\mathbf x_0-\chi_*\mathbf e)
+(1-E)\int\frac{d\hat{\mathbf m}}{4\pi}S_*(\mathbf x_0-\chi_{\rm re}\mathbf e-\Delta\chi\hat{\mathbf m})}.
$$

This derivation inherits the neglected scattering quadrupole and polarization assumptions of part (ii); the screen is an idealized isotropizing approximation.

For a plane [Fourier mode](../../../../../../fourier-mode.md) $S_*(\mathbf x)=S_{\mathbf k}e^{i\mathbf k\cdot\mathbf x}$, the angular average is explicit:

$$
\frac12\int_{-1}^{1}e^{-ik\Delta\chi\mu}d\mu
=j_0(k\Delta\chi)=\frac{\sin(k\Delta\chi)}{k\Delta\chi},
$$

where $j_0$ is the zeroth [Spherical Bessel function](../../../../../../spherical-bessel-function.md). The mode's observed transfer is

$$
Y_{\rm obs}=S_{\mathbf k}e^{i\mathbf k\cdot\mathbf x_0}
\left[E e^{-i\mathbf k\cdot\mathbf e\chi_*}+(1-E)j_0(k\Delta\chi)e^{-i\mathbf k\cdot\mathbf e\chi_{\rm re}}\right].
$$

If $k\Delta\chi\gg1$, the rescattered monopole is suppressed by at least $1/(k\Delta\chi)$, because the incoming directions sample incoherent phases. If $k\Delta\chi\ll1$, $j_0=1+O((k\Delta\chi)^2)$ and the two propagation phases agree to leading order. The two weights then sum to one. Consequently

$$
\boxed{Y_{\rm obs}(\mathbf e)\simeq\begin{cases}
 e^{-\tau_{\rm re}}S_*(\mathbf x_0-\chi_*\mathbf e),&k\Delta\chi\gg1,\\
 S_*(\mathbf x_0-\chi_*\mathbf e),&k\Delta\chi\ll1.
\end{cases}}
$$

These are the small-scale damping and large-scale coherence limits of [reionization damping of cosmic microwave background temperature anisotropy](../../../../../../reionization-damping-of-cosmic-microwave-background-temperature-anisotropy.md).

Each small-scale primary temperature amplitude is multiplied by $e^{-\tau_{\rm re}}$, so its [Cosmic microwave background power spectrum](../../../../../../cosmic-microwave-background-power-spectrum.md) is multiplied by $e^{-2\tau_{\rm re}}$. Holding transfer parameters fixed,

$$
\boxed{C_\ell^{TT,\rm primary}\propto A_s e^{-2\tau_{\rm re}}\quad\text{on the damped angular scales}}.
$$

Many measured high-$\ell$ modes determine this combination accurately. Their derivatives $\partial\log C_\ell/\partial\log A_s=1$ and $\partial\log C_\ell/\partial\tau_{\rm re}=-2$ are degenerate: a change $d\log A_s=2d\tau_{\rm re}$ leaves the leading temperature spectrum unchanged. The undamped large-scale modes can distinguish the parameters, but there are few of them and [cosmic variance](../../../../../../cosmic-variance.md) gives fractional full-sky uncertainty $\sqrt{2/(2\ell+1)}$ per multipole. This explains the [primordial-amplitude–optical-depth degeneracy](../../../../../../primordial-amplitude-optical-depth-degeneracy.md). Polarization from reionization, lensing, and more complete late-time effects partly break it. The TeX's final $\tau_e$ is a transcription mismatch; the PDF uses $\tau_{\rm re}$ consistently.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
