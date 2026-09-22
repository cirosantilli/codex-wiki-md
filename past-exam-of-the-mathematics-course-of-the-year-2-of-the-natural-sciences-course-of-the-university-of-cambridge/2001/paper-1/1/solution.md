<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**Vector identity.** Work in [Cartesian coordinates](../../../../cartesian-coordinate-system.md) and use the [Einstein summation convention](../../../../einstein-notation.md). Contraction of the two [Levi-Civita symbols](../../../../levi-civita-symbol.md) gives

$$
\begin{aligned}
[\mathbf u\times(\nabla\times\mathbf u)]_i&=\epsilon_{ijk}u_j\epsilon_{klm}\partial_lu_m\\
&=(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})u_j\partial_lu_m\\
&=u_j\partial_iu_j-u_j\partial_ju_i\\
&=\tfrac12\partial_i(u_ju_j)-[(\mathbf u\cdot\nabla)\mathbf u]_i.
\end{aligned}
$$

Thus the [convective acceleration identity](../../../../convective-acceleration-identity.md) is

$$
\boxed{(\mathbf u\cdot\nabla)\mathbf u=\frac12\nabla|\mathbf u|^2-\mathbf u\times(\nabla\times\mathbf u).}
$$

Each term is a geometrically defined [vector field](../../../../vector-field.md): the [directional derivative](../../../../directional-derivative.md) of a vector along itself, the [gradient](../../../../gradient.md) of a [scalar field](../../../../scalar-field.md), and a [cross product](../../../../cross-product.md) with the [curl](../../../../curl.md). Equality in a Cartesian frame is equality of these vectors, so it holds in every coordinate system. When using a varying coordinate [basis](../../../../basis.md), derivatives of the varying basis vectors must be included; differentiating only the component functions would describe a different operation.

**Spherical metric.** Let

$$
R(r,\theta,\phi)=(r\sin\theta\cos\phi,r\sin\theta\sin\phi,r\cos\theta).
$$

Differentiating gives the coordinate [tangent vectors](../../../../tangent-vector-split.md)

$$
\begin{aligned}
R_r&=(\sin\theta\cos\phi,\sin\theta\sin\phi,\cos\theta),\\
R_\theta&=r(\cos\theta\cos\phi,\cos\theta\sin\phi,-\sin\theta),\\
R_\phi&=r\sin\theta(-\sin\phi,\cos\phi,0).
\end{aligned}
$$

Their pairwise [dot products](../../../../dot-product.md) vanish, proving that [spherical coordinates](../../../../spherical-coordinate-system.md) are [orthogonal coordinates](../../../../orthogonal-coordinates.md). Their lengths are the [scale factors of orthogonal coordinates](../../../../scale-factors-of-orthogonal-coordinates.md):

$$
\boxed{h_r=1,\qquad h_\theta=r,\qquad h_\phi=r\sin\theta,\qquad ds^2=dr^2+r^2d\theta^2+r^2\sin^2\theta\,d\phi^2.}
$$

These formulas use the usual chart $r>0,0<\theta<\pi$; the origin and polar axis are coordinate singularities.

**Azimuthal field.** Write the speed as $U(r)$ to distinguish it from the [velocity field](../../../../velocity-field.md) $\mathbf u=U(r)e_\phi$. Using the [curl in spherical coordinates](../../../../curl-in-spherical-coordinates.md),

$$
\nabla\times\mathbf u=\frac{U\cot\theta}{r}e_r-\frac{U+rU'}r e_\theta.
$$

Also $\frac12\nabla|\mathbf u|^2=UU'e_r$. Since $e_\phi\times e_r=e_\theta$ and $e_\phi\times e_\theta=-e_r$,

$$
\mathbf u\times(\nabla\times\mathbf u)=\frac{U(U+rU')}r e_r+\frac{U^2\cot\theta}r e_\theta.
$$

The $UU'$ terms cancel in the [convective acceleration identity](../../../../convective-acceleration-identity.md), giving

$$
\boxed{[(\mathbf u\cdot\nabla)\mathbf u]_r=-\frac{U^2}r,\quad[(\mathbf u\cdot\nabla)\mathbf u]_\theta=-\frac{U^2\cot\theta}r,\quad[(\mathbf u\cdot\nabla)\mathbf u]_\phi=0.}
$$

This [centripetal acceleration of an azimuthal flow](../../../../centripetal-acceleration-of-an-azimuthal-flow.md) points toward the polar axis. A streamline is a [circle](../../../../circle.md) of cylindrical radius $r\sin\theta$, so its acceleration is $-U^2e_\rho/(r\sin\theta)$, with $e_\rho=\sin\theta\,e_r+\cos\theta\,e_\theta$. This independent geometric argument recovers both nonzero components and explains why $U'$ cannot appear: the particle travels at fixed $r$.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2001](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
