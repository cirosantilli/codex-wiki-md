<h1 id="12a/solution">Solution</h1>

↑ **Parent:** [12A](../12a.md)

For a sufficiently regular [vector field](../../../../../vector-field.md) $F$ on a bounded region $V$ with piecewise smooth boundary $S$, the [divergence theorem](../../../../../divergence-theorem.md) states

$$
\int_V\nabla\cdot F\,dV=\int_S F\cdot n\,dS,
$$

where $n$ is the outward unit [normal vector](../../../../../normal-vector.md). Apply it to $F=fk$ for an arbitrary constant vector $k$. Since $\nabla\cdot(fk)=k\cdot\nabla f$, it gives

$$
k\cdot\int_V\nabla f\,dV=k\cdot\int_S f n\,dS.
$$

Equality for every constant $k$ proves the [vector gradient form of the divergence theorem](../../../../../vector-gradient-form-of-the-divergence-theorem.md):

$$
\boxed{\int_V\nabla f\,dV=\int_S f\,d\mathbf S}.
$$

Applying the same [divergence theorem](../../../../../divergence-theorem.md) directly to $G$, with $\nabla\cdot G=\rho$, proves the flux law

$$
\boxed{\int_SG\cdot d\mathbf S=\int_V\rho\,dV}.
$$

This is the Gauss flux law for the prescribed source density, obtained directly from the [divergence theorem](../../../../../divergence-theorem.md). For the piecewise source in this problem the divergence relation is understood away from the interface, or almost everywhere; applying the theorem separately to the two sides gives the same law because the normal field is continuous across the interface and the internal boundary fluxes cancel.

For the radial field, its normal component on a sphere of radius $r$ is the constant $G(r)$, so its total flux is $4\pi r^2G(r)$. For $0<r\le a$ the enclosed source is $4\pi\rho_0r^3/3$; for $r>a$ it is $4\pi\rho_0a^3/3$. Thus the [origin-regular spherical Poisson flux law](../../../../../origin-regular-spherical-poisson-flux-law.md) gives

$$
\boxed{G(x)=\begin{cases}\dfrac{\rho_0}{3}x,&r\le a,\\\dfrac{\rho_0a^3}{3r^3}x,&r>a.\end{cases}}
$$

The value at $r=0$ is the continuous value zero. A singular inverse-square radial addition is excluded by the source equation throughout space, including the origin: it would add a point source there.

Since $G=\nabla f$, radial integration gives $f_r=\rho_0r/3$ inside and $f_r=\rho_0a^3/(3r^2)$ outside. The decay condition fixes the exterior constant, giving $f=-\rho_0a^3/(3r)$ for $r\ge a$. Integrating inside gives $f=\rho_0r^2/6+C_0$, and matching at $r=a$ yields $C_0=-\rho_0a^2/2$. Hence the [potential of a uniform spherical source](../../../../../potential-of-a-uniform-spherical-source.md) is

$$
\boxed{f(x)=\begin{cases}\dfrac{\rho_0}{6}(r^2-3a^2),&r\le a,\\-\dfrac{\rho_0a^3}{3r},&r\ge a.\end{cases}}
$$

Both $f$ and its radial derivative are continuous at $a$; there is no surface source hidden in the matching.

For any ball centred at the origin, the [gradient](../../../../../gradient.md) $G(x)$ is odd under $x\mapsto-x$, so its volume integral vanishes by symmetry. On the bounding sphere, $f$ is constant and outward normals at antipodal points are opposite, so $\int_S f n\,dS=0$ as well. **Both sides of the vector [gradient](../../../../../gradient.md) identity are therefore zero**, for radii below, above, or equal to $a$.

## ↑ Ancestors (10)

1. [12A](../12a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
