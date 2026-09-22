<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $r=|\mathbf x|$. In the [Unscaled Papkovich–Neuber representation](../../../../../../unscaled-papkovich-neuber-representation.md), choose the [componentwise harmonic vector field](../../../../../../componentwise-harmonic-vector-field.md)

$$
\boldsymbol\Phi=-\tfrac12f(r)\boldsymbol\Omega\times\mathbf x,
\qquad f(r)=A+\frac B{r^3}.
$$

Both $\boldsymbol\Omega\times\mathbf x$ and $(\boldsymbol\Omega\times\mathbf x)/r^3$ are harmonic away from the origin: the latter is a linear combination of derivatives of the [harmonic function](../../../../../../harmonic-function.md) $1/r$. Also $\mathbf x\cdot\boldsymbol\Phi=0$, so the representation gives $\mathbf u=f(r)\boldsymbol\Omega\times\mathbf x$. The [no-slip boundary condition](../../../../../../no-slip-boundary-condition.md) requires $f(a)=1$ and $f(b)=0$, giving

$$
A=-\frac{a^3}{b^3-a^3},\qquad B=\frac{a^3b^3}{b^3-a^3}.
$$

Thus the [Rotational Stokes flow between concentric spheres](../../../../../../rotational-stokes-flow-between-concentric-spheres.md) is

$$
\boxed{\mathbf u=\frac{a^3}{b^3-a^3}\left(\frac{b^3}{r^3}-1\right)
\boldsymbol\Omega\times\mathbf x.}
$$

The [divergence](../../../../../../divergence.md) of $\boldsymbol\Phi$ is zero: the cross-product field itself has zero [divergence](../../../../../../divergence.md), and $\nabla f$ is radial and perpendicular to $\boldsymbol\Omega\times\mathbf x$. Hence $p=2\mu\nabla\cdot\boldsymbol\Phi=0$ in this [pressure](../../../../../../pressure.md) gauge.

There is also a symmetry argument. Take the rotation axis as the polar axis. [Linearity of Stokes flow](../../../../../../linearity-of-stokes-flow.md) makes [velocity](../../../../../../velocity.md) and [pressure](../../../../../../pressure.md) perturbations change sign when the rotation reverses. Reflection in any plane containing that axis reverses the axial rotation vector. Combined with axial symmetry, this excludes meridional [velocity](../../../../../../velocity.md) components and forces the [pressure](../../../../../../pressure.md) perturbation to be both unchanged and sign-reversed by that reflection. Equivalently a purely azimuthal axisymmetric [Stokes flow](../../../../../../stokes-flow-split.md) has no meridional component of its vector [Laplacian](../../../../../../laplacian.md), so its meridional [pressure](../../../../../../pressure.md) gradient vanishes. Thus the [pressure](../../../../../../pressure.md) is constant; setting that arbitrary constant to zero gives the same result without solving the radial coefficients.

For the [Newtonian fluid stress tensor](../../../../../../newtonian-fluid-stress-tensor.md), let $\mathbf q=\boldsymbol\Omega\times\mathbf x$. The symmetric part of the [velocity](../../../../../../velocity.md) gradient is

