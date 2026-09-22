<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\mathsf R(\alpha)$ denote the planar [rotation matrix](../../../../rotation-matrix.md), and choose the initial cup center on the positive $x$ axis, as in the requested equations. Its [trajectory](../../../../trajectory.md) is $\mathbf C(t)=R(\cos\Omega t,\sin\Omega t)$. The handle rotates relative to the radial line at signed rate $\phi$, so its absolute [angular velocity](../../../../angular-velocity.md) is $\nu=\Omega+\phi$. A positive recurrence time is $2\pi/|\phi|$; the sign records [rotation](../../../../rotation-mathematics.md) direction.

Writing $\mathbf q=(x_1,y_1)$, the relation is

$$
\boxed{\mathbf r=\mathbf C+\mathsf R(\nu t)\mathbf q,}
$$

or explicitly

$$
x=R\cos\Omega t+x_1\cos\nu t-y_1\sin\nu t,
\qquad
y=R\sin\Omega t+x_1\sin\nu t+y_1\cos\nu t.
$$

One obtains the same result by rotating cup coordinates through $\phi t$ into the radially aligned axes, then rotating through $\Omega t$ into the inertial axes.

At $\phi=-\Omega$, $\nu=0$, and

$$
\boxed{x=R\cos\Omega t+x_1,\qquad y=R\sin\Omega t+y_1.}
$$

The axes maintain a fixed orientation in inertial space while their origin accelerates around a circle. This is translation without [rotation](../../../../rotation-mathematics.md) of the cup frame; it is not an inertial frame because the origin accelerates. In particular its inertial correction is a spatially uniform fictitious force, rather than a [Coriolis force](../../../../coriolis-force.md) from [rotation](../../../../rotation-mathematics.md) of these axes.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the classical mechanics course of Part B of the physics course of the University of Oxford](../../../split.md)
5. [Classical mechanics course of Part B of the physics course of the University of Oxford](../../../../classical-mechanics-course-of-part-b-of-the-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
