<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In a [Cartesian coordinate system](../../../../cartesian-coordinate-system.md) the leading [electric dipole field](../../../../electric-dipole-field.md) gives

$$
\mathbf F(x,y)=\frac{k_epQ}{(x^2+y^2)^{5/2}}\left(3xy\,\hat{\mathbf x}+(2y^2-x^2)\,\hat{\mathbf y}\right).
$$

Therefore

$$
\boxed{\mathbf F(-d,0)=\mathbf F(d,0)=-\frac{k_epQ}{d^3}\hat{\mathbf y},\qquad
\mathbf F(0,-d)=\frac{2k_epQ}{d^3}\hat{\mathbf y}.}
$$

The [force](../../../../force-split.md) is downwards on the equator and upwards on the negative axial side. A free positive [electric charge](../../../../electric-charge-split.md) released from rest at the left-hand point initially accelerates downwards. As it moves into $x<0,y<0$, the [force](../../../../force-split.md) also acquires a positive $x$ component. Its path bends toward the right; the [force](../../../../force-split.md) continually changes as its position changes. An initial velocity was not specified, so the following more precise trajectory assumes release from rest and neglects [radiation reaction](../../../../radiation-reaction.md).

There is a useful exact result within the point-[electric dipole](../../../../electric-dipole.md) approximation. Put $A=k_epQ>0$; the [potential energy](../../../../potential-energy.md) is $U=Ay/r^3$, a [homogeneous function](../../../../homogeneous-function.md) of degree $-2$. Thus $\mathbf r\cdot\mathbf F=2U$. For a particle of mass $m$, [Newton's second law](../../../../newton-s-second-law.md) and [conservation of energy](../../../../conservation-of-energy.md) imply

$$
\frac{d^2r^2}{dt^2}=2v^2+\frac2m\mathbf r\cdot\mathbf F=\frac4m(K+U)=\frac{4E}{m}.
$$

At release, both [kinetic energy](../../../../kinetic-energy.md) and [potential energy](../../../../potential-energy.md) vanish, so $E=0$; also $d(r^2)/dt=0$. Consequently $r=d$ throughout the motion. Parametrize the lower semicircle by $x=-d\cos\alpha$, $y=-d\sin\alpha$. Then

$$
\dot\alpha^2=\frac{2A}{md^4}\sin\alpha,\qquad
\ddot\alpha=\frac{A}{md^4}\cos\alpha.
$$

The [electric charge](../../../../electric-charge-split.md) gains speed until the bottom point, where the [force](../../../../force-split.md) is inward and the speed is $\sqrt{2A/(md^2)}$. It then slows, reaches $(d,0)$ at rest, and reverses. Thus, under these assumptions,

$$
\boxed{\text{the charge oscillates along the lower semicircle }x^2+y^2=d^2,\quad y\leq0.}
$$

Its trajectory is not an [electric field line](../../../../electric-field-line.md): the [force](../../../../force-split.md) determines acceleration, rather than velocity direction. For the finite two-charge [electric dipole](../../../../electric-dipole.md), corrections of order $a^2/d^2$ perturb the circular trajectory; an arbitrary nonzero initial velocity also changes it.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
