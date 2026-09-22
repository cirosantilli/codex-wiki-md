<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a [force](../../../../../force.md) $\mathbf F\delta(\mathbf x)$ acting on an unbounded incompressible fluid, the [Stokeslet](../../../../../stokeslet.md) and its [pressure](../../../../../pressure.md) are

$$
\boxed{u_i(\mathbf x)=G_{ij}(\mathbf x)F_j,\quad G_{ij}=\frac1{8\pi\mu}\left(\frac{\delta_{ij}}r+\frac{x_ix_j}{r^3}\right),\quad p=\frac{\mathbf F\cdot\mathbf x}{4\pi r^3}.}
$$

They solve $-\nabla p+\mu\nabla^2\mathbf u+\mathbf F\delta=0$ and $\nabla\cdot\mathbf u=0$. Approximate a slender body by a line distribution of these point [forces](../../../../../force.md) on its centreline. At a point labelled by arclength $s$,

$$
\dot{\mathbf X}(s)\simeq\int G(\mathbf X(s)-\mathbf X(s'))\mathbf f(s')\,ds'.
$$

To extract the large logarithm, write $s'=s+\ell$ and approximate $\mathbf X(s+\ell)-\mathbf X(s)\simeq\ell\mathbf t$, $\mathbf f(s+\ell)\simeq\mathbf f(s)$, where $\mathbf t=\mathbf X'$ is the unit [tangent vector](../../../../../tangent-vector.md). The near-line contribution has kernel $(I+\mathbf t\mathbf t)/(8\pi\mu|\ell|)$. Cut it off at the wire radius $R$ and a macroscopic length $L$. The two sides of the line give

$$
\dot{\mathbf X}\sim\frac{\ln(L/R)}{4\pi\mu}(I+\mathbf t\mathbf t)\mathbf f.
$$

The far contribution and changes in the cutoff add terms without the leading logarithm. Since $(I+\mathbf t\mathbf t)^{-1}=I-\mathbf t\mathbf t/2$, inversion proves the leading [slender-body force density](../../../../../slender-body-force-density.md)

$$
\boxed{\mathbf f\sim\frac{2\pi\mu}{\ln(L/R)}(2I-\mathbf t\mathbf t)\dot{\mathbf X}.}
$$

This is [force](../../../../../force.md) on the fluid; the fluid's [force](../../../../../force.md) on the wire has the opposite sign. It gives twice the resistance to transverse motion as to tangential motion at this order.

The stated arclength describes the circular [helix](../../../../../helix.md) $\mathbf X=(a\cos\theta,a\sin\theta,b\theta)$. The PDF omits the second $a$ in the coordinates, so the literal printed curve and its arclength are inconsistent unless $a=1$. First use the circular interpretation consistent with the given arclength. Put $q=\sqrt{a^2+b^2}$ and $c=2\pi\mu/\ln(L/R)$. Then

$$
\mathbf t=\frac{(-a\sin\theta,a\cos\theta,b)}q,\qquad ds=q\,d\theta.
$$

Rotation about $z$ has [velocity](../../../../../velocity.md) $\mathbf v=\Omega(-a\sin\theta,a\cos\theta,0)$, so $\mathbf t\cdot\mathbf v=\Omega a^2/q$. The axial [force](../../../../../force.md) density is $f_z=-c\Omega a^2b/q^2$. Integrating over one turn gives

$$
\boxed{F_z^{\rm rotation}=-\frac{4\pi^2\mu a^2b}{\ln(L/R)\sqrt{a^2+b^2}}\,\Omega.}
$$

For translation, $\mathbf v=W\widehat{\mathbf z}$ and $\mathbf f=cW(2\widehat{\mathbf z}-(b/q)\mathbf t)$. Only the tangential term contributes to axial couple. Since $(\mathbf X\times\mathbf t)_z=a^2/q$, its density is $-cWa^2b/q^2$, giving

$$
\boxed{G_z^{\rm translation}=-\frac{4\pi^2\mu a^2b}{\ln(L/R)\sqrt{a^2+b^2}}\,W.}
$$

These are the off-diagonal coefficients of the [axial resistance matrix of a slender helix](../../../../../axial-resistance-matrix-of-a-slender-helix.md). Their equality does not depend on this particular geometry: with symmetric local resistance $D=c(2I-\mathbf t\mathbf t)$, the rotation-induced axial [force](../../../../../force.md) is $\int\widehat{\mathbf z}\cdot D(\widehat{\mathbf z}\times\mathbf X)ds$, whereas the translation-induced axial [torque](../../../../../torque.md) is $\int(\widehat{\mathbf z}\times\mathbf X)\cdot D\widehat{\mathbf z}\,ds$. They agree pointwise by [symmetry](../../../../../symmetry-physics.md) of $D$. The full Stokes-flow statement is the [Lorentz reciprocal theorem](../../../../../lorentz-reciprocal-theorem-for-stokes-flow.md).

For completeness, retaining the literal elliptic [helix](../../../../../helix.md) instead gives $s'=\sqrt{a^2\sin^2\theta+\cos^2\theta+b^2}$ and the [axial coupling of an elliptic helix](../../../../../axial-coupling-of-an-elliptic-helix.md)

$$
\boxed{\frac{F_z}{\Omega}=\frac{G_z}{W}=-\frac{2\pi\mu ab}{\ln(L/R)}\int_{-\pi}^{\pi}\frac{d\theta}{\sqrt{a^2\sin^2\theta+\cos^2\theta+b^2}}.}
$$

Thus reciprocity holds for the literal curve as well; only the geometric coefficient and arclength change. In all these formulas the equal and opposite [force](../../../../../force.md) or couple on the wire reverses the displayed sign.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 86](../../paper-86-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
