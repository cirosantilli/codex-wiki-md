<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The continuity and [Cosmological Euler equation in synchronous gauge](../../../../../../cosmological-euler-equation-in-synchronous-gauge.md) combine particularly simply. Differentiate $\delta_C'=-\nabla\cdot v_C-h'/2$ and add $\mathcal H\delta_C'$:

$$
\delta_C''+\mathcal H\delta_C'=-\nabla\cdot(v_C'+\mathcal Hv_C)-\frac12(h''+\mathcal Hh')=4\pi Ga^2\sum_N(1+3c_N^2)\rho_N\delta_N.
$$

The [velocity](../../../../../../velocity.md) terms cancel by the [Cosmological Euler equation in synchronous gauge](../../../../../../cosmological-euler-equation-in-synchronous-gauge.md), so this step does not require setting the initial [velocity](../../../../../../velocity.md) exactly to zero.

For subhorizon modes deep in [radiation domination](../../../../../../radiation-domination.md), take the rapidly oscillating radiation perturbation to be negligible in the averaged gravitational forcing. Also neglect the subdominant matter self-gravity to leading order in $\rho_C/\rho_r$. With $a\propto\tau$ and $\mathcal H=1/\tau$, the resulting equation is

$$
\delta_C''+\frac1\tau\delta_C'=0,\qquad (\tau\delta_C')'=0.
$$

Integrating twice gives

$$
\boxed{\delta_C(\tau,x)=A(x)\log(\tau/\tau_*)+B(x),}
$$

where the arbitrary reference time $\tau_*$ makes the logarithm dimensionless and can be absorbed into $B$. This is [logarithmic growth of matter perturbations during radiation domination](../../../../../../logarithmic-growth-of-matter-perturbations-during-radiation-domination.md).

The neglect of matter self-gravity is needed for the displayed form to be exact within the leading radiation-background approximation. Uniform radiation alone leaves a nonzero term $4\pi Ga^2\rho_C\delta_C$ if the cold-matter density is retained. Relative to $\mathcal H^2$, its coefficient is $3\Omega_C(a)/2$, small deep in the radiation era but not near equality. The [Mészáros equation](../../../../../../meszaros-equation.md) retains that effect in a matter-plus-radiation background; its solution basis tends to a constant and a logarithm at $a/a_{\rm eq}\ll1$, recovering the present leading result. It connects smoothly to matter-era growth rather than allowing the logarithmic approximation to be extrapolated indefinitely.

Galaxy-scale modes enter the [Hubble radius](../../../../../../hubble-radius.md) before [matter-radiation equality](../../../../../../matter-radiation-equality.md). The earlier radiation forcing and horizon-entry matching ordinarily generate a nonzero logarithmic coefficient, even though subsequent oscillatory radiation forcing is small. A [Fourier mode](../../../../../../fourier-mode.md) with entry time $\tau_h\sim k^{-1}$ accumulates $\log(\tau_{\rm eq}/\tau_h)\sim\log(k\tau_{\rm eq})$ before equality. Across a large scale-factor range this factor need not be small, so treating the [density contrast](../../../../../../density-contrast.md) as exactly frozen would lose an important part of the galaxy-scale seed amplitude and its scale dependence. Growth is nevertheless much slower than $\delta_C\propto a$ in [matter domination](../../../../../../matter-domination.md). This is the [Mészáros effect](../../../../../../meszaros-effect.md), and the logarithmic matching contributes to the small-scale matter [cold-dark-matter transfer function](../../../../../../cold-dark-matter-transfer-function.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
