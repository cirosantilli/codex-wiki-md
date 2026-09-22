<h1 id="17a/solution">Solution</h1>

↑ **Parent:** [17A](../17a.md)

Define source strength $m$ here as the volume [flux](../../../../../flux.md) through a small sphere around the source. For incompressible [potential flow](../../../../../potential-flow.md), $\mathbf u=\nabla\phi$ and the governing conditions are

$$
\Delta\phi=m\delta(\mathbf x-\mathbf x_s),\qquad
\partial_z\phi=0\text{ on }z=0,\qquad \phi\to0\text{ at infinity}.
$$

Equivalently the [Laplace equation](../../../../../laplace-equation.md) holds away from the source, with local behavior $\phi\sim-m/(4\pi|\mathbf x-\mathbf x_s|)$. The boundary condition expresses impermeability. The [method of images](../../../../../method-of-images.md) uses an equal source below the plane:

$$
\boxed{\phi(\mathbf x)=-\frac m{4\pi}\left(\frac1{\sqrt{x^2+y^2+(z-a)^2}}+\frac1{\sqrt{x^2+y^2+(z+a)^2}}\right).}
$$

The image singularity lies outside the fluid, the two vertical [derivatives](../../../../../derivative.md) cancel on the wall, and the source has the specified outward [flux](../../../../../flux.md).

Let $s=\sqrt{x^2+y^2}$. On the wall $u_z=0$ and the tangential radial velocity is $u_s=ms/[2\pi(s^2+a^2)^{3/2}]$. With ambient [pressure](../../../../../pressure.md) $p_\infty$, the steady [Bernoulli equation](../../../../../bernoulli-equation.md) in this [irrotational flow](../../../../../irrotational-flow.md) gives

$$
\boxed{p(s,0)=p_\infty-\frac{\rho m^2s^2}{8\pi^2(s^2+a^2)^3}.}
$$

The fluid [pressure](../../../../../pressure.md) is reduced everywhere on the wall except at its axis and in the infinite-distance limit. The finite hydrodynamic force is the excess over the uniform ambient-pressure force. Integrating its magnitude over the plane yields

$$
F=2\pi\int_0^\infty[p_\infty-p(s,0)]s\,ds
=\frac{\rho m^2}{4\pi}\int_0^\infty\frac{s^3\,ds}{(s^2+a^2)^3}.
$$

Putting $u=s^2$ gives the last [integral](../../../../../integral.md) as $\tfrac12\int_0^\infty u(u+a^2)^{-3}du=1/(4a^2)$. Hence

$$
\boxed{F=\frac{\rho m^2}{16\pi a^2},\qquad \mathbf F=F\mathbf e_z.}
$$

Relative to ambient [pressure](../../../../../pressure.md) on the other side, the boundary is **attracted toward the source**. This is the [hydrodynamic attraction of a plane wall to a point source](../../../../../hydrodynamic-attraction-of-a-plane-wall-to-a-point-source.md).

There is an alternative source-strength convention: if $m$ denotes the coefficient in $u_r=m/r^2$ rather than total volume [flux](../../../../../flux.md), replace the [flux](../../../../../flux.md) above by $4\pi m$. Then $\phi=-m(1/r_++1/r_-)$, $p-p_\infty=-2\rho m^2s^2/(s^2+a^2)^3$, and $F=\pi\rho m^2/a^2$. The physical result is identical once the normalization is fixed.

## ↑ Ancestors (10)

1. [17A](../17a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
