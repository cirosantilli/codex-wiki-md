<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The flat interface is an equilibrium reservoir with $\mu=0$, while the droplet has the constant surface value $\mu_s=\gamma/(\phi_BR)$. The exterior [chemical potential](../../../../../../chemical-potential.md) satisfies the [Laplace equation](../../../../../../laplace-equation.md), tends to zero far away, and obeys these two surface values. These are exactly the [electrostatic boundary conditions at a conductor](../../../../../../electrostatic-boundary-conditions-at-a-conductor.md) for a sphere held at potential $\mu_s$ above a grounded infinite plane.

Introduce an arbitrary [permittivity](../../../../../../permittivity.md) $\epsilon$. In the electrostatic problem, $Q=-\epsilon\int_{S_R}\partial_n\mu\,dS=C(R,h)\mu_s$. Therefore the [diffusion-capacitance analogy](../../../../../../diffusion-capacitance-analogy.md) gives the outward current

$$
I(R,h)=-M\int_{S_R}\partial_n\mu\,dS=\frac M\epsilon C(R,h)\mu_s.
$$

For an isolated sphere, its [capacitance](../../../../../../capacitance.md) is $C(R,\infty)=4\pi\epsilon R$, so $I(R,\infty)=4\pi MR\mu_s=4\pi M\gamma/\phi_B$. Dividing gives

$$
\boxed{I(R,h)=I(R,\infty)c(R/h),\qquad c(R/h)=\frac{C(R,h)}{C(R,\infty)}.}
$$

Thus [sphere-plane capacitance](../../../../../../sphere-plane-capacitance.md) determines the evaporation enhancement. The assumed spherical shape gives the corresponding law $\dot R=-M\gamma c(R/h)/(2\phi_B^2R^2)$ for [droplet evaporation near a planar reservoir](../../../../../../droplet-evaporation-near-a-planar-reservoir.md). The local surface current is generally nonuniform, even though its total is described by a single capacitance.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
