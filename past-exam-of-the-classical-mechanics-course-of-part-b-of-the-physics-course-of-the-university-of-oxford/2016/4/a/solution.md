<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix an initial event $(q_i,t_i)$. For each reachable final event $(q_f,t_f)$, evaluate the [action](../../../../action.md) on a classical path satisfying those endpoints. On a chosen local branch this produces Hamilton's principal function $S(q_f,t_f)$, rather than a functional of every possible path. Multiple classical paths may make this function multivalued, so the derivation is local to a branch.

Allow the final event to vary. The integrated interior variation vanishes by the [Euler-Lagrange equations](../../../../euler-lagrange-equation.md). The endpoint variation must distinguish the total coordinate change from the change at fixed time: $\delta q(t_f)=\delta q_f-\dot q_f\delta t_f$. Consequently

$$
\delta S=\sum_ip_{i,f}(\delta q_{i,f}-\dot q_{i,f}\delta t_f)+L_f\delta t_f
=\sum_ip_{i,f}\delta q_{i,f}-H_f\delta t_f.
$$

Hence $p_i=\partial S/\partial q_i$ and $\partial S/\partial t=-H$. Eliminating the [momenta](../../../../momentum-split.md) yields the [Hamilton-Jacobi equation](../../../../hamilton-jacobi-equation.md)

$$
\boxed{\frac{\partial S}{\partial t}+H\left(q,\frac{\partial S}{\partial q},t\right)=0.}
$$

A [complete integral of the Hamilton-Jacobi equation](../../../../complete-integral-of-the-hamilton-jacobi-equation.md) depends on $n$ suitable independent constants for $n$ coordinates; differentiating it with respect to those constants supplies the conjugate integration constants needed to reconstruct [trajectories](../../../../trajectory.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
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
