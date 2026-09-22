<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $A$ be the constant cross-sectional [area](../../../../../../surface-area.md), and suppose that the [temperature](../../../../../../temperature-split.md) is uniform on each cross-section. Consider a slice $[a,b]$. Its stored thermal [energy](../../../../../../energy-split.md) is $\rho cA\int_a^bT(x,t)\,dx$. Since the lateral surface is insulated and there is no internal [heat](../../../../../../heat-split.md) generation, [conservation of energy](../../../../../../conservation-of-energy.md) gives

$$
\rho cA\frac{d}{dt}\int_a^bT(x,t)\,dx=Aq(a,t)-Aq(b,t),
$$

where $q$ is the [heat flux](../../../../../../heat-flux-density.md) in the positive $x$ direction. By [Fourier's law](../../../../../../fourier-s-law.md), $q=-kT_x$, so

$$
\rho c\int_a^bT_t\,dx=kT_x(b,t)-kT_x(a,t)=k\int_a^bT_{xx}\,dx.
$$

The slice is arbitrary; therefore the local [heat equation](../../../../../../heat-equation.md) is

$$
\boxed{T_t=\kappa T_{xx},\qquad\kappa=\frac{k}{\rho c}>0.}
$$

The constant $\kappa$ is the [thermal diffusivity](../../../../../../thermal-diffusivity.md). The cancellation of $A$ uses a rod of uniform cross-section; the one-dimensional model assumes no transverse [temperature](../../../../../../temperature-split.md) variation.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
