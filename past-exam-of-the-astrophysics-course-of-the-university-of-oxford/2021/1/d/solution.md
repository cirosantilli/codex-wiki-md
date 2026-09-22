<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $q_{\rm in}$ be the [photoionization rate](../../../../photoionization-rate.md) per neutral hydrogen atom just outside the empty cavity. With an isotropic central source and no attenuation inside that cavity,

$$
q_{\rm in}=\int_0^\infty\frac{\sigma_\nu L_\nu^*}{4\pi r_{\rm in}^2h\nu}\,d\nu
=\frac{\langle\sigma\rangle Q}{4\pi r_{\rm in}^2}.
$$

The [cross section](../../../../cross-section-physics.md) is zero below threshold; this permits the lower integration limit zero. Pure hydrogen with [hydrogen ionization fraction](../../../../hydrogen-ionization-fraction.md) $\zeta$ has $n_{\rm HI}=n_H(1-\zeta)$ and $n_e=n_p=n_H\zeta$. Local [photoionization equilibrium](../../../../photoionization-equilibrium.md) is therefore

$$
n_H(1-\zeta_{\rm in})q_{\rm in}=\alpha_rn_H^2\zeta_{\rm in}^2.
$$

Define the dimensionless quantity $\Theta_{\rm phys}=\alpha_rn_H/q_{\rm in}$. Solving the resulting [quadratic equation](../../../../quadratic-equation.md), $\Theta_{\rm phys}\zeta_{\rm in}^2+\zeta_{\rm in}-1=0$, gives the physical root

$$
\boxed{\zeta_{\rm in}=\frac{\sqrt{1+4\Theta_{\rm phys}}-1}{2\Theta_{\rm phys}}
=\frac{2}{1+\sqrt{1+4\Theta_{\rm phys}}}.}
$$

The rationalized form avoids numerical cancellation for small $\Theta_{\rm phys}$. Strong illumination gives $\zeta_{\rm in}\simeq1-\Theta_{\rm phys}$; weak illumination gives $\zeta_{\rm in}\simeq\Theta_{\rm phys}^{-1/2}$.

Eliminating $Q$ with the [H-alpha](../../../../h-alpha.md) [luminosity](../../../../luminosity.md), $Q=2.2(4\pi D^2F_{\rm H\alpha})\lambda_{\rm H\alpha}/(hc)$, yields

$$
\boxed{\Theta_{\rm phys}=\frac{n_H\alpha_rhc}{2.2\langle\sigma\rangle F_{\rm H\alpha}\lambda_{\rm H\alpha}}
\left(\frac{r_{\rm in}}D\right)^2.}
$$

**The printed definition of $\Theta$ is inconsistent with the defined radii.** The source calls $r_*$ a physical stellar radius, but its factor $(2\pi r_*D)^2$ gives $\Theta$ units of length to the fourth power, rather than a dimensionless value. It also omits the physically necessary cavity radius $r_{\rm in}$. For a concrete counterexample, double $r_{\rm in}$ while holding the source, $D$, and $n_H$ fixed: the incident [photoionization rate](../../../../photoionization-rate.md) falls by four, so $\Theta_{\rm phys}$ rises by four; the printed expression does not change. The root has the requested form with the corrected $\Theta_{\rm phys}$ above. There is no supplied relation allowing $r_{\rm in}$ to be replaced by $r_*$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
