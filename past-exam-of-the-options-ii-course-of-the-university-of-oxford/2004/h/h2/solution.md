<h1 id="h/h2/solution">Solution</h1>

↑ **Parent:** [H2](../h2.md)

At fractional position $s$ along a straight rigid rod, the velocity is $(1-s)u+sv$. Uniform mass per unit length gives

$$
T=\frac m2\int_0^1|(1-s)u+sv|^2ds
=\boxed{\frac m6(|u|^2+u\cdot v+|v|^2)}.
$$

The string constraints are $x_1^2+y_1^2+(-l+z_1)^2=l^2$ and $x_2^2+y_2^2+(-2l+z_2)^2=4l^2$. Their first-order terms give $z_1=z_2=0$. Their second-order terms then give

$$
\boxed{z_1=(x_1^2+y_1^2)/(2l),\qquad z_2=(x_2^2+y_2^2)/(4l).}
$$

The rod constraint is $(l+x_2-x_1)^2+(y_2-y_1)^2+(-l+z_2-z_1)^2=2l^2$. Its first-order part is $2l(x_2-x_1)=0$, hence $x_2=x_1$ to first order.

The [centre of mass](../../../../center-of-mass.md) rises by $(z_1+z_2)/2$. Substituting the quadratic string expansions and the linear relation between the horizontal displacements gives

$$
\boxed{V=\frac{mg}{8l}(3x_1^2+2y_1^2+y_2^2).}
$$

Vertical velocities contribute only at fourth order to the [energy](../../../../energy-split.md). Substituting $u=(\dot x_1,\dot y_1,0)$ and $v=(\dot x_1,\dot y_2,0)$ into the rod [energy](../../../../energy-split.md) gives

$$
\boxed{T=\frac m6(3\dot x_1^2+\dot y_1^2+\dot y_2^2+\dot y_1\dot y_2).}
$$

The decoupled $x_1$ equation is $\ddot x_1+3gx_1/(4l)=0$. For the other two coordinates put $\kappa=3g/(2l)$; their equations are

$$
2\ddot y_1+\ddot y_2+2\kappa y_1=0,\qquad
\ddot y_1+2\ddot y_2+\kappa y_2=0.
$$

A normal-mode ansatz gives $3\omega^4-6\kappa\omega^2+2\kappa^2=0$, whose roots are $\omega^2=g(3\pm\sqrt3)/(2l)$. The corresponding displacement ratios are $y_2/y_1=1\mp\sqrt3$. Therefore the three periods are

$$
\boxed{\frac{2\pi}{\sqrt{3g/(4l)}},\qquad\frac{2\pi}{\sqrt{g(3+\sqrt3)/(2l)}},\qquad\frac{2\pi}{\sqrt{g(3-\sqrt3)/(2l)}}.}
$$

## ↑ Ancestors (12)

1. [H2](../h2.md)
2. [H](../../h.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
