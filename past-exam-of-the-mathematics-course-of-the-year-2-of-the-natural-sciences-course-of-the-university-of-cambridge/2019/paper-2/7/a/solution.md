<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an ordinary conservative mechanical system, choose [generalized coordinates](../../../../../generalized-coordinate.md) $q_i$ measured from a static [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md). Assume the [kinetic energy](../../../../../kinetic-energy.md) is quadratic in velocities and there are no velocity-dependent forces. Expanding about equilibrium, the linear term in the [potential energy](../../../../../potential-energy.md) vanishes. Retaining only terms of total degree two gives the [small oscillation](../../../../../small-oscillation.md) [Lagrangian](../../../../../lagrangian.md)

$$
\boxed{L=\frac12\dot{\mathbf q}^{\,T}M\dot{\mathbf q}-\frac12\mathbf q^TK\mathbf q},\qquad
M_{ij}=\left.\frac{\partial^2T}{\partial\dot q_i\partial\dot q_j}\right|_0,\quad
K_{ij}=\left.\frac{\partial^2V}{\partial q_i\partial q_j}\right|_0.
$$

An irrelevant constant has been dropped. Coordinate dependence of $M$ contributes only terms of third or higher total degree. The matrices $M,K$ are symmetric, $M$ is positive definite for independent coordinates, and $K$ is positive semidefinite at a [stable equilibrium](../../../../../stable-equilibrium.md). The [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) are

$$
\boxed{M\ddot{\mathbf q}+K\mathbf q=0}.
$$

A [normal mode](../../../../../normal-mode.md) has a fixed [mode shape](../../../../../mode-shape.md) $\mathbf v$ and one time factor: $\mathbf q=\mathbf v Q(t)$. Its [angular frequency](../../../../../angular-frequency.md) $\omega$ solves the [generalized eigenvalue problem](../../../../../generalized-eigenvalue-problem.md) $K\mathbf v=\omega^2M\mathbf v$, with $\ddot Q+\omega^2Q=0$. Thus $\omega$ is the normal angular frequency, and the frequency in cycles per unit time is $\omega/(2\pi)$. A [zero mode](../../../../../zero-mode.md) satisfies $K\mathbf v=0$; its time dependence is $Q=A+Bt$, describing an unopposed displacement or uniform drift rather than a restoring oscillation.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [7](../../7.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
