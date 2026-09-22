<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $b=|\mathbf r_0|$, $r=|\mathbf r|$, $\mathbf P=\mathbf r-\mathbf r_0$ and $P=|\mathbf P|$. Initially assume $0<b<a$ and a nonzero [current dipole](../../../../../current-dipole.md). The possible singularities of the continued formulas occur when $r=0$, $P=0$ or

$$
D=rP+\mathbf r\cdot\mathbf P=0.
$$

By the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md), $D\geq0$. Away from the two endpoints it vanishes exactly when $\mathbf P$ is antiparallel to $\mathbf r$, namely on the open segment $\mathbf r=s\mathbf r_0$, $0<s<1$. Thus both formulas are regular in the physical exterior $r>a$; the singularities requested here belong to their analytic expressions continued into the sphere.

To determine the order on the segment, let $\mathbf e=\mathbf r_0/b$ and approach an interior point as $\mathbf r=z\mathbf e+\rho\mathbf e_\rho$, with $0<z<b$ and $\mathbf e_\rho\perp\mathbf e$ a unit transverse direction. Expansion gives

$$
D=\frac{b^2\rho^2}{2z(b-z)}+O(\rho^4),
\quad P\mathbf r+r\mathbf P=b\rho\mathbf e_\rho+O(\rho^2),
\quad F=PD=\frac{b^2\rho^2}{2z}+O(\rho^4).
$$

Consequently the leading singular terms in the [electric potential](../../../../../electric-potential.md) and [magnetic scalar potential](../../../../../magnetic-scalar-potential.md) are

$$
u^+\sim\frac{1}{4\pi\sigma}\frac{2\mathbf Q\cdot\mathbf e_\rho}{b\rho},
\qquad
U\sim\frac{\mu_0}{4\pi}\frac{2z(\mathbf Q\times\mathbf e)\cdot\mathbf e_\rho}{b\rho}.
$$

Thus a dipole with a nonzero transverse moment has **first-order line singularities** on the open segment: their generic growth is $1/\rho$, the inverse distance to that segment. Angular coefficients can vanish along particular approach directions without removing the line singularity.

At the source point put $\mathbf r=\mathbf r_0+P\mathbf n$ with a fixed direction $\mathbf n\neq-\mathbf e$. The explicit dipole term gives

$$
u^+=\frac{2\mathbf Q\cdot\mathbf n}{4\pi\sigma P^2}+O(P^{-1}),
\qquad
U=\frac{\mu_0}{4\pi}\frac{(\mathbf Q\times\mathbf e)\cdot\mathbf n}{P(1+\mathbf e\cdot\mathbf n)}+O(1).
$$

The source therefore has a **second-order electric dipole singularity** and, for a nonradial moment, a **first-order magnetic singularity**. Approaches tangent to the singular segment need not have these fixed-angle scalings.

At the origin put $\mathbf r=r\mathbf n$, with $\mathbf n\neq\mathbf e$. The leading terms are

$$
u^+=\frac{1}{4\pi\sigma}\frac{\mathbf Q\cdot(\mathbf n-\mathbf e)}{br(1-\mathbf n\cdot\mathbf e)}+O(1),
\qquad
U=\frac{\mu_0}{4\pi}\frac{(\mathbf Q\times\mathbf e)\cdot\mathbf n}{b(1-\mathbf n\cdot\mathbf e)}+O(r).
$$

The electric expression has a **first-order point singularity** there. The magnetic expression has a generally direction-dependent finite radial limit, so the origin is a nonremovable endpoint singularity of radial order zero, rather than an isolated $1/r$ pole. It can still be unbounded along approaches whose angle to the segment also tends to zero. Stating the approach matters for this nonisolated singularity.

For a [radial current dipole](../../../../../radial-current-dipole.md), $\mathbf Q=q\mathbf e$, the transverse line terms cancel and the electric line singularity is removable. Its only electric singularities are the first-order term $-q/(4\pi\sigma br)$ at the origin and the second-order dipole at $\mathbf r_0$. The magnetic potential is identically zero because $\mathbf Q\times\mathbf r_0=0$. Finally, if $\mathbf r_0=0$, the two terms in the given exterior electric expression combine to

$$
\boxed{u^+=\frac{3}{4\pi\sigma}\frac{\mathbf Q\cdot\mathbf r}{r^3},\qquad U=0.}
$$

There is then just a second-order electric singularity at the origin. A zero dipole moment makes both potentials zero.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