$$
e_{ij}=\frac{f'(r)}{2r}(q_ix_j+x_iq_j),
$$

because the gradient of rigid rotation is antisymmetric. Consequently the full [stress tensor](../../../../../../cauchy-stress-tensor.md), with $p=0$, is

$$
\boxed{\sigma_{ij}=-\frac{3\mu B}{r^5}(q_ix_j+x_iq_j).}
$$

For $\boldsymbol\Omega=\Omega\mathbf e_z$, its only nonzero spherical-coordinate components are $\sigma_{r\phi}=\sigma_{\phi r}=-3\mu B\Omega\sin\vartheta/r^3$. On the inner sphere the traction exerted by the fluid, using the sphere's outward normal $\mathbf n$, is

$$
\mathbf t=\boldsymbol\sigma\mathbf n
=-\frac{3\mu B}{a^3}\boldsymbol\Omega\times\mathbf n.
$$

Its [torque](../../../../../../torque.md) is

$$
\int_{r=a}\mathbf x\times\mathbf t\,dS
=-3\mu B\int\{\boldsymbol\Omega-\mathbf n(\mathbf n\cdot\boldsymbol\Omega)\}\,d\omega
=-8\pi\mu B\boldsymbol\Omega,
$$

using $\int n_in_j\,d\omega=4\pi\delta_{ij}/3$. Therefore the applied [Torque in rotational Stokes flow between concentric spheres](../../../../../../torque-in-rotational-stokes-flow-between-concentric-spheres.md) is

$$
\boxed{\mathbf G_0=\frac{8\pi\mu a^3b^3}{b^3-a^3}\boldsymbol\Omega.}
$$

For $b\gg a$, the relevant speed and length are $\Omega a$ and $a$, so negligible inertia requires the rotational [Reynolds number](../../../../../../reynolds-number.md)

$$
\boxed{\frac{\rho|\Omega|a^2}{\mu}\ll1.}
$$

For a narrow gap $d=b-a\ll a$, the viscous gradients are controlled by $d$, not $a$. A centrifugal acceleration of scale $\Omega^2a$ is then compared with viscous scale $\mu\Omega a/d^2$, rather than $\mu\Omega/a$. Their ratio is $\rho|\Omega|d^2/\mu$. This explains why the large-gap condition is not a necessary narrow-gap criterion; a thin gap greatly strengthens viscous resistance. This base-flow scaling is distinct from a criterion for stability to arbitrary short-scale disturbances.

The [Minimum-dissipation theorem for Stokes flow](../../../../../../minimum-dissipation-theorem-for-stokes-flow.md) compares a Stokes solution with all sufficiently regular incompressible trial velocities in the same fluid domain that have the same prescribed boundary velocities. With no body-force work, the dissipation functional is

$$
D[\mathbf v]=\int 2\mu\,\mathbf e(\mathbf v):\mathbf e(\mathbf v)\,dV.
$$

If $\mathbf v=\mathbf u+\mathbf w$ and $\mathbf w=0$ on the prescribed boundary, integration by parts with $\nabla\cdot\boldsymbol\sigma(\mathbf u)=0$ and $\nabla\cdot\mathbf w=0$ makes the cross term vanish. Thus

$$
D[\mathbf v]-D[\mathbf u]=2\mu\int\mathbf e(\mathbf w):\mathbf e(\mathbf w)\,dV\ge0.
$$

The comparison fixes velocities, rather than applied torques or forces.

Now let the particles take their actual rigid translations and rotations in the particle-containing flow. Extend the fluid [velocity](../../../../../../velocity.md) through each particle by its rigid [velocity](../../../../../../velocity.md). [No-slip boundary conditions](../../../../../../no-slip-boundary-condition.md) make this extension continuous; rigid motion has zero [rate-of-strain tensor](../../../../../../strain-rate-tensor.md) and zero [divergence](../../../../../../divergence.md). The extension is therefore an admissible trial field in the original particle-free annulus, and its dissipation equals that of the fluid outside the particles. Hence $D\ge D_0$.

The Stokes boundary-work identity gives $D=\mathbf G\cdot\boldsymbol\Omega$. The outer sphere is stationary, the maintained inner sphere has zero translational [velocity](../../../../../../velocity.md), and every added particle has zero total [force](../../../../../../force.md) and [torque](../../../../../../torque.md), so none of those other boundaries contributes power. Likewise $D_0=\mathbf G_0\cdot\boldsymbol\Omega$. Therefore

$$
\boldsymbol\Omega\cdot\mathbf G\ge\boldsymbol\Omega\cdot\mathbf G_0.
$$

For nonzero rotation and a particle of positive volume the inequality is strict: equality in the dissipation identity would [force](../../../../../../force.md) the extension to be the unique original flow, but that original flow has nonzero strain on every open particle region, whereas a rigid interior has zero strain. This proves that [force-free inclusions increase rotational resistance](../../../../../../force-free-inclusions-increase-rotational-resistance.md):

$$
\boxed{\mathbf G\cdot\frac{\boldsymbol\Omega}{|\boldsymbol\Omega|}
>\frac{8\pi\mu a^3b^3}{b^3-a^3}|\boldsymbol\Omega|.}
$$

No dilute-suspension approximation or assumption about the particle shapes was used.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
