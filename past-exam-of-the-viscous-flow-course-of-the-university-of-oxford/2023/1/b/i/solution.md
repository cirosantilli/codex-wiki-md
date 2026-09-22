<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the [unidirectional flow](../../../../../unidirectional-flow.md) $\mathbf u=(0,0,w)$, [incompressibility](../../../../../incompressible-flow.md) gives $\partial_z w=0$. Hence $w=w(x,y,t)$, and the [convective acceleration](../../../../../convective-acceleration.md) $w\partial_z w$ vanishes. The transverse components of the [Navier-Stokes equation](../../../../../navier-stokes-equation.md) give $p_x=p_y=0$, while the axial component gives

$$
\rho\partial_t w=G+\mu(w_{xx}+w_{yy}).
$$

**A steady-flow assumption is implicit in the question.** Neither [unidirectional flow](../../../../../unidirectional-flow.md) nor a time-independent [pressure gradient](../../../../../pressure-gradient.md) alone eliminates $\partial_t w$: a decaying transient can be superposed on the final pipe profile. The native PDF does not explicitly say [steady flow](../../../../../steady-flow.md) in this part. For the intended [steady flow](../../../../../steady-flow.md), $w_t=0$, and therefore

$$
\boxed{w_{xx}+w_{yy}=-\frac G\mu.}
$$

Taking the pipe walls to be stationary, the [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) is

$$
\boxed{w(\pm a,y)=0\quad(-b\leq y\leq b),\qquad
w(x,\pm b)=0\quad(-a\leq x\leq a).}
$$

The [no-penetration boundary condition](../../../../../no-penetration-boundary-condition.md) is already satisfied by the assumed [velocity field](../../../../../velocity-field.md). This is the [Poisson equation](../../../../../poisson-s-equation.md) defining [rectangular duct flow](../../../../../rectangular-duct-flow.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the viscous flow course of the University of Oxford](../../../../split.md)
6. [Viscous flow course of the University of Oxford](../../../../../viscous-flow-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
