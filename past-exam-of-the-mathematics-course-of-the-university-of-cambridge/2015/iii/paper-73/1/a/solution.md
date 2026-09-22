<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

One convention for the [Papkovich–Neuber representation](../../../../../../papkovich-neuber-representation.md) uses a harmonic vector potential $\boldsymbol\Phi$ and a harmonic scalar potential $\chi$:

$$
\boxed{2\mu\mathbf u=\nabla(\mathbf r\cdot\boldsymbol\Phi+\chi)-2\boldsymbol\Phi,\qquad p=\nabla\cdot\boldsymbol\Phi,\qquad\nabla^2\boldsymbol\Phi=0,\quad\nabla^2\chi=0.}
$$

These are [harmonic functions](../../../../../../harmonic-function.md) away from any singular [force](../../../../../../force.md) point. Since $\nabla^2(\mathbf r\cdot\boldsymbol\Phi)=2\nabla\cdot\boldsymbol\Phi$, the representation gives $\nabla\cdot\mathbf u=0$ and $\mu\nabla^2\mathbf u=\nabla p$, the equations of homogeneous [Stokes flow](../../../../../../stokes-flow-split.md).

Place the point [force](../../../../../../force.md) at the origin. A [velocity](../../../../../../velocity.md) linear in $\mathbf F$, decaying as $r^{-1}$ and having the rotational symmetry of a point [force](../../../../../../force.md) is obtained from $\boldsymbol\Phi=c\mathbf F/r$, $\chi=0$. The vector components are [harmonic functions](../../../../../../harmonic-function.md) for $r>0$; scalar dipole potentials would instead generate higher-order decaying singularities. The [force](../../../../../../force.md) normalization fixes $c=-1/(4\pi)$. Indeed, substitution gives the [Stokeslet](../../../../../../stokeslet.md):

$$
\boxed{\mathbf u(\mathbf r)=\frac1{8\pi\mu}\left(\frac{\mathbf F}{r}+\frac{(\mathbf F\cdot\mathbf r)\mathbf r}{r^3}\right),\qquad p(\mathbf r)=\frac{\mathbf F\cdot\mathbf r}{4\pi r^3}.}
$$

To verify its strength, the [Newtonian fluid stress tensor](../../../../../../newtonian-fluid-stress-tensor.md) is $\sigma_{ij}=-3(\mathbf F\cdot\mathbf r)r_i r_j/(4\pi r^5)$. Its outward traction integrated over any [sphere](../../../../../../sphere.md) surrounding the origin is $-\mathbf F$, because $\int\mathbf n\mathbf n\,d\Omega=(4\pi/3)I$. Thus the localized [force](../../../../../../force.md) applied to the fluid is $\mathbf F$, as required. Translation of the origin gives the same [Stokeslet](../../../../../../stokeslet.md) centered at any prescribed [force](../../../../../../force.md) point.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
