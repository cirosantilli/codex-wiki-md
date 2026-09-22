<h1 id="2/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Set $x=L\tilde x$, $h=H\tilde h$, and $t=T\tilde t$. The [Boussinesq equation for an unconfined aquifer](../../../../../boussinesq-equation-for-an-unconfined-aquifer.md) becomes

$$
\frac{\phi H}{T}\tilde h_{\tilde t}
=\frac{KH^2}{L^2}(\tilde h\tilde h_{\tilde x})_{\tilde x}+R.
$$

Balance rainfall recharge with lateral drainage, and then with storage:

$$
\boxed{H=L\sqrt{\frac RK},\qquad
T=\frac{\phi H}{R}=\frac{\phi L}{\sqrt{KR}}.}
$$

Dropping tildes, the dimensionless equation is

$$
\boxed{h_t=(hh_x)_x+1.}
$$

The horizontal [Darcy velocity](../../../../../darcy-velocity.md), vertical [Darcy velocity](../../../../../darcy-velocity.md), and discharge scales are respectively $\sqrt{KR}$, $R$, and $RL$. Thus the vertical thickness scale is set by **rainfall balanced against [hydraulic conductivity](../../../../../hydraulic-conductivity.md) over the finite drainage length $L$**, rather than by [porosity](../../../../../porosity.md). The latter determines the storage time $T$. The [Dupuit approximation](../../../../../dupuit-approximation.md) requires $H/L=\sqrt{R/K}\ll1$ for these scales. The initially dry [initial condition](../../../../../initial-condition.md) is $h(x,0)=0$.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topics in fluid mechanics course of the University of Oxford](../../../../split.md)
6. [Topics in fluid mechanics course of the University of Oxford](../../../../../topics-in-fluid-mechanics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
