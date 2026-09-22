<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

One normalization of the [Papkovich–Neuber representation](../../../../../../papkovich-neuber-representation.md) uses a harmonic vector $\boldsymbol\Phi$ and harmonic scalar $\psi$:

$$
\boxed{\mathbf u=\boldsymbol\Phi-\frac12\nabla(\mathbf x\cdot\boldsymbol\Phi+\psi),\qquad
p=-\mu\nabla\cdot\boldsymbol\Phi,\qquad
\nabla^2\boldsymbol\Phi=0,\quad\nabla^2\psi=0.}
$$

These formulae give $\nabla\cdot\mathbf u=0$ because $\nabla^2(\mathbf x\cdot\boldsymbol\Phi)=2\nabla\cdot\boldsymbol\Phi$, and give $\mu\nabla^2\mathbf u=\nabla p$. Rescaling the potentials gives the other common normalizations of the representation.

A point [force](../../../../../../force.md) requires a decaying, rotationally covariant field linear in $\mathbf F$, with no length scale. Thus choose the harmonic monopole $\boldsymbol\Phi=c\mathbf F/r$, $\psi=0$, for $r>0$. Differentiating gives

$$
\mathbf u=\frac c2\left(\frac{\mathbf F}{r}+\frac{(\mathbf F\cdot\mathbf x)\mathbf x}{r^3}\right),\qquad
p=\mu c\frac{\mathbf F\cdot\mathbf x}{r^3}.
$$

The [Newtonian fluid stress tensor](../../../../../../newtonian-fluid-stress-tensor.md) is $\sigma_{ij}=-p\delta_{ij}+\mu(\partial_i u_j+\partial_j u_i)$, which simplifies to $\sigma_{ij}=-3\mu c(\mathbf F\cdot\mathbf x)x_ix_j/r^5$. Its traction resultant on a [sphere](../../../../../../sphere.md), using an outward normal from the origin, is $-4\pi\mu c\mathbf F$. Momentum balance with the [force](../../../../../../force.md) $\mathbf F\delta(\mathbf x)$ therefore fixes $c=1/(4\pi\mu)$. The resulting [Stokeslet](../../../../../../stokeslet.md) is

$$
\boxed{u_i=\frac1{8\pi\mu}\left(\frac{F_i}{r}+\frac{(\mathbf F\cdot\mathbf x)x_i}{r^3}\right),\qquad
p=\frac{\mathbf F\cdot\mathbf x}{4\pi r^3},\qquad
\sigma_{ij}=-\frac3{4\pi}\frac{(\mathbf F\cdot\mathbf x)x_ix_j}{r^5}.}
$$

An arbitrary constant [pressure](../../../../../../pressure.md) may be added. The stress has purely radial traction on concentric [spheres](../../../../../../sphere.md), and its integrated traction $-\mathbf F$ supplies the required distributional point-force normalization.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
