<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Treat the [free surface](../../../../../free-surface.md) as the material level set $F(x,y,t)=y-\eta(x,t)=0$. The [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) $DF/Dt=0$, with $\mathbf u=\nabla\phi$, gives

$$
-\eta_t-\phi_x\eta_x+\phi_y=0,
\qquad
\boxed{\phi_y=\eta_t+\phi_x\eta_x\quad\text{on }y=\eta.}
$$

This says that fluid initially on the [free surface](../../../../../free-surface.md) remains on it.

For constant [mass density](../../../../../density.md) $\rho$, the [Euler momentum equation](../../../../../euler-equations-for-an-inviscid-fluid-split.md) under [gravity](../../../../../gravity.md) is $D\mathbf u/Dt=-\nabla p/\rho-g\mathbf e_y$. Since the flow is [irrotational](../../../../../irrotational-vector-field.md), $(\mathbf u\cdot\nabla)\mathbf u=\nabla(|\mathbf u|^2/2)$. Integration in space therefore gives the [Unsteady Bernoulli equation](../../../../../unsteady-bernoulli-equation.md)

$$
\phi_t+\frac12|\nabla\phi|^2+\frac p\rho+gy=B(t).
$$

At the [free surface](../../../../../free-surface.md), $p=P_a$ and $y=\eta$. Adding a function $G(t)$ to the [velocity potential](../../../../../velocity-potential.md) leaves the [velocity field](../../../../../velocity-field.md) unchanged; choose $G'=P_a/\rho-B(t)$. With this choice the surface [dynamic boundary condition for an inviscid interface](../../../../../dynamic-boundary-condition-for-an-inviscid-interface.md) becomes

$$
\boxed{\phi_t+\frac12|\nabla\phi|^2+g\eta=0\quad\text{on }y=\eta.}
$$

The constant atmospheric [pressure](../../../../../pressure-split.md) has been absorbed into this choice of potential.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the fluids and waves course of the University of Oxford](../../../../split.md)
6. [Fluids and waves course of the University of Oxford](../../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
