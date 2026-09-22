<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write physical position as $\mathbf r=a(t)\mathbf x$ and physical velocity as

$$
\dot{\mathbf r}=H\mathbf r+\mathbf v,
\qquad
\mathbf v=a\dot{\mathbf x}.
$$

Subtract the homogeneous expanding background from the pressureless [Euler equation](../../../../../euler-equations-for-an-inviscid-fluid.md). To linear order in [peculiar velocity](../../../../../peculiar-velocity.md) and [density contrast](../../../../../density-contrast.md), the convective term is negligible and

$$
\dot{\mathbf v}+H\mathbf v
=-\frac1a\nabla\Phi,
$$

or

$$
\boxed{\frac d{dt}(a\mathbf v)=-\nabla\Phi}.
$$

Here $\nabla$ differentiates with respect to comoving position and $\Phi$ is the peculiar [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md).

The linear continuity and [Poisson equations](../../../../../poisson-equation.md) are

$$
\dot\delta+\frac1a\nabla\cdot\mathbf v=0,
\qquad
\nabla^2\Phi=4\pi Ga^2\bar\rho_m\delta.
$$

For the growing mode $\delta(\mathbf x,t)=D(a)\delta_i(\mathbf x)$, matter conservation gives $\bar\rho_m\propto a^{-3}$, so the potential scales as

$$
\Phi(\mathbf x,t)=\frac{D(a)}a\Phi_i(\mathbf x)
$$

after absorbing the fiducial normalization into $\Phi_i$. Integrating the linear Euler equation with a negligible decaying mode gives

$$
\boxed{
\mathbf v=-\frac{\nabla\Phi_i}{a}
\int^t\frac{D(a)}a\,dt'
}.
$$

Taking the divergence of Euler and using continuity and Poisson yields the [linear growth equation](../../../../../linear-growth-equation.md)

$$
\ddot D+2H\dot D-4\pi G\bar\rho_mD=0.
$$

In the fiducial normalization used in the question this can be rearranged as

$$
\boxed{
\frac{D(a)}a
=\frac1{4\pi G\bar\rho_{m,i}}
\frac d{dt}\left(a^2\frac{dD}{dt}\right)
}.
$$

The [cosmological Lagrangian displacement](../../../../../cosmological-lagrangian-displacement.md) obeys $\dot{\boldsymbol\psi}=\mathbf v/a$. Combining the last two relations and choosing the growing displacement gives the [Zeldovich approximation](../../../../../zeldovich-approximation.md)

$$
\boxed{
\boldsymbol\psi(t)
=-\frac{D(a)}{4\pi G\bar\rho_{m,i}}\nabla\Phi_i
}.
$$

Define

$$
b(t)=\frac{D(a)}{4\pi G\bar\rho_{m,i}}.
$$

Then $\mathbf x=\mathbf x_i-b\nabla\Phi_i$ and $\mathbf v=-a\dot b\nabla\Phi_i$. Keeping the lowest nonvanishing order in displacement in the halo angular momentum gives

$$
\boxed{
\mathbf J
=-\bar\rho_ma^5\dot b
\int_{V_L}d^3x_i\,
(\mathbf x_i-\bar{\mathbf x}_i)\times\nabla\Phi_i
}.
$$

The angular momentum vanishes for a spherical Lagrangian patch, and also whenever the patch's inertia principal axes align with the local tidal-field principal axes. It likewise vanishes in a locally isotropic tidal field.

Taylor-expand

$$
\partial_j\Phi_i(\mathbf x_i)
=\partial_j\Phi_i(\bar{\mathbf x}_i)
+T_{jl}(x_i-\bar x_i)_l+\cdots,
\qquad
T_{jl}=\left.\partial_j\partial_l\Phi_i\right|_{\bar{\mathbf x}_i}.
$$

The constant-gradient term vanishes by the barycentre definition. With

$$
I_{lk}=\int_{V_L}d^3x_i\,
(x_i-\bar x_i)_l(x_i-\bar x_i)_k\,a^3\bar\rho_m,
$$

one obtains the [tidal torque theory](../../../../../tidal-torque-theory.md) result

$$
\boxed{
J_i=-a^2\dot b\,\epsilon_{ijk}T_{jl}I_{lk}
}.
$$

$I$ is the protohalo inertia tensor and $T$ is the local tidal, or gravitational Hessian, tensor. Their eigenframe misalignment produces the torque.

In an [Einstein-de Sitter universe](../../../../../einstein-de-sitter-universe.md), $D\propto a\propto t^{2/3}$. Hence $\dot b\propto\dot a\propto t^{-1/3}$ and

$$
|\mathbf J|\propto a^2\dot b\propto t.
$$

This linear estimate is normally stopped near turnaround. Simulated haloes subsequently gain angular momentum through nonlinear torques, anisotropic accretion, and mergers, including the orbital angular momentum of infalling subhaloes, so the early linear estimate underpredicts the final value.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 346](../../paper-346-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
