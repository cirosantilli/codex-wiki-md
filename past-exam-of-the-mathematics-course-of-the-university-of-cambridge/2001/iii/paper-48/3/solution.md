<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [quasi-geostrophic approximation](../../../../../quasi-geostrophic-approximation.md) isolates slowly evolving, nearly balanced motions in a rotating, stably stratified fluid. Ocean eddies and mid-latitude atmospheric disturbances often have this character: a leading [Coriolis force](../../../../../coriolis-force.md)–pressure balance suppresses rapid horizontal acceleration, while [hydrostatic balance](../../../../../hydrostatic-balance.md) suppresses rapid vertical acceleration. Small [ageostrophic flow](../../../../../ageostrophic-flow.md) nevertheless supplies the vertical motion that changes the leading [vorticity](../../../../../vorticity.md). The approximation filters fast [inertia-gravity waves](../../../../../inertia-gravity-wave.md) while retaining nonlinear transport, vertical shear and [Rossby waves](../../../../../rossby-wave.md).

Use a reference density $\rho_0$ and remove the background [hydrostatic pressure](../../../../../hydrostatic-pressure.md). Let $\pi=p'/\rho_0$ and let the upward [buoyancy perturbation](../../../../../buoyancy-perturbation.md) be $b=-g\rho'/\rho_0$. A vertically varying reference [density stratification](../../../../../density-stratification.md) has $N^2(z)>0$. Under the [Boussinesq approximation](../../../../../boussinesq-approximation.md), the inviscid and adiabatic equations are

$$
\frac{D\mathbf u_H}{Dt}+f\widehat{\mathbf z}\times\mathbf u_H=-\nabla_H\pi,\qquad
\frac{Dw}{Dt}=-\pi_z+b,\qquad
\frac{Db}{Dt}+N^2w=0,\qquad
\nabla_H\cdot\mathbf u_H+w_z=0.
$$

Here $D/Dt=\partial_t+\mathbf u_H\cdot\nabla_H+w\partial_z$. Density variations are small compared with $\rho_0$ but retained in the vertical buoyancy force. This is a useful local, incompressible description; a compressible atmosphere needs the corresponding weighted or pressure-coordinate version.

Let horizontal and vertical lengths be $L,H$, speed be $U$, and take the slow time $L/U$. Take $f_0>0$ for definiteness; use $|f_0|$ in the scale estimates in the opposite hemisphere. The principal small parameter is the [Rossby number](../../../../../rossby-number.md) $\mathrm{Ro}=U/(f_0L)\ll1$ at a latitude where $f_0\ne0$. For the hydrostatic, strongly stratified regime, $H/L\ll1$ and $f_0/N\ll1$. Retaining both horizontal [vorticity](../../../../../vorticity.md) and [vortex stretching](../../../../../vortex-stretching.md) gives the [Burger number](../../../../../burger-number.md)

$$
\mathrm{Bu}=\frac{N^2H^2}{f_0^2L^2}=O(1).
$$

The [geostrophic balance](../../../../../geostrophic-balance.md) pressure scale is $f_0UL$ and the [buoyancy perturbation](../../../../../buoyancy-perturbation.md) scale is $B=f_0UL/H$. Hence $B/(N^2H)=\mathrm{Ro}/\mathrm{Bu}\ll1$: [buoyancy perturbations](../../../../../buoyancy-perturbation.md) produce small displacements relative to the background stratification scale. The [ageostrophic flow](../../../../../ageostrophic-flow.md) is $O(\mathrm{Ro}\,U)$ and [incompressibility](../../../../../incompressible-flow.md) then gives $w=O(\mathrm{Ro}\,UH/L)$. Vertical acceleration is smaller than hydrostatic terms by order $\mathrm{Ro}^2(f_0/N)^2$ in this scaling. Weak forcing or diffusion can be added at the slow order, but neither is present here.

Define the [quasi-geostrophic streamfunction](../../../../../quasi-geostrophic-streamfunction.md) by $\psi=\pi/f_0$. Leading [geostrophic balance](../../../../../geostrophic-balance.md) and [hydrostatic balance](../../../../../hydrostatic-balance.md) imply

$$
\boxed{u_g=-\psi_y,\qquad v_g=\psi_x,\qquad b=f_0\psi_z.}
$$

Differentiating horizontally and vertically gives the [thermal-wind balance](../../../../../thermal-wind.md)

$$
f_0u_{g,z}=-b_y,\qquad f_0v_{g,z}=b_x.
$$

Thus vertical shear is determined by horizontal [buoyancy gradients](../../../../../buoyancy-gradient.md). The homogeneous [Taylor–Proudman theorem](../../../../../taylor-proudman-theorem.md) is recovered only when those gradients vanish. Stable stratification allows sloping density surfaces and different [geostrophic flow](../../../../../geostrophic-flow.md) at different levels, without abandoning leading balance.

The [Prandtl ratio of scales](../../../../../prandtl-ratio-of-scales.md) makes that modification quantitative. Horizontal and vertical terms in balanced [potential-vorticity inversion](../../../../../potential-vorticity-inversion.md) have sizes $\psi/L^2$ and $(f_0^2/N^2)\psi/H^2$. Equality gives

$$
\boxed{\frac HL\sim\frac{|f_0|}{N}.}
$$

