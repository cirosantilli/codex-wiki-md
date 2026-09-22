<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $K=\rho_0|\mathbf u|^2/2$ be the [kinetic energy](../../../../../../kinetic-energy.md) per unit volume. Dot the momentum equation with $\rho_0\mathbf u$. The [Coriolis acceleration](../../../../../../coriolis-acceleration.md) does no work because $\mathbf u\cdot(\mathbf e_z\times\mathbf u)=0$. [Incompressibility](../../../../../../incompressible-flow.md) turns the [advection](../../../../../../advection.md) and [pressure](../../../../../../pressure.md) terms into divergences, yielding

$$
\boxed{\partial_tK+\nabla\cdot\bigl[(K+P)\mathbf u\bigr]=\rho_0\Omega^2(3x-2qz)u_x.}
$$

Thus $\mathbf F=(K+P)\mathbf u$ is the [energy flux](../../../../../../energy-flux.md) and $S=\rho_0\Omega^2(3x-2qz)u_x$ is the source in the requested kinetic-energy form.

To decide about [conservation of energy](../../../../../../conservation-of-energy.md), absorb the ordinary radial [shearing-sheet tidal potential](../../../../../../shearing-sheet-tidal-potential.md) $\Phi_t=-3\Omega^2x^2/2$ into the density. Its material derivative cancels the $3x$ work term:

$$
\boxed{\partial_t(K+\rho_0\Phi_t)+\nabla\cdot\bigl[(K+P+\rho_0\Phi_t)\mathbf u\bigr]=-2\rho_0\Omega^2qz\,u_x.}
$$

For $q=0$ this is the usual conservative [Jacobi energy in a shearing sheet](../../../../../../jacobi-energy-in-a-shearing-sheet.md), subject to vanishing boundary energy flux. For $q\ne0$, the extra body force has nonzero [curl](../../../../../../curl.md), $\nabla\times[-2\Omega^2qz\mathbf e_x]=-2\Omega^2q\mathbf e_y$, so no scalar potential can absorb it. A potential $2\Omega^2qxz$ would necessarily introduce a vertical force $-2\Omega^2qx\mathbf e_z$, absent from the model. Therefore **this vertical-shear model does not generically conserve the standard total mechanical energy**: its maintained shear/irradiation background can supply or remove energy. This is the [energy balance of the incompressible vertical-shear model](../../../../../../energy-balance-of-the-incompressible-vertical-shear-model.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
