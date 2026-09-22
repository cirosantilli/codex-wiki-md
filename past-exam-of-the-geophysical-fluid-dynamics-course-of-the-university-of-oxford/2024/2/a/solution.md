<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use eastward $x$, northward $y$, constant layer depth $H$, constant reference [density](../../../../density.md) $\rho_0$, and a depth-independent horizontal [velocity field](../../../../velocity-field.md) $(u,v)$. Assume a flat bottom and a rigid upper boundary, giving the two-dimensional [incompressibility condition](../../../../incompressible-flow.md) $u_x+v_y=0$. The [traditional approximation](../../../../traditional-approximation-geophysical-fluid-dynamics.md) retains only the vertical component of planetary rotation in the horizontal equations. Take the [Coriolis parameter](../../../../coriolis-parameter.md) $f=f(y)$, a constant [linear drag](../../../../linear-drag.md) rate $r$, and no other torques. The component [Cauchy momentum equations](../../../../cauchy-momentum-equation.md) are

$$
Du-fv=-\frac{p_x}{\rho_0}+\frac{\tau_s}{\rho_0H}-ru,
\qquad Dv+fu=-\frac{p_y}{\rho_0}-rv,
\qquad D=\partial_t+u\partial_x+v\partial_y.
$$

Define [relative vorticity](../../../../relative-vorticity.md) $\xi=v_x-u_y$. Apply $\partial_x$ to the second equation and subtract $\partial_y$ of the first. The [pressure gradient force](../../../../pressure-gradient-force.md) has zero [curl](../../../../curl.md) because $\rho_0$ is constant and mixed [partial derivatives](../../../../partial-derivative.md) commute. Direct expansion of the material-acceleration terms gives

$$
\partial_x(Dv)-\partial_y(Du)
=D\xi+(u_x+v_y)\xi=D\xi.
$$

The [curl](../../../../curl.md) of the rotation terms is

$$
\partial_x(fu)+\partial_y(fv)
=f(u_x+v_y)+vf_y=vf_y.
$$

The imposed zonal [wind stress](../../../../wind-stress.md) contributes $-\tau_{s,y}/(\rho_0H)$, and constant [linear drag](../../../../linear-drag.md) contributes $-r\xi$. Hence

$$
D\xi+vf_y=-\frac{\tau_{s,y}}{\rho_0H}-r\xi.
$$

Since $Df=vf_y$, defining [absolute vorticity](../../../../absolute-vorticity.md) $\zeta=\xi+f$ gives

$$
\boxed{\left(\partial_t+u\partial_x+v\partial_y\right)\zeta
=-\frac1{\rho_0H}\frac{\partial\tau_s}{\partial y}-r\xi.}
$$

Without the [incompressibility condition](../../../../incompressible-flow.md), the left-hand side would contain the stretching term $\zeta\nabla_h\cdot\mathbf u$. Variable layer depth, variable [density](../../../../density.md) or spatially varying [linear drag](../../../../linear-drag.md) would introduce further terms. No small-[Rossby number](../../../../rossby-number.md) assumption was needed to obtain this constant-depth [vorticity equation](../../../../vorticity-equation.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the geophysical fluid dynamics course of the University of Oxford](../../../split.md)
5. [Geophysical fluid dynamics course of the University of Oxford](../../../../geophysical-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
