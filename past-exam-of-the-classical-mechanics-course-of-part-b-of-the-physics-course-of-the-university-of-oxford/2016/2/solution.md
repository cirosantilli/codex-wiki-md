<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [constant of motion](../../../conserved-quantity.md) is a function $I(\mathbf q,\mathbf p,t)$ whose [total derivative](../../../total-derivative.md) vanishes along every physical [trajectory](../../../trajectory.md). It may depend explicitly on time; arbitrary functions of conserved quantities are also conserved, so a count normally concerns a specified independent set or symmetry generators.

For a fixed-time infinitesimal variation $\delta q_i=\epsilon\xi_i(\mathbf q,t)$, suppose $\delta L=\epsilon\,dB/dt$. On a solution of the [Euler-Lagrange equations](../../../euler-lagrange-equation.md),

$$
\frac{\delta L}{\epsilon}=\sum_i\left(L_{q_i}\xi_i+p_i\dot\xi_i\right)
=\frac d{dt}\sum_ip_i\xi_i.
$$

Therefore [Noether theorem](../../../noether-theorem.md) gives

$$
\boxed{I=\sum_i p_i\xi_i-B,\qquad \frac{dI}{dt}=0.}
$$

For a transformation also changing time by $\delta t=\epsilon\tau$, the [action](../../../action.md) variation includes $L\,d(\delta t)/dt$, and the transformed [velocity](../../../velocity.md) varies by $\epsilon(\dot\xi_i-\dot q_i\dot\tau)$. The same [integration by parts](../../../integration-by-parts.md) gives the general point-symmetry charge

$$
\boxed{I=\sum_ip_i\xi_i-H\tau-B.}
$$

Thus a [time-translation symmetry](../../../time-translation-symmetry.md) gives the [energy](../../../energy-split.md), a spatial translation gives the corresponding total [momentum](../../../momentum-split.md), and a [rotation](../../../rotation-mathematics.md) gives its angular-momentum generator. The required symmetry is a symmetry of the [action](../../../action.md), allowing a boundary term; demanding that the numerical value of the [Lagrangian](../../../lagrangian.md) remain strictly unchanged is unnecessarily restrictive. Conversely, explicit time dependence of a [Lagrangian](../../../lagrangian.md) generally prevents conservation of its [energy](../../../energy-split.md) even while other charges survive.[Chapter 2, section 2.6 and 2.6.1, continuous symmetries, conserved charges and Noether's theorem](../../../classical-dynamics-by-david-tong.md)

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2016](../../2016-split.md)
3. [Past exam of the classical mechanics course of Part B of the physics course of the University of Oxford](../../split.md)
4. [Classical mechanics course of Part B of the physics course of the University of Oxford](../../../classical-mechanics-course-of-part-b-of-the-physics-course-of-the-university-of-oxford.md)
5. [Year 3 of the physics course of the University of Oxford](../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
