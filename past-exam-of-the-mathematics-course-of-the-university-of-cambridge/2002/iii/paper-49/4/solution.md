<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

[Potential-vorticity inversion](../../../../../potential-vorticity-inversion.md) is the diagnostic recovery of the flow from its advected vortical scalar, using the balance relation and specified [boundary conditions](../../../../../boundary-condition.md). Its usefulness is a separation of tasks: transport the scalar by the current [velocity](../../../../../velocity.md), invert to find the new [velocity](../../../../../velocity.md), and repeat. The inverse is spatially nonlocal even though the transport law is local. The four models differ chiefly in the operator being inverted and the information needed at boundaries.

In [two-dimensional vortex dynamics](../../../../../two-dimensional-vortex-dynamics.md), planar [incompressibility](../../../../../incompressible-flow.md) permits $\boldsymbol u=(-\psi_y,\psi_x)$, and vertical [vorticity](../../../../../vorticity.md) is $\zeta=\nabla^2\psi$. The [curl](../../../../../curl.md) of inviscid momentum gives

$$
\zeta_t+J(\psi,\zeta)=0,\qquad
J(\psi,\zeta)=\psi_x\zeta_y-\psi_y\zeta_x.
$$

There is no [vortex stretching](../../../../../vortex-stretching.md) in strictly planar motion, so [vorticity](../../../../../vorticity.md) is materially conserved. The [two-dimensional potential-vorticity inversion](../../../../../two-dimensional-potential-vorticity-inversion.md) is the [Poisson equation](../../../../../poisson-equation.md) $\nabla^2\psi=\zeta$. On the plane, with suitable integrability and far-field behavior, its [Green's function](../../../../../green-s-function.md) is $(2\pi)^{-1}\log|\boldsymbol x-\boldsymbol x'|$, giving

$$
\psi(\boldsymbol x)=\frac1{2\pi}\int\zeta(\boldsymbol x')\log|\boldsymbol x-\boldsymbol x'|\,d^2x'+\psi_h(\boldsymbol x).
$$

Differentiation gives the [planar Biot-Savart kernel](../../../../../planar-vorticity-velocity-kernel.md). Here $\psi_h$ is a [harmonic function](../../../../../harmonic-function.md) fixed by boundary, circulation and far-field data. A rigid impermeable wall is a streamline, so $\psi$ is constant on it; constants or circulations around distinct holes require specification. The [vorticity](../../../../../vorticity.md) alone cannot distinguish two flows differing by a permitted harmonic contribution, such as a uniform current on an unbounded plane. A constant added to $\psi$ has no physical effect.

In [nonrotating layerwise-two-dimensional vortex dynamics](../../../../../nonrotating-layerwise-two-dimensional-vortex-dynamics.md), strong stable [density stratification](../../../../../density-stratification.md) constrains motion to almost horizontal layers. In the ideal independent-layer limit, vertical [velocity](../../../../../velocity.md) vanishes at leading order, $(u,v)=(-\psi_y,\psi_x)$ and

$$
\zeta_t+J(\psi,\zeta)=0,\qquad\nabla_h^2\psi=\zeta
$$

hold separately at each fixed $z$. Height is a parameter: the horizontal inverse [Laplacian](../../../../../laplacian.md) contains no vertical [derivative](../../../../../derivative.md). With background buoyancy $N^2z$, the leading [Ertel potential vorticity](../../../../../ertel-potential-vorticity.md) is $Q=\boldsymbol\omega\cdot\nabla b\simeq N^2\zeta$, so the materially advected normalized scalar is $Q/N^2\simeq\zeta$. The same horizontal [Poisson equation](../../../../../poisson-equation.md) is inverted layer by layer, using each layer's boundary data. This is an asymptotic constrained model, not arbitrary three-dimensional Euler motion with vertical [velocity](../../../../../velocity.md) set to zero: its validity requires small [Froude number](../../../../../froude-number.md) and controlled vertical scales. At finite [buoyancy frequency](../../../../../buoyancy-frequency.md), the weak vertical motion and tilted [isopycnals](../../../../../isopycnal.md) restore coupling. The inversion may be independent by layer while the reconstructed fields vary with height. The horizontal [Euler equations for an inviscid fluid](../../../../../euler-equations-for-an-inviscid-fluid.md) determine the [pressure gradient](../../../../../pressure-gradient.md), while [hydrostatic balance](../../../../../hydrostatic-balance.md) relates its vertical [derivative](../../../../../derivative.md) to [buoyancy](../../../../../buoyancy.md).

In [shallow-water quasi-geostrophic inversion](../../../../../shallow-water-quasi-geostrophic-inversion.md), begin with the exact [shallow-water potential vorticity](../../../../../shallow-water-potential-vorticity.md) $(f+\zeta)/h$. Linearizing its anomaly about depth $H$ gives, after multiplying by $H$, $\zeta-f_0\eta/H$. For small [Rossby number](../../../../../rossby-number.md), [geostrophic balance](../../../../../geostrophic-balance.md) gives $\psi=g\eta/f_0$, while $\zeta=\nabla_h^2\psi$. Keeping the [beta plane](../../../../../beta-plane.md) background gradient gives

$$
q=\nabla_h^2\psi-\frac{\psi}{L_D^2}+\beta y,\qquad
L_D=\frac{\sqrt{gH}}{|f_0|},\qquad
q_t+J(\psi,q)=0.
$$

Thus $q-\beta y$ is inverted with the [modified Helmholtz equation](../../../../../modified-helmholtz-equation.md) $(\nabla_h^2-L_D^{-2})\psi=q-\beta y$, under the specified boundary and far-field conditions. The [velocity](../../../../../velocity.md) follows from $\psi$ and surface elevation from $\eta=f_0\psi/g$. A horizontal [Fourier mode](../../../../../fourier-mode.md) of the anomaly satisfies

$$
\widehat\psi=-\frac{\widehat{q-\beta y}}{|\boldsymbol k_h|^2+L_D^{-2}}.
$$

The [Rossby deformation radius](../../../../../rossby-deformation-radius.md) therefore limits the reach of the balanced response. Layer stretching, represented by $-\psi/L_D^2$, is absent from ordinary planar [vorticity](../../../../../vorticity.md) inversion. Unlike the pure [Poisson equation](../../../../../poisson-equation.md), the finite-deformation operator also responds to the constant part of $\psi$, which specifies mean elevation rather than an arbitrary streamfunction offset. Specified bottom topography adds a known source to $q$; it is subtracted along with the background before inversion.

In [stratified quasi-geostrophic inversion](../../../../../stratified-quasi-geostrophic-inversion.md), continuously varying vertical displacement replaces the shallow layer's single stretching term. For positive $N^2(z)$ and constant nonzero $f_0$, the [three-dimensional quasi-geostrophic potential vorticity](../../../../../three-dimensional-quasi-geostrophic-potential-vorticity.md) is

$$
q=\nabla_h^2\psi+\partial_z\left(\frac{f_0^2}{N^2}\psi_z\right)+\beta y,
\qquad q_t+J(\psi,q)=0.
$$

[Geostrophic balance](../../../../../geostrophic-balance.md) and [hydrostatic balance](../../../../../hydrostatic-balance.md) give [velocity](../../../../../velocity.md) $(-\psi_y,\psi_x)$ and [buoyancy perturbation](../../../../../buoyancy-perturbation.md) $b=f_0\psi_z$. Invert the anisotropic [elliptic boundary value problem](../../../../../elliptic-boundary-value-problem-split.md) using interior $q$, prescribed top and bottom [buoyancy](../../../../../buoyancy.md) as [Neumann boundary conditions](../../../../../neumann-boundary-condition.md), and the lateral, far-field and global-flow data. Boundary [buoyancy](../../../../../buoyancy.md) evolves by its own material conservation when the boundary is impermeable. It cannot be discarded: the [Eady edge wave](../../../../../eady-edge-wave.md) in the preceding solution has zero interior [potential vorticity](../../../../../potential-vorticity.md) anomaly but nonzero boundary buoyancy and a nonzero induced flow.

For constant $N,f_0$, the [stretched coordinates for quasi-geostrophic inversion](../../../../../stretched-coordinates-for-quasi-geostrophic-inversion.md) $Z=Nz/|f_0|$ turn the inversion operator into the three-dimensional [Laplacian](../../../../../laplacian.md). Its infinite-space [Green's function](../../../../../green-s-function.md) is $-1/(4\pi|\boldsymbol X-\boldsymbol X'|)$ in $(x,y,Z)$ coordinates. Hence a horizontal disturbance of scale $L$ communicates vertically over scale $|f_0|L/N$, explicitly coupling layers. In a bounded domain with homogeneous difference data, multiplying the difference of two inversions by its [streamfunction](../../../../../stream-function.md) and applying [integration by parts](../../../../../integration-by-parts.md) gives

$$
\int\left(|\nabla_h\delta\psi|^2+\frac{f_0^2}{N^2}|\delta\psi_z|^2\right)dV=0.
$$

This proves uniqueness up to a constant when the relevant boundary terms vanish; a mean or pressure reference fixes the remaining constant. Compatible boundary fluxes are needed for a purely [Neumann boundary-value problem](../../../../../neumann-boundary-value-problem.md).

Across all four models, inversion provides the induced flow, while scalar transport supplies time evolution. The independent horizontal inverse in the first two models becomes a finite-deformation inverse in shallow water and a vertically coupled elliptic inverse in continuous stratification. The principle applies within the stated balance or constrained model. In the unrestricted [Boussinesq equations](../../../../../boussinesq-equations.md) or [shallow water equations](../../../../../shallow-water-equations.md), [gravity waves](../../../../../gravity-wave-split.md) and divergent motion can share the same [potential vorticity](../../../../../potential-vorticity.md), so the vortical scalar alone does not reconstruct every possible flow.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
