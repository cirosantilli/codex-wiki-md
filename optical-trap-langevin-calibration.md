# Optical trap Langevin calibration

↑ **Parent:** [Thermal calibration of an optical trap](thermal-calibration-of-an-optical-trap.md)

Add the random thermal [force](force-split.md) to the deterministic [optical trap relaxation time](optical-trap-relaxation-time.md) model. In one stationary coordinate of a [harmonic optical trap](harmonic-optical-trap.md), the overdamped [Langevin equation](langevin-dynamics.md) is

$$
\zeta\dot x=-kx+\xi(t),\qquad
\langle\xi(t)\rangle=0,\qquad
\langle\xi(t)\xi(t')\rangle=2k_BT\zeta\,\delta(t-t').
$$

Here $\xi$ is [Gaussian white noise](gaussian-white-noise.md) understood through its integrals, $\delta$ is the [Dirac delta function](dirac-delta-function.md), and $\zeta$ is the [linear friction coefficient](linear-friction-coefficient.md). The covariance coefficient has units $\mathrm{N^2\,s}$; multiplying by $\delta(t-t')$, of units $\mathrm{s^{-1}}$, gives squared [force](force-split.md). This [fluctuation-dissipation relation for a Langevin particle](fluctuation-dissipation-relation-for-a-langevin-particle.md) makes the stationary [variance](variance-split.md) $\sigma^2=k_BT/k$, consistent with the [equipartition theorem](equipartition-theorem.md). The solution is an [Ornstein-Uhlenbeck process](ornstein-uhlenbeck-process.md) with [autocovariance function](autocovariance.md)

$$
C_x(t)=\sigma^2e^{-|t|/\tau},\qquad
\tau=\frac{\zeta}{k}.
$$

Indeed, at positive lag the noise has zero correlation with the initial position, so $\zeta C_x'=-kC_x$; its initial value is $\sigma^2$. This supplies both a decay time and an amplitude, making a stronger calibration test than a position histogram alone.

Specify the [Fourier transform](fourier-transform-split.md) convention before using a [power spectral density](power-spectral-density.md). For [frequency](frequency.md) $f$ in [hertz](hertz.md), define $S_x^{(2)}(f)=\int_{-\infty}^{\infty}C_x(t)e^{-2\pi ift}\,dt$ and the one-sided density $S_x^{(1)}(f)=2S_x^{(2)}(f)$ for $f>0$. Integration of the exponential gives

$$
S_x^{(1)}(f)=\frac{4k_BT\zeta}{k^2+(2\pi f\zeta)^2}
=\frac{k_BT}{\pi^2\zeta(f^2+f_c^2)},\qquad
f_c=\frac{k}{2\pi\zeta},\qquad
\int_0^\infty S_x^{(1)}(f)\,df=\frac{k_BT}{k}.
$$

The position [power spectral density](power-spectral-density.md) has units $\mathrm{m^2/Hz}$; its integral is a [variance](variance-split.md), not a [standard deviation](standard-deviation.md). At $f=f_c$ it is half its zero-frequency plateau. Angular [frequency](frequency.md) conventions require a corresponding $2\pi$ conversion in both axis and integration measure. If $x=\beta(V-V_0)$ with position sensitivity $\beta$ in $\mathrm{m/V}$, then $S_V^{(1)}=S_x^{(1)}/\beta^2$ in $\mathrm{V^2/Hz}$ before independent detector noise is added.

For an original invented calibration example, choose $a=0.500\,\mathrm{\mu m}$, [dynamic viscosity](dynamic-viscosity-split.md) $\eta=1.00\times10^{-3}\,\mathrm{Pa\,s}$, $T=300\,\mathrm K$, $k=0.0200\,\mathrm{pN/nm}=2.00\times10^{-5}\,\mathrm{N/m}$, and $\beta=100\,\mathrm{nm/V}$. The unbounded no-slip [Stokes drag law](stokes-s-law.md) gives

$$
\zeta=9.42478\times10^{-9}\,\mathrm{N\,s/m},\quad
\tau=0.471239\,\mathrm{ms},\quad
f_c=337.737\,\mathrm{Hz},\quad
\sigma=14.391\,\mathrm{nm}.
$$

The corresponding voltage [standard deviation](standard-deviation.md) is $0.14391\,\mathrm V$, and the position [power spectral density](power-spectral-density.md) plateau is $0.390369\,\mathrm{nm^2/Hz}$, or $3.90369\times10^{-5}\,\mathrm{V^2/Hz}$ in the detector. Recovering both $k=k_BT/\sigma^2$ and $k=2\pi\zeta f_c$ is an internal model check; actual agreement also tests the assumed [temperature](temperature-split.md), drag and detector response.

<a id="image-synthetic-harmonic-optical-trap-fluctuations-power-spectral-density-and-optical-trap-drag-calibration"></a>
![](optical-tweezers-synthetic-calibration.png)

**[Figure 13](#image-synthetic-harmonic-optical-trap-fluctuations-power-spectral-density-and-optical-trap-drag-calibration). Synthetic harmonic optical trap fluctuations, power spectral density and optical trap drag calibration**. [Source](optical-tweezers-synthetic-calibration.py). Original model calculations and seeded synthetic [Ornstein-Uhlenbeck process](ornstein-uhlenbeck-process.md) samples; explicitly not measured data. The $10\,\mathrm s$ record is sampled at $20\,\mathrm{kHz}$ with no detector noise or exposure averaging. The dashed spectrum includes sampling aliases; the red continuous spectrum integrates to the exact [equipartition theorem](equipartition-theorem.md) variance. The drag line is an exact steady-model prediction.

The generator uses the exact stationary update $x_{j+1}=\rho x_j+\sigma\sqrt{1-\rho^2}\,Z_j$, with $\rho=e^{-\Delta t/\tau}$ and independent standard [normal random variables](gaussian-random-variable.md) $Z_j$. For a demeaned block of $N$ samples and its unnormalized [discrete Fourier transform](discrete-fourier-transform-split.md) $X_j$, the two-sided [periodogram](periodogram.md) is $\Delta t|X_j|^2/N$; doubling positive bins except the zero and Nyquist endpoints gives a one-sided density. Summing those bins times $\Delta f=1/(N\Delta t)$ returns the block mean square by [discrete Parseval identity](discrete-parseval-identity.md). Independent detector noise, finite exposure and [aliasing](aliasing.md) would alter a measured spectrum and must enter a fit before interpreting $f_c$.

**Table of contents**

- [Sinusoidal-stage optical trap calibration](sinusoidal-stage-optical-trap-calibration.md)

## ↑ Ancestors (7)

1. [Thermal calibration of an optical trap](thermal-calibration-of-an-optical-trap.md)
2. [Harmonic optical trap](harmonic-optical-trap.md)
3. [Optical tweezers](optical-tweezers.md)
4. [Optics](optics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Optical trap drag calibration](optical-trap-drag-calibration.md)
- [Solution](past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2004/section-b/b7/c/solution.md)
- [Solution](past-exam-of-the-soft-matter-and-biological-physics-course-of-the-university-of-cambridge/2012/paper-1/3/a/solution.md)
