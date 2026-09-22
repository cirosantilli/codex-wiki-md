<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [WKB approximation](../../../../wkb-approximation.md) fails at a simple [classical turning point](../../../../classical-turning-point.md) $x_t$, because $p(x_t)=0$ makes its amplitude singular and violates the [WKB validity condition](../../../../wkb-validity-condition.md). Locally replace $V(x)-E$ by $V'(x_t)(x-x_t)$. For a forbidden region on the right, $V'(x_t)>0$ and the rescaled coordinate $z=[2mV'(x_t)/\hbar^2]^{1/3}(x-x_t)$ changes the time-independent [Schrödinger equation](../../../../schrodinger-equation.md) into the [Airy ordinary differential equation](../../../../airy-ordinary-differential-equation.md) $\psi_{zz}-z\psi=0$. Reversing the coordinate handles a forbidden region on the left.

The two independent [Airy functions](../../../../airy-function.md) have asymptotic forms, for $z,w>0$,

$$
\begin{aligned}
\operatorname{Ai}(z)&\sim\frac{z^{-1/4}}{2\sqrt\pi}e^{-2z^{3/2}/3},&\operatorname{Bi}(z)&\sim\frac{z^{-1/4}}{\sqrt\pi}e^{2z^{3/2}/3},\\
\operatorname{Ai}(-w)&\sim\frac{w^{-1/4}}{\sqrt\pi}\sin(2w^{3/2}/3+\pi/4),&\operatorname{Bi}(-w)&\sim\frac{w^{-1/4}}{\sqrt\pi}\cos(2w^{3/2}/3+\pi/4).
\end{aligned}
$$

Match these to the [WKB approximation](../../../../wkb-approximation.md) in an overlap region where the linearization of the [potential energy](../../../../potential-energy.md) and the large-argument [asymptotic expansions](../../../../asymptotic-expansion-split.md) both apply. If $K_t=\hbar^{-1}|\int_{x_t}^x\chi\,dx|$ on the forbidden side and $s_t=\hbar^{-1}|\int_{x_t}^xp\,dx|$ on the allowed side, the [Airy turning-point connection formula](../../../../airy-turning-point-connection-formula.md) is

$$
\boxed{\frac{B}{\sqrt\chi}e^{-K_t}\ \longleftrightarrow\ \frac{2B}{\sqrt p}\sin(s_t+\pi/4),\qquad\frac{A}{\sqrt\chi}e^{K_t}\ \longleftrightarrow\ \frac{A}{\sqrt p}\cos(s_t+\pi/4).}
$$

Thus a decaying exponential acquires a factor two in its allowed-side amplitude, whereas a growing exponential does not. The phase convention uses positive integrals measured away from the [classical turning point](../../../../classical-turning-point.md), so it applies at both ends of the well without an extra orientation sign. These are leading semiclassical matching rules for simple, separated [classical turning points](../../../../classical-turning-point.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the further quantum theory course of the University of Oxford](../../../split.md)
5. [Further quantum theory course of the University of Oxford](../../../../further-quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
