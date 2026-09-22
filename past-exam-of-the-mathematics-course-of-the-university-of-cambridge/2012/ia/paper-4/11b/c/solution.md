<h1 id="11b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Measure a signed angle $\theta$ from the upward radius $A\to O$ in the direction of falling. With $I_A=3ma^2/2$, gravitational [torque](../../../../../../torque.md) gives

$$
\boxed{\ddot\theta=\frac{2g}{3a}\sin\theta.}
$$

There is an idealization in the release condition: **exactly upright and exactly at rest is an unstable equilibrium, so the exact ideal solution stays there.** Uniqueness of this smooth equation with $\theta(0)=\dot\theta(0)=0$ prevents spontaneous departure. The usual falling calculation means an infinitesimal disturbance, with its energy tending to that of the upright rest state. For that limiting [separatrix](../../../../../../separatrix.md) motion, conservation of [mechanical energy](../../../../../../mechanical-energy.md) gives

$$
\frac12I_A\dot\theta^2=mga(1-\cos\theta),\qquad
\boxed{\dot\theta^2=\frac{4g}{3a}(1-\cos\theta).}
$$

On the branch with increasing angle, $\dot\theta=\sqrt{8g/(3a)}\sin(\theta/2)$ for $0<\theta<2\pi$; the opposite branch has the opposite [angular velocity](../../../../../../angular-velocity.md). The nontrivial limiting motion approaches the upright position only as $t\to-\infty$, because $dt/d\theta$ has a logarithmically divergent integral near zero.

Let $e_r$ point from $A$ toward $O$, and $e_\theta$ in the direction of increasing angle, so $e_r=\sin\theta\,e_x+\cos\theta\,e_z$ and $e_\theta=\cos\theta\,e_x-\sin\theta\,e_z$. The [centre of mass](../../../../../../center-of-mass.md) acceleration on the limiting falling branch is

$$
\boxed{a_O=-\frac{4g}{3}(1-\cos\theta)e_r+\frac{2g}{3}\sin\theta\,e_\theta.}
$$

Gravity has components $-mg\cos\theta\,e_r+mg\sin\theta\,e_\theta$. Applying [Newton's second law](../../../../../../newton-s-second-law.md) to the whole disc gives

$$
\boxed{R=\frac{mg}{3}(7\cos\theta-4)e_r-\frac{mg}{3}\sin\theta\,e_\theta.}
$$

The signed component parallel to the radius, positive from $A$ toward $O$, is the required $mg(7\cos\theta-4)/3$. This same radial formula is consistent at the exact stationary upright state, where $\theta=0$, $a_O=0$, and $R=mg e_z$; nonzero falling angles require the limiting-release interpretation just stated.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11B](../../11b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
