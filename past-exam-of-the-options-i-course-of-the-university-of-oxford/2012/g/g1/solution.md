<h1 id="g/g1/solution">Solution</h1>

↑ **Parent:** [G1](../g1.md)

For variations vanishing at the endpoints, the [Euler-Lagrange equations](../../../../euler-lagrange-equation.md) are

$$
\boxed{\frac d{dt}F_{\dot r}-F_r=0,\qquad
\frac d{dt}F_{\dot\theta}-F_\theta=0.}
$$

Differentiate the stated energy expression using the [chain rule](../../../../chain-rule.md). The acceleration terms cancel, leaving

$$
\begin{aligned}
\frac{dH}{dt}
&=\dot r\left(\frac d{dt}F_{\dot r}-F_r\right)
+\dot\theta\left(\frac d{dt}F_{\dot\theta}-F_\theta\right)-F_t.
\end{aligned}
$$

Along a stationary trajectory the two brackets vanish. Thus $dH/dt=-F_t$, and in the absence of explicit time dependence $\boxed{H\text{ is constant}}$.

In plane [polar coordinates](../../../../polar-coordinates.md), the squared speed is $\dot r^2+r^2\dot\theta^2$, so the [kinetic energy](../../../../kinetic-energy.md) is $T=\tfrac12m(\dot r^2+r^2\dot\theta^2)$. An inverse-square central [gravitational force](../../../../gravitational-force.md) has [potential energy](../../../../potential-energy.md) proportional to $1/r$. With the sign convention printed in this paper, write $V=km/r$, giving

$$
F=T-V=\frac m2(\dot r^2+r^2\dot\theta^2)-\frac{km}{r}.
$$

For attraction to a star of mass $M_\star$, this convention has $k=-GM_\star<0$. Keeping $k$ real and signed is essential; no sign is changed in differentiating the printed functional.

Since $F_r=mr\dot\theta^2+km/r^2$, $F_{\dot r}=m\dot r$, $F_\theta=0$ and $F_{\dot\theta}=mr^2\dot\theta$, the equations of motion are

$$
\boxed{\ddot r-r\dot\theta^2=\frac{k}{r^2},\qquad
\frac d{dt}(mr^2\dot\theta)=0.}
$$

The second equation gives the conserved [angular momentum](../../../../angular-momentum.md) $J=mr^2\dot\theta$; equivalently $r\ddot\theta+2\dot r\dot\theta=0$. The autonomous-functional identity gives a second conserved quantity,

$$
\boxed{H=\dot rF_{\dot r}+\dot\theta F_{\dot\theta}-F
=\frac m2(\dot r^2+r^2\dot\theta^2)+\frac{km}{r}=T+V.}
$$

This is the total [mechanical energy](../../../../mechanical-energy.md); for attractive gravity the potential contribution is negative because $k<0$.

## ↑ Ancestors (12)

1. [G1](../g1.md)
2. [G](../../g.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
