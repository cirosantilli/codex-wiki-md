<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume $U_c=(U_a+U_b)/2>0$ and set $\Delta U=U_a-U_b>0$. With $\nu_T=C\Delta U\delta(x)$ independent of $y$, balancing streamwise transport with transverse mixing gives a layer width proportional to $x$. Write its constant slope as

$$
\boxed{\delta'=\frac{S\Delta U}{U_c},\qquad
\delta(x)=\frac{S\Delta U}{U_c}x.}
$$

Here $S>0$ is a spreading constant associated with the chosen definition of thickness; it is unrelated to the capillary $S$ in Question 1. The origin $x=0$ selects zero virtual-origin offset.

Define $a=\sqrt{S/C}$, $\xi=ay/\delta$, and introduce the [stream function](../../../../../stream-function.md)

$$
\psi=U_c\left[y+\frac\delta a F(\xi)\right],\qquad
U=\psi_y,\quad V=-\psi_x.
$$

This automatically satisfies [incompressibility](../../../../../incompressible-flow.md) and yields

$$
\boxed{U=U_c[1+F'(\xi)],\qquad
V=\Delta U\sqrt{CS}\,[\xi F'(\xi)-F(\xi)].}
$$

For the momentum equation, use $\xi_x=-\xi\delta'/\delta$ and $\xi_y=a/\delta$:

$$
\begin{aligned}
U_x&=-U_c\frac{\delta'}\delta\xi F'',&
U_y&=U_c\frac a\delta F'',\\
UU_x+VU_y&=-\frac{U_c^2\delta'}\delta(\xi+F)F'',&
\nu_TU_{yy}&=\frac{S\Delta U\,U_c}\delta F'''.
\end{aligned}
$$

Because $U_c^2\delta'=S\Delta U\,U_c$, the common coefficient cancels, giving the [turbulent mixing-layer similarity equation](../../../../../turbulent-mixing-layer-similarity-equation.md)

$$
\boxed{F'''+(\xi+F)F''=0.}
$$

The [boundary layer](../../../../../boundary-layer.md) approximation also requires $S\Delta U/U_c\ll1$, consistently with the assumed slow spreading.

## ↑ Ancestors (13)

1. [I](../i.md)
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
