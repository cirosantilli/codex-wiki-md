<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For ordinary conservative [classical mechanics](../../../classical-mechanics-split.md), the [Lagrangian](../../../lagrangian.md) is $L(q,\dot q,t)=T-V$, where $T$ is the [kinetic energy](../../../kinetic-energy.md) and $V$ the [potential energy](../../../potential-energy.md). More generally it is the function whose [action](../../../action.md) $\int L\,dt$ satisfies the [principle of stationary action](../../../principle-of-stationary-action.md). The [canonical momenta](../../../canonical-momentum.md) and [Hamiltonian](../../../hamiltonian.md) are

$$
p_i=\frac{\partial L}{\partial\dot q_i},\qquad
\boxed{H(q,p,t)=\sum_i p_i\dot q_i-L(q,\dot q,t).}
$$

For a [regular Lagrangian](../../../regular-lagrangian.md), the first equations can be inverted to express the [generalized velocities](../../../generalized-velocity.md) in terms of $q,p,t$; this defines the [Legendre transform](../../../convex-conjugate.md) on [phase space](../../../phase-space.md).

Along a solution of the [Euler-Lagrange equations](../../../euler-lagrange-equation.md), $\dot p_i=\partial L/\partial q_i$. Taking a total [time derivative](../../../time-derivative.md) gives

$$
\begin{aligned}
\frac{dH}{dt}
&=\sum_i\left(\dot p_i\dot q_i+p_i\ddot q_i\right)
-\sum_i\left(\frac{\partial L}{\partial q_i}\dot q_i+
\frac{\partial L}{\partial\dot q_i}\ddot q_i\right)
-\frac{\partial L}{\partial t}\\
&=-\frac{\partial L}{\partial t}.
\end{aligned}
$$

Thus an autonomous [Lagrangian](../../../lagrangian.md) has

$$
\boxed{\frac{dH}{dt}=0.}
$$

For the usual time-independent mechanical coordinates and a velocity-independent [potential energy](../../../potential-energy.md), the [kinetic energy](../../../kinetic-energy.md) is quadratic in the [generalized velocities](../../../generalized-velocity.md), so $\sum_i p_i\dot q_i=2T$ and $H=T+V$. The conservation proof itself uses the [Euler-Lagrange equations](../../../euler-lagrange-equation.md), rather than assuming this special expression for [energy](../../../energy-split.md).

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2018](../../2018-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
