<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\boldsymbol\zeta=\nabla\times\boldsymbol u$ and $\boldsymbol\omega=\boldsymbol\zeta+2\Omega\boldsymbol e_z$ be the [relative vorticity](../../../../../../relative-vorticity.md) and [absolute vorticity](../../../../../../absolute-vorticity.md). The nonlinear acceleration identity rewrites the momentum equation as

$$
\partial_t\boldsymbol u-\boldsymbol u\times\boldsymbol\omega
=-\nabla\left(\frac P{\rho_0}+\frac12|\boldsymbol u|^2-\frac32\Omega^2x^2\right)-N^2\theta\boldsymbol e_x.
$$

Taking the [curl](../../../../../../curl.md) removes the [pressure](../../../../../../pressure.md), [kinetic energy](../../../../../../kinetic-energy.md) gradient and [shearing-sheet tidal potential](../../../../../../shearing-sheet-tidal-potential.md). Thus

$$
\partial_t\boldsymbol\omega-\nabla\times(\boldsymbol u\times\boldsymbol\omega)
=-N^2\nabla\theta\times\boldsymbol e_x.
$$

Both $\nabla\cdot\boldsymbol u$ and $\nabla\cdot\boldsymbol\omega$ vanish. The [vorticity equation](../../../../../../vorticity-equation.md) is consequently

$$
\partial_t\omega_j+u_i\partial_i\omega_j-\omega_i\partial_i u_j
=-N^2(\nabla\theta\times\boldsymbol e_x)_j.
$$

For the [absolute-vorticity flux tensor](../../../../../../absolute-vorticity-flux-tensor.md) $T_{ij}=u_i\omega_j-\omega_i u_j$, use the flux convention $(\nabla\cdot\boldsymbol T)_j=\partial_iT_{ij}$, with the first index denoting transport direction. This gives

$$
\boxed{\partial_t\boldsymbol\omega+\nabla\cdot\boldsymbol T=-N^2\nabla\theta\times\boldsymbol e_x.}
$$

The scalar $\theta$ is a [buoyancy displacement variable](../../../../../../buoyancy-displacement-variable.md), so dimensional consistency gives it units of length; the printed potential-temperature terminology presupposes this normalization. Its [curl](../../../../../../curl.md) source directly forces only the $y,z$ components of [absolute vorticity](../../../../../../absolute-vorticity.md). Hence [radial vorticity conservation in a shearing sheet](../../../../../../radial-vorticity-conservation-in-a-shearing-sheet.md) takes the local flux form

$$
\boxed{\partial_t\omega_x+\partial_i(u_i\omega_x-\omega_i u_x)=0.}
$$

Its volume integral is constant when the net boundary flux vanishes. However $D_t\omega_x=\boldsymbol\omega\cdot\nabla u_x$ still permits [vortex stretching](../../../../../../vortex-stretching.md); the radial component is not generally a materially conserved scalar in three dimensions. Using divergence on the second index of the stated tensor would reverse the transport sign, so the tensor convention matters.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
