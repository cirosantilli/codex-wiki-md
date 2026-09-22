<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

In the inertial [centre of mass](../../../center-of-mass.md) frame, the [Lagrangian mechanics](../../../lagrangian-mechanics-split.md) description starts from [kinetic energy](../../../kinetic-energy.md) minus [potential energy](../../../potential-energy.md):

$$
L=\frac12m_1|\dot{\mathbf r}_1|^2
+\frac12m_2|\dot{\mathbf r}_2|^2-V(|\mathbf r_1-\mathbf r_2|).
$$

Define the [two-particle relative coordinate](../../../two-particle-relative-coordinate.md) $\mathbf r=\mathbf r_1-\mathbf r_2$. The [centre of mass](../../../center-of-mass.md) condition gives

$$
m_1\mathbf r_1+m_2\mathbf r_2=0,
\qquad
\mathbf r_1=\frac{m_2}{m_1+m_2}\mathbf r,
\quad
\mathbf r_2=-\frac{m_1}{m_1+m_2}\mathbf r.
$$

Substitution therefore gives

$$
\boxed{L=\frac12\mu|\dot{\mathbf r}|^2-V(r),
\qquad\mu=\frac{m_1m_2}{m_1+m_2},\quad r=|\mathbf r|.}
$$

The [Euler-Lagrange equation](../../../euler-lagrange-equation.md) is simply $\mu\ddot{\mathbf r}=-\nabla V(r)$. Thus [center-of-mass reduction](../../../center-of-mass-reduction.md) turns a [two-body problem](../../../two-body-problem.md) into a one-particle [central force](../../../central-force.md) problem with [reduced mass](../../../reduced-mass.md) $\mu$, reducing six position components to three relative components. In an arbitrary [inertial frame](../../../inertial-frame.md) one adds the independent [centre of mass](../../../center-of-mass.md) term $\tfrac12(m_1+m_2)|\dot{\mathbf R}|^2$; that free motion does not affect the relative solution. Since $V$ depends only on separation, [conservation of angular momentum](../../../conservation-of-angular-momentum.md) further confines a nonradial relative trajectory to a plane.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2021 resit](../../2021-resit-split.md)
3. [Past exam of the physics 1 paper of the University of Oxford](../../split.md)
4. [Physics 1 paper of the University of Oxford](../../../physics-1-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
