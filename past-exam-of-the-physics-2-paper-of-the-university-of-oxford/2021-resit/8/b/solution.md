<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the grounded [electrical conductor](../../../../electrical-conductor.md) to occupy $z\leq0$ and approximate the negligible-radius charged sphere by a [point charge](../../../../point-charge.md) $Q$ at $\mathbf r_+=D\widehat{\mathbf z}$. Put a fictitious [image charge](../../../../image-charge.md) $-Q$ at $\mathbf r_-=-D\widehat{\mathbf z}$. The constructed [electric potential](../../../../electric-potential.md) is zero on $z=0$, has the correct [point charge](../../../../point-charge.md) singularity, and vanishes at infinity. The [uniqueness theorem for the electrostatic potential](../../../../uniqueness-theorem-for-the-electrostatic-potential.md) makes it the physical [electric potential](../../../../electric-potential.md) for $z>0$:

$$
\phi(\mathbf r)=\frac Q{4\pi\epsilon_0}
\left(\frac1{|\mathbf r-D\widehat{\mathbf z}|}
-\frac1{|\mathbf r+D\widehat{\mathbf z}|}\right).
$$

Taking its negative [gradient](../../../../gradient.md) gives the requested [electric field](../../../../electric-field-split.md) outside the small sphere:

$$
\boxed{\mathbf E(\mathbf r)=\frac Q{4\pi\epsilon_0}
\left[\frac{\mathbf r-D\widehat{\mathbf z}}{|\mathbf r-D\widehat{\mathbf z}|^3}
-\frac{\mathbf r+D\widehat{\mathbf z}}{|\mathbf r+D\widehat{\mathbf z}|^3}\right],\quad z>0.}
$$

On the plane at cylindrical [radius](../../../../radius.md) $r$, the tangential components cancel and the normal component is

$$
E_z(r,0^+)=-\frac{QD}{2\pi\epsilon_0(r^2+D^2)^{3/2}}.
$$

The [electrostatic boundary conditions at a conductor](../../../../electrostatic-boundary-conditions-at-a-conductor.md), with outward [unit normal](../../../../unit-normal.md) $+\widehat{\mathbf z}$ and zero interior [electric field](../../../../electric-field-split.md), give the induced [surface charge density](../../../../surface-charge-density.md)

$$
\boxed{\sigma(r)=\epsilon_0 E_z(r,0^+)
=-\frac{QD}{2\pi(r^2+D^2)^{3/2}}.}
$$

Finally integrate over annuli of [area](../../../../surface-area.md) $2\pi r\,dr$:

$$
Q_{\rm ind}=\int_0^\infty\sigma(r)2\pi r\,dr
=-QD\int_0^\infty\frac{r\,dr}{(r^2+D^2)^{3/2}}
=-QD\left[-\frac1{\sqrt{r^2+D^2}}\right]_0^\infty,
\qquad\boxed{Q_{\rm ind}=-Q.}
$$

The [image charge](../../../../image-charge.md) is a computational device, not a real charge below the plane. For a finite conducting sphere, its induced polarization would change the point-source approximation; the stated negligible [radius](../../../../radius.md) is essential.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
