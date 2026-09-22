<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\delta\ll L$ be a representative mixing-layer thickness, $\epsilon_m=\delta/L$, and let $U_s$ be a representative streamwise [velocity](../../../../velocity.md). Use the scales

$$
x\sim L,\quad y\sim\delta,\quad U\sim U_s,\quad
V\sim\epsilon_m U_s,\quad P\sim\rho U_s^2.
$$

The transverse [velocity](../../../../velocity.md) scale follows from the mean [continuity equation](../../../../continuity-equation.md). For turbulent transverse transport to balance streamwise inertia,

$$
\frac{U_s^2}{L}\sim\frac{\nu_TU_s}{\delta^2},\qquad
\nu_T\sim\frac{U_s\delta^2}{L}.
$$

With this ordering, the streamwise eddy-stress [divergence](../../../../divergence.md) is

$$
\partial_x(2\nu_TU_x)+\partial_y[\nu_T(U_y+V_x)]
=\partial_y(\nu_TU_y)+O(\epsilon_m^2U_s^2/L).
$$

Thus transverse diffusion of streamwise [linear momentum](../../../../momentum-split.md) is retained, while streamwise diffusion and the $V_x$ contribution are smaller by $\epsilon_m^2$. Molecular [kinematic viscosity](../../../../kinematic-viscosity.md) is neglected where $\nu_T\gg\nu$.

In the transverse momentum equation, inertia and the retained eddy stresses have scale $\epsilon_m U_s^2/L$, whereas an order-one transverse [pressure](../../../../pressure-split.md) variation would give $P_y/\rho\sim U_s^2/(\epsilon_m L)$. Hence the leading dimensionless transverse balance is $P_y=0$. The resulting [boundary layer](../../../../boundary-layer.md) equations for the [planar turbulent mixing layer](../../../../planar-turbulent-mixing-layer.md) are

$$
\boxed{\begin{aligned}
U_x+V_y&=0,\\
UU_x+VU_y&=-\rho^{-1}P_x+\partial_y(\nu_TU_y),\\
0&=-\rho^{-1}P_y.
\end{aligned}}
$$

Here $\nu_T=\mu_T/\rho$. The effective [pressure](../../../../pressure-split.md) convention explained in part (a)(iii) is understood. Since the outer streams have uniform horizontal [velocities](../../../../velocity.md), their inviscid momentum equations give $P_x=0$; choosing the far-field [gauge pressure](../../../../gauge-pressure.md) as zero gives $P=0$ throughout this approximation.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../../split.md)
5. [Topics in fluid mechanics course of the University of Oxford](../../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
