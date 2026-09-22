<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [rolling disk with a rim point mass](../../../../rolling-disk-with-a-rim-point-mass.md), impose [rolling without slipping](../../../../rolling-without-slipping.md) and take the clockwise angular displacement $\theta$ from the configuration with the extra [mass](../../../../mass.md) at the bottom. The disk centre has $x_C=R\theta$ and $y_C=R$. The extra [mass](../../../../mass.md) has

$$
x_M=R(\theta-\sin\theta),\qquad y_M=R(1-\cos\theta),\qquad v_M^2=2R^2(1-\cos\theta)\dot\theta^2.
$$

The disk's translational and [rotational kinetic energies](../../../../rotational-kinetic-energy.md) sum to $3MR^2\dot\theta^2/2$. Including the rim [mass](../../../../mass.md) gives

$$
T=\frac12MR^2(5-2\cos\theta)\dot\theta^2,\qquad U=MgR(1-\cos\theta).
$$

The exact [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) is

$$
MR^2(5-2\cos\theta)\ddot\theta+MR^2\sin\theta\,\dot\theta^2+MgR\sin\theta=0.
$$

To first order, $3MR^2\ddot\theta+MgR\theta=0$. Therefore

$$
\boxed{\omega_{\rm roll}=\sqrt{\frac{g}{3R}},\qquad \frac{T_{\rm roll}}{T_{\rm fixed}}=\sqrt{\frac32}.}
$$

At the bottom the extra [mass](../../../../mass.md) is instantaneously at the contact point and has no first-order [velocity](../../../../velocity.md). The increased effective inertia comes from the moving disk. Static [friction](../../../../friction.md) enforces the rolling constraint without doing [work](../../../../work.md) at the stationary contact.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the physics 1 paper of the University of Oxford](../../../split.md)
5. [Physics 1 paper of the University of Oxford](../../../../physics-1-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
