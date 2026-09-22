# Rutherford impact-parameter relation

↑ **Parent:** [Rutherford scattering](rutherford-scattering.md)

Let $\theta$ be the scattering [angle](angle.md) between incoming and outgoing [velocities](velocity.md), so forward scattering is $\theta=0$ and exact reversal is $\theta=\pi$. Define the [length](length.md) $a=\kappa/(2E)$. Then

$$
\boxed{b=a\cot\frac\theta2},\qquad
\theta=2\arctan\frac{a}{b}.
$$

For $b>0$, this gives $0<\theta<\pi$; $b=0$ is the head-on limiting case $\theta=\pi$. Large deflections select small [impact parameters](impact-parameter.md), rather than requiring every incident [alpha particle](alpha-particle.md) to reverse.

A short derivation uses [conservation of angular momentum](conservation-of-angular-momentum.md) and [conservation of energy](conservation-of-energy.md). Choose the polar [angle](angle.md) $\phi=0$ at closest approach, and write $u=1/r$. The [Binet equation](binet-equation.md) for the repulsive [Coulomb potential](coulomb-potential-energy.md) gives

$$
\frac{d^2u}{d\phi^2}+u=-\frac{m\kappa}{L^2},\qquad
u=\frac{m\kappa}{L^2}(\epsilon\cos\phi-1),\qquad
\epsilon^2=1+\frac{2EL^2}{m\kappa^2}.
$$

The last equality follows by substituting this [orbit](orbit-dynamical-system.md) into $E=m\dot r^2/2+L^2/(2mr^2)+\kappa/r$. The [hyperbola](hyperbola.md) reaches infinity at $\phi=\pm\phi_\infty$, with $\cos\phi_\infty=1/\epsilon$. Its scattering [angle](angle.md) is $\theta=\pi-2\phi_\infty$, hence

$$
\cot\frac\theta2=\sqrt{\epsilon^2-1}
=\frac{\sqrt{2E/m}\,L}{\kappa}
=\frac{2Eb}{\kappa}.
$$

This proves the relation without assuming that the deflection is small. The symbol $\epsilon$ here is a dimensionless orbital parameter, distinct from $\varepsilon_0$.

## ↑ Ancestors (4)

1. [Rutherford scattering](rutherford-scattering.md)
2. [Atomic physics](atomic-physics-split.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2019/paper-1/section-c/c10/solution.md)
- [Rutherford differential cross-section](rutherford-differential-cross-section.md)
