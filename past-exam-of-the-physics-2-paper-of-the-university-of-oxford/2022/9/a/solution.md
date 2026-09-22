<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set the grounded plane at $z=0$ and the real [point charge](../../../../point-charge.md) at $(0,0,h)$. The [image charge](../../../../image-charge.md) $-q$ at $(0,0,-h)$ makes the [electrostatic potential](../../../../electric-potential.md) vanish throughout the plane. The [uniqueness theorem for the electrostatic potential](../../../../uniqueness-theorem-for-the-electrostatic-potential.md) then identifies the physical solution in $z>0$:

$$
\Phi(a,z)=\frac{q}{4\pi\epsilon_0}\left[\frac1{\sqrt{a^2+(z-h)^2}}-\frac1{\sqrt{a^2+(z+h)^2}}\right].
$$

The normal [electric field](../../../../electric-field-split.md) is $E_z=-\partial_z\Phi$. Differentiation gives

$$
E_z(a,z)=\frac{q}{4\pi\epsilon_0}\left[\frac{z-h}{[a^2+(z-h)^2]^{3/2}}-\frac{z+h}{[a^2+(z+h)^2]^{3/2}}\right],
$$

and therefore

$$
\boxed{E_z(a,0^+)=-\frac{q}{2\pi\epsilon_0}\frac{h}{(a^2+h^2)^{3/2}}.}
$$

For $q>0$ the [electric field](../../../../electric-field-split.md) points into the [electrical conductor](../../../../electrical-conductor.md), consistently with negative induced [surface charge density](../../../../surface-charge-density.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [9](../../9.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
