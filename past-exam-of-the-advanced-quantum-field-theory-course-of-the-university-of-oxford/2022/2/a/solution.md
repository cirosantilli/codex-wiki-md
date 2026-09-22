<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At the stated order the [renormalization-group beta function](../../../../beta-function-physics.md) is separable:

$$
\int_{\alpha_i}^{\alpha_f}\frac{d\alpha}{\alpha^2}
=b_0\int_{\mu_i}^{\mu_f}\frac{d\mu}{\mu}.
$$

Consequently

$$
\boxed{\frac1{\alpha_f}=\frac1{\alpha_i}-b_0\ln\frac{\mu_f}{\mu_i},\qquad
\alpha_f=\frac{\alpha_i}{1-b_0\alpha_i\ln(\mu_f/\mu_i)}.}
$$

For a positive initial [running coupling](../../../../running-coupling.md), this expression is used on the connected interval containing $\mu_i$ where its denominator is positive and [perturbation theory](../../../../perturbation-theory.md) remains valid.

If $b_0<0$, the [running coupling](../../../../running-coupling.md) decreases at high [renormalization scale](../../../../renormalization-scale.md) and tends to zero: this is [asymptotic freedom](../../../../asymptotic-freedom.md). Decreasing the [renormalization scale](../../../../renormalization-scale.md) increases the [running coupling](../../../../running-coupling.md), with a formal infrared pole at $\Lambda=\mu_i\exp[1/(b_0\alpha_i)]$. Near $\Lambda$, [perturbation theory](../../../../perturbation-theory.md) fails; the pole alone is not a proof of [confinement](../../../../confinement.md). Both [QCD](../../../../quantum-chromodynamics.md) and the [SU(2)](../../../../su-2-group.md) weak [gauge coupling](../../../../gauge-coupling.md) have this sign for the [Standard Model](../../../../standard-model-split.md) particle content above the relevant thresholds.

If $b_0>0$, the [running coupling](../../../../running-coupling.md) decreases towards low [renormalization scale](../../../../renormalization-scale.md) and grows towards high [renormalization scale](../../../../renormalization-scale.md). The formal ultraviolet [Landau pole](../../../../landau-pole.md) is $\mu_L=\mu_i\exp[1/(b_0\alpha_i)]$. The pole signals failure of this perturbative evolution, rather than a controlled physical infinity. The [hypercharge](../../../../hypercharge.md) [gauge coupling](../../../../gauge-coupling.md) and ordinary [QED](../../../../quantum-electrodynamics.md) with charged matter have this sign.

If $b_0=0$, the [running coupling](../../../../running-coupling.md) is constant **at this order**; higher-order terms may still make it run. No [Standard Model](../../../../standard-model-split.md) gauge factor has a vanishing one-[loop order](../../../../loop-order.md) coefficient for the usual particle content.

For precise normalization, take $\alpha_i=g_i^2/(4\pi)$ and $Q=T_3+Y$. The [Standard Model one-loop gauge coefficients](../../../../standard-model-one-loop-gauge-coefficients.md) then give

$$
(b_0^Y,b_0^2,b_0^3)=\frac1{2\pi}\left(\frac{41}{6},-\frac{19}{6},-7\right).
$$

These coefficients use $d/d\ln\mu$, not $d/d\ln\mu^2$. Threshold matching changes the active particle content, so the single constant-$b_0$ expression is applied piecewise across thresholds.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the advanced quantum field theory course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory course of the University of Oxford](../../../../advanced-quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
