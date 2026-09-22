<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For stationary horizontally homogeneous means, [incompressibility](../../../../../../incompressible-flow.md) gives $\bar w_z=0$ and the impermeable boundary makes $\bar w=0$ throughout. With no imposed horizontal mean pressure gradient, the balances reduce to

$$
\frac{d}{dz}\left(-\kappa\bar b_z+\overline{w'b'}\right)=0,\qquad
\frac{d}{dz}\left(-\nu\bar u_z+\overline{w'u'}\right)=0,\qquad
\bar p_z=\rho_0\bar b-\rho_0\frac{d}{dz}\overline{w'^2}.
$$

The last equation includes the vertical [Reynolds stress](../../../../../../reynolds-stress.md); omitting it requires an additional small-normal-stress approximation. The total vertical buoyancy flux is $B_0$ and the horizontal momentum flux is a signed constant $J_M$ with $|J_M|=U_*^2$. These are fluxes per unit reference density.

The local down-gradient closure defines [eddy viscosity](../../../../../../eddy-viscosity.md) and [eddy diffusivity](../../../../../../eddy-diffusivity.md) by

$$
\overline{w'u'}=-K_M\bar u_z,\qquad
\overline{w'b'}=-K_B\bar b_z.
$$

A parcel moving upwards typically retains the smaller momentum or scalar value from its previous height in an increasing mean profile; its fluctuation then correlates negatively with upward motion. This motivates positive coefficients, but is a closure assumption, not a universal theorem about turbulent or convective fluxes. The mean gradients obey

$$
\boxed{\bar u_z=-\frac{J_M}{\nu+K_M},\qquad
\bar b_z=-\frac{B_0}{\kappa+K_B}.}
$$

For positive applied traction on a fluid above a bottom boundary, $J_M=+U_*^2$ and the mean velocity decreases away from the forcing boundary. The usual atmospheric convention specifies the stress absorbed by the boundary and has the opposite sign of $J_M$; scalar and Richardson-number results are unchanged. At large [Reynolds number](../../../../../../reynolds-number.md) and [Péclet number](../../../../../../peclet-number.md), outside the molecular wall sublayers, $K_M\gg\nu$ and $K_B\gg\kappa$, so molecular transport can be neglected in these flux-gradient relations. Large bulk numbers do not justify doing this exactly at a smooth solid wall.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
