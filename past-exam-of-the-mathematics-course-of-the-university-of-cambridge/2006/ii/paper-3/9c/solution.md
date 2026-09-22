<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

The bob has $\dot x=\ell\cos\theta\,\dot\theta$ and $\dot y=at-\ell\sin\theta\,\dot\theta$. Substituting these into the [Lagrangian](../../../../../lagrangian.md) gives

$$
L=\tfrac12m\ell^2\dot\theta^2-ma\ell t\sin\theta\,\dot\theta+mg\ell\cos\theta+\tfrac12m(a^2+ga)t^2.
$$

The mixed term is $\frac{d}{dt}(ma\ell t\cos\theta)-ma\ell\cos\theta$. Removing this total derivative and the time-only term leaves the equivalent [Lagrangian](../../../../../lagrangian.md) $L_{\rm eff}=\frac12m\ell^2\dot\theta^2+m(g-a)\ell\cos\theta$. The [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) becomes

$$
\boxed{\ddot\theta+\frac{g-a}{\ell}\sin\theta=0.}
$$

In free fall, $a=g$, so $\theta=\theta_0+\omega_0t$: a bob initially at rest relative to the lift remains at its initial angle, and otherwise moves around the pivot with constant angular speed. Every constant angle is then an [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md), with no restoring force. For $a\ne g$, the [equilibria](../../../../../equilibrium-point-of-a-dynamical-system.md) are $\theta=0$ and $\theta=\pi$ modulo $2\pi$.

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
