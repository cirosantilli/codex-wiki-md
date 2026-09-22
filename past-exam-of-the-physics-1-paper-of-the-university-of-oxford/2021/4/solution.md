<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Choose the vertical $z$ axis downward, and measure the [polar angle](../../../polar-angle.md) $\theta$ from it. With [azimuth](../../../azimuth.md) $\phi$ and fixed rod [length](../../../length.md) $r$, the [Cartesian coordinates](../../../cartesian-coordinate-system.md) are

$$
\boxed{x=r\sin\theta\cos\phi,\qquad y=r\sin\theta\sin\phi,\qquad z=r\cos\theta.}
$$

The massless rod has no [kinetic energy](../../../kinetic-energy.md). Differentiating these [coordinates](../../../coordinate-linear-algebra.md) and adding the squared components of [velocity](../../../velocity.md) yields

$$
v^2=\dot x^2+\dot y^2+\dot z^2
=r^2\left(\dot\theta^2+\sin^2\theta\,\dot\phi^2\right).
$$

The [gravitational potential energy](../../../gravitational-energy.md) is $V=-mgz=-mgr\cos\theta$, up to an arbitrary constant. The [Lagrangian](../../../lagrangian.md) of this [spherical pendulum](../../../spherical-pendulum.md) is therefore

$$
\boxed{L=\frac12mr^2\left(\dot\theta^2+\sin^2\theta\,\dot\phi^2\right)+mgr\cos\theta.}
$$

Applying the [Euler-Lagrange equation](../../../euler-lagrange-equation.md) to the two [generalized coordinates](../../../generalized-coordinate.md) gives

$$
mr^2\ddot\theta-mr^2\sin\theta\cos\theta\,\dot\phi^2+mgr\sin\theta=0,
\qquad
\frac{d}{dt}\left(mr^2\sin^2\theta\,\dot\phi\right)=0.
$$

Equivalently, away from the [coordinate singularities](../../../coordinate-singularity.md) at the poles,

$$
\boxed{\ddot\theta=\sin\theta\cos\theta\,\dot\phi^2-\frac gr\sin\theta,\qquad
\ddot\phi+2\cot\theta\,\dot\theta\dot\phi=0.}
$$

Since $L$ is independent of $\phi$, the [azimuth](../../../azimuth.md) is a [cyclic coordinate](../../../cyclic-coordinate.md). Its [conjugate momentum](../../../canonical-momentum.md)

$$
p_\phi=mr^2\sin^2\theta\,\dot\phi
$$

is the conserved component of [angular momentum](../../../angular-momentum.md) about the downward vertical axis. The [polar angle](../../../polar-angle.md) is not a [cyclic coordinate](../../../cyclic-coordinate.md). Using an upward $z$ axis instead reverses the sign of the cosine term in $L$ and of the corresponding gravity term; it describes the same motion with the opposite [polar angle](../../../polar-angle.md) convention.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2021](../../2021-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
