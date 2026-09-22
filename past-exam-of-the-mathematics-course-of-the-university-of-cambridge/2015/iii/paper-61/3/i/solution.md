<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Integrate [galactic stellar mass](../../../../../../galaxy-stellar-mass.md), rather than galaxy count, against the [galaxy stellar mass function](../../../../../../galaxy-stellar-mass-function.md). With $x=M_*/M_{*,\rm ch}$, the comoving [cosmic stellar mass density](../../../../../../cosmic-stellar-mass-density.md), evaluated by the [stellar mass density from a square-root exponential cutoff](../../../../../../stellar-mass-density-from-a-square-root-exponential-cutoff.md), is

$$
\rho_*^{\rm com}=\phi_{\rm ch}M_{*,\rm ch}\int_0^\infty x^{-3/4}e^{-\sqrt x}\,dx.
$$

Put $u=\sqrt x$, so $dx=2u\,du$ and $x^{-3/4}=u^{-3/2}$. The integral is $2\Gamma(1/2)=2\sqrt\pi$, giving

$$
\boxed{\rho_*^{\rm com}=2\sqrt\pi\,\phi_{\rm ch}M_{*,\rm ch}\simeq3.54\times10^8\,M_\odot\,\mathrm{Mpc^{-3}}.}
$$

The supplied present mean matter density and $\Omega_m=0.25$ imply $\rho_{\rm crit,0}=3.5\times10^{10}/0.25=1.4\times10^{11}\,M_\odot\,\mathrm{Mpc^{-3}}$. Therefore

$$
\boxed{\frac{\rho_*^{\rm com}}{\rho_{\rm crit,0}}\simeq2.53\times10^{-3},\qquad \frac{\rho_*^{\rm com}}{\bar\rho_{m,0}}\simeq1.01\times10^{-2}.}
$$

This is about **$0.25\%$ of today's [critical density](../../../../../../critical-density.md)**, or **$1\%$ of today's mean matter density**, expressed per present [comoving volume](../../../../../../comoving-volume.md). The proper stellar density at $z=3$ is $64\rho_*^{\rm com}$; if comparing that proper density directly with today's [critical density](../../../../../../critical-density.md) its ratio is $0.162$. It must not be confused with the usual comoving-density comparison. The low-mass number integral diverges if extrapolated to zero mass, but the mass integral converges; real populations require a low-mass cutoff.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
