<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The two external stream [velocities](../../../../../velocity.md) impose

$$
\boxed{F'(+\infty)=\frac{\Delta U}{2U_c},\qquad
F'(-\infty)=-\frac{\Delta U}{2U_c}.}
$$

Let $r=\Delta U/U_c\ll1$ and seek $F=O(r)$ over $\xi=O(1)$. The nonlinear term $FF''$ is then $O(r^2)$, so the leading [ordinary differential equation](../../../../../ordinary-differential-equation.md) is

$$
F'''+\xi F''=0.
$$

For $G=F''$, this is the first-order [linear differential equation](../../../../../linear-differential-equation.md) $G'+\xi G=0$. Its [integrating factor](../../../../../integrating-factor.md) is $e^{\xi^2/2}$, giving $F''=M e^{-\xi^2/2}$. An [integration](../../../../../integral-split.md) using the [error function](../../../../../error-function.md) gives

$$
F'=M\sqrt{\frac\pi2}\operatorname{erf}(\xi/\sqrt2)+E.
$$

The two far-field [boundary conditions](../../../../../boundary-condition.md) require $E=0$ and $M=r/\sqrt{2\pi}$. A second [integration](../../../../../integral-split.md) uses

$$
\int\operatorname{erf}(\xi/\sqrt2)\,d\xi
=\xi\operatorname{erf}(\xi/\sqrt2)+\sqrt{\frac2\pi}e^{-\xi^2/2}.
$$

Consequently

$$
\boxed{F=A\xi\operatorname{erf}(\xi/\sqrt2)+Be^{-\xi^2/2}+D,
\qquad A=\frac{\Delta U}{2U_c},\quad
B=A\sqrt{\frac2\pi}=\frac{\Delta U}{U_c\sqrt{2\pi}}.}
$$

The relation between $A$ and $B$ cancels the extra $\xi e^{-\xi^2/2}$ term when differentiating. It gives the familiar [error function](../../../../../error-function.md) mean [velocity](../../../../../velocity.md) profile

$$
U=U_c+\frac{\Delta U}{2}\operatorname{erf}(\xi/\sqrt2)
$$

to first order in $r$. The additive constant $D=O(r)$ does not affect this [velocity](../../../../../velocity.md) profile at the retained order; its interpretation comes from the transverse [velocity](../../../../../velocity.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
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