For constant $N$, $Z=(N/|f_0|)z$ makes the inversion operator an ordinary three-dimensional [Laplacian](../../../../../laplacian.md). Equivalently, an interior balanced disturbance of horizontal size $L$ naturally penetrates a depth of order $|f_0|L/N$. With $N\gg|f_0|$ this is a thin, vertically sheared structure, rather than the arbitrarily tall homogeneous columns suggested by strict [Taylor–Proudman theorem](../../../../../taylor-proudman-theorem.md) behaviour. This is an aspect-ratio statement, not the diffusivity [Prandtl number](../../../../../prandtl-number.md).

To allow a weak meridional variation of the [Coriolis parameter](../../../../../coriolis-parameter.md), use the [beta plane](../../../../../beta-plane.md) $f=f_0+\beta y$, with $\beta L/f_0=O(\mathrm{Ro})$, or equivalently $\beta L^2/U=O(1)$. The small correction to the leading balance is dynamically important on the slow time. Let $\xi=\nabla_H^2\psi$ be vertical relative [vorticity](../../../../../vorticity.md) and let $D_g=\partial_t+\mathbf u_g\cdot\nabla_H$. At the first nontrivial order, the vertical [vorticity equation](../../../../../vorticity-equation.md) and [buoyancy](../../../../../buoyancy.md) equation reduce to

$$
D_g\xi+\beta v_g=f_0w_z,\qquad D_gb+N^2w=0.
$$

Relative-vorticity stretching and tilting are higher order here; planetary-vorticity stretching $f_0w_z$ must remain. Eliminate $w$ to expose a materially conserved balanced scalar. Because $\mathbf u_{g,z}=(-b_y/f_0,b_x/f_0)$, the commutator term $\mathbf u_{g,z}\cdot\nabla_H b$ is exactly zero. For $N=N(z)$ this gives

$$
D_g\!\left[\partial_z\left(\frac{f_0b}{N^2}\right)\right]
=\partial_z\left(\frac{f_0}{N^2}D_gb\right)=-f_0w_z.
$$

Adding the two equations proves the [quasi-geostrophic potential-vorticity equation](../../../../../quasi-geostrophic-potential-vorticity-equation.md)

$$
\boxed{Q=\nabla_H^2\psi+\partial_z\left(\frac{f_0^2}{N^2}\psi_z\right)+\beta y,\qquad D_gQ=0.}
$$

An additive constant such as $f_0$ changes no dynamics. The horizontal [streamfunction advection bracket](../../../../../streamfunction-advection-bracket.md) can express this as $Q_t+\psi_xQ_y-\psi_yQ_x=0$. Although small departures from balance generated this evolution equation, the leading [geostrophic flow](../../../../../geostrophic-flow.md) itself advects $Q$ nonlinearly. The stretching term couples horizontal motion to vertical displacement of density surfaces.

This gives the practical advection-and-inversion description. Start with interior [three-dimensional quasi-geostrophic potential vorticity](../../../../../three-dimensional-quasi-geostrophic-potential-vorticity.md), advect it with $\mathbf u_g$, and recover $\psi$ from

$$
\left[\nabla_H^2+\partial_z\left(\frac{f_0^2}{N^2}\partial_z\right)\right]\psi=Q-\beta y.
$$

The [stratified quasi-geostrophic inversion](../../../../../stratified-quasi-geostrophic-inversion.md) is elliptic for positive $N^2$. It must be supplied with lateral and vertical [boundary conditions](../../../../../boundary-condition.md) and any circulation or mean-flow constraints; interior [potential vorticity](../../../../../potential-vorticity.md) alone is not sufficient. At rigid horizontal lids, $w=0$ makes boundary [buoyancy](../../../../../buoyancy.md) satisfy $D_gb=0$, and $b=f_0\psi_z$ supplies the vertical derivative data for inversion. Boundary [buoyancy perturbations](../../../../../buoyancy-perturbation.md) can therefore support flow even when the interior anomaly is zero. Once $\psi$ is found, its horizontal derivatives give velocity, its vertical derivative gives buoyancy, and the thermodynamic equation diagnoses $w$. This balanced evolution excludes the independent fast-wave initial data present in the full equations.

Finally, a gradient in $f$ supplies a restoring mechanism even in an otherwise uniform fluid. Linearizing about rest with constant $N$, the [quasi-geostrophic potential-vorticity equation](../../../../../quasi-geostrophic-potential-vorticity-equation.md) becomes

$$
\partial_t\left(\nabla_H^2\psi+\frac{f_0^2}{N^2}\psi_{zz}\right)+\beta\psi_x=0.
$$

Substitution of $\psi\propto e^{i(kx+ly+mz-\omega t)}$ gives the [Rossby wave](../../../../../rossby-wave.md) dispersion

$$
\boxed{\omega=-\frac{\beta k}{k^2+l^2+f_0^2m^2/N^2}.}
$$

For $\beta>0$, its zonal phase speed is westward relative to a resting background. A meridionally displaced parcel retains [potential vorticity](../../../../../potential-vorticity.md), so it acquires a relative-vorticity anomaly that induces the velocity tending to return the disturbance. Background shear and stratification modify the full [potential-vorticity gradient](../../../../../potential-vorticity-gradient.md); they can alter propagation or permit instability. On a constant [f-plane](../../../../../f-plane.md) the planetary contribution vanishes, but gradients of relative [vorticity](../../../../../vorticity.md), boundary buoyancy or topography can still support balanced wave motion. Close enough to the equator that $f_0$ vanishes, this mid-latitude [quasi-geostrophic approximation](../../../../../quasi-geostrophic-approximation.md) and its scaling must be replaced.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
