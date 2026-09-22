<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Each [simple pendulum](../../../../simple-pendulum-split.md) moves in the vertical plane containing the pivots. Ignoring contact between the ideal rods and [point masses](../../../../point-mass.md), each rod can turn through a full [circle](../../../../circle.md). Thus the [configuration space](../../../../mechanical-configuration-space.md) is the [torus](../../../../torus.md)

$$
\boxed{\mathcal Q=S^1\times S^1.}
$$

Choose [generalized coordinates](../../../../generalized-coordinate.md) $\theta_1,\theta_2$, measured from the downward vertical, positive towards the right and understood modulo $2\pi$. These [angles](../../../../angle.md) are local coordinates on the [torus](../../../../torus.md), rather than a single globally one-to-one real [coordinate chart](../../../../manifold-chart.md). With upward Cartesian coordinate $y$, the bob [positions](../../../../position.md) are

$$
\mathbf r_1=(l\sin\theta_1,-l\cos\theta_1),\qquad
\mathbf r_2=(r+l\sin\theta_2,-l\cos\theta_2).
$$

Their [velocities](../../../../velocity.md) satisfy $|\dot{\mathbf r}_j|^2=l^2\dot\theta_j^2$, so [kinetic energy from Cartesian position vectors](../../../../kinetic-energy-from-cartesian-position-vectors.md) gives

$$
T=\frac{ml^2}{2}(\dot\theta_1^2+\dot\theta_2^2).
$$

The [spring](../../../../spring.md) length is the [Euclidean distance](../../../../euclidean-distance.md)

$$
d=|\mathbf r_2-\mathbf r_1|
=\sqrt{\bigl(r+l(\sin\theta_2-\sin\theta_1)\bigr)^2+l^2(\cos\theta_2-\cos\theta_1)^2}.
$$

Taking gravitational [potential energy](../../../../potential-energy.md) zero at pivot height gives $V_g=-mgl(\cos\theta_1+\cos\theta_2)$. The [spring](../../../../spring.md) [potential energy](../../../../potential-energy.md) is $V_s=k(d-r)^2/2$, since $r$ is its natural length. Consequently the [Lagrangian](../../../../lagrangian.md) is

$$
\boxed{L=T-V_g-V_s
=\frac{ml^2}{2}(\dot\theta_1^2+\dot\theta_2^2)
+mgl(\cos\theta_1+\cos\theta_2)-\frac{k}{2}(d-r)^2.}
$$

In the paper's notation $t(\theta_1,\theta_2)=V_s$; this function is distinct from the time variable. This is the [exact Lagrangian of two spring-coupled pendulums](../../../../exact-lagrangian-of-two-spring-coupled-pendulums.md).

One alternative [Lagrangian](../../../../lagrangian.md) is

$$
\boxed{\widetilde L=L-2mgl.}
$$

It corresponds to setting gravitational [potential energy](../../../../potential-energy.md) zero at the downward position. The constant disappears from every [Euler-Lagrange equation](../../../../euler-lagrange-equation.md). More generally, [total-time-derivative invariance of a Lagrangian](../../../../total-time-derivative-invariance-of-a-lagrangian.md) allows $\widetilde L=L+dF(\theta_1,\theta_2,t)/dt$ for any smooth $F$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the classical mechanics course of the University of Oxford](../../../split.md)
5. [Classical mechanics course of the University of Oxford](../../../../classical-mechanics-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
