<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The metric source is a gravitational frequency shift. [photons](../../../../photon.md) following [null geodesics](../../../../null-geodesic.md) through a time-dependent spatial metric change [momentum](../../../../momentum-split.md) relative to the background comoving frame. The directional projection of that metric change gives the $\mu^2$ factor. It is not a collision term or continuing [photon](../../../../photon.md) scattering after recombination. The normalization and sign belong to the specified definition of $h$ and $\Delta$; a distribution perturbation should not silently be identified with [temperature](../../../../temperature-split.md) without fixing that normalization.

Define $\mathcal H=\dot R/R$, where dots here mean conformal-time derivatives. In an Einstein-de Sitter background,

$$
\mathcal H=\frac2\tau,\qquad
\mathcal H^2=\frac{8\pi G}{3}\bar\rho_mR^2,
\qquad4\pi G\bar\rho_mR^2=\frac6{\tau^2}.
$$

A [power law](../../../../power-law.md) $h\propto\tau^p$ therefore satisfies $p(p-1)+2p=6$, or $(p-2)(p+3)=0$. Thus

$$
\boxed{h=A\tau^2+B\tau^{-3}},
$$

with the required growing mode $h=A\tau^2$. This is a solution in the perturbation convention used in the question, rather than a statement that every gauge-invariant gravitational potential grows as $\tau^2$.

Use an [integrating factor](../../../../integrating-factor.md) for the [photon](../../../../photon.md) equation:

$$
\Delta(\tau)=\Delta_R e^{-ik\mu(\tau-\tau_R)}
+2\mu^2\int_{\tau_R}^{\tau}\dot h(t)e^{-ik\mu(\tau-t)}dt.
$$

For the growing mode $\dddot h=0$. For the [polynomial-source photon transport solution](../../../../polynomial-source-photon-transport-solution.md), a particular solution is $B_h=-2i\mu\dot h/k+2\ddot h/k^2$: direct substitution gives $\dot B_h+ik\mu B_h=2\mu^2\dot h$. The initial-value solution is consequently

$$
\boxed{\Delta(\tau)=\left[\Delta_R+\frac{2i\mu\dot h_R}{k}-\frac{2\ddot h_R}{k^2}\right]e^{-ik\mu(\tau-\tau_R)}
-\frac{2i\mu\dot h(\tau)}{k}+\frac{2\ddot h(\tau)}{k^2}}.
$$

This also follows by integrating the source twice by parts. The apparent inverse powers of $k$ cancel in the complete long-wavelength limit; the integral form remains regular. At $\mu=0$, the source vanishes and the complete expression reduces to $\Delta=\Delta_R$.

Physically, the exponential transports the recombination pattern along [photon](../../../../photon.md) trajectories; its direction-dependent phase projects a Fourier perturbation onto different angular multipoles. The extra terms are the accumulated gravitational contribution, here expressible as endpoint terms because the source has this special time dependence. For [endpoint monopole and dipole in photon transport](../../../../endpoint-monopole-and-dipole-in-photon-transport.md), at the observer the last two terms are respectively a directional dipole and an angular monopole for each mode; they do not supply a new sky pattern at multipoles $\ell\geq2$. The propagating recombination combination contains the intrinsic perturbation and gravitational/velocity endpoint contributions. Individual terms depend on the perturbation gauge; observable [temperature](../../../../temperature-split.md) anisotropy requires the consistent emitter and observer contributions.

In pure matter domination the gauge-invariant scalar potentials are constant for a growing linear mode: the matter contrast grows as $R$ while the potential scales as its contrast divided by $R$. Thus **growth of this $h$ is compatible with no late [Integrated Sachs-Wolfe effect](../../../../integrated-sachs-wolfe-effect.md) in Einstein-de Sitter**. When [dark energy](../../../../dark-energy.md) suppresses matter growth, the potentials generally evolve; [photons](../../../../photon.md) gain and lose unequal energies entering and leaving a potential well. In a convention where $\Phi,\Psi$ are the dimensionless Newtonian-gauge potentials, the integrated [temperature](../../../../temperature-split.md) source is $\int(\dot\Phi+\dot\Psi)d\tau$ along the light path.

Large-angle cosmic microwave background data can constrain that late contribution, but low-multipole power alone has large [cosmic variance](../../../../cosmic-variance.md) and depends on the primordial [radiation spectrum](../../../../radiation-spectrum.md), geometry and foreground treatment. Cross-correlating the [temperature](../../../../temperature-split.md) map with low-redshift galaxies or other matter tracers isolates a late-time connection; decaying wells typically correlate overdensities with hotter [cosmic microwave background](../../../../cosmic-microwave-background-split.md) directions. Boughn and Crittenden compared WMAP [temperature](../../../../temperature-split.md) data with the HEAO1 hard X-ray background and examined possible foreground origins of the correlation. This tests potential evolution under a cosmological model, not [dark energy](../../../../dark-energy.md) independently of all gravity and [curvature](../../../../curvature.md) assumptions.[abstract and foreground-correlation tests](../../../../investigating-the-origins-of-the-cmb-xrb-cross-correlation-by-stephen-boughn-and-robert-crittenden.md)

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the particle Astrophysics course of the University of Cambridge](../../../split.md)
5. [Particle Astrophysics course of the University of Cambridge](../../../../particle-astrophysics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
