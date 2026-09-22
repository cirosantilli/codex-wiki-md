<h1 id="4/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [method of multiple scales](../../../../../../../method-of-multiple-scales.md), $T=\varepsilon t$, and write $x_0=A(T)\cos\psi$, $\psi=t+\theta(T)$. At first order,

$$
(\partial_t^2+1)x_1=2A_T\sin\psi+2A\theta_T\cos\psi+A f(A\cos\psi)\sin\psi.
$$

Removing the fundamental [secular terms](../../../../../../../secular-term.md) gives the [averaged amplitude for position-dependent damping](../../../../../../../averaged-amplitude-for-position-dependent-damping.md):

$$
A_T=-A\langle f(A\cos\psi)\sin^2\psi\rangle,\qquad \theta_T=0,
$$

where the brackets mean a full-period average. The [initial conditions](../../../../../../../initial-condition.md) set $A(0)=1$ and $\theta(0)=0$ at leading order. For quadratic damping, $\langle\sin^2\psi\rangle=1/2$ and $\langle\cos^2\psi\sin^2\psi\rangle=1/8$, giving

$$
A_T=\frac A2-\frac{A^3}{8},\qquad A(T)=\frac2{\sqrt{1+3e^{-T}}}.
$$

Thus the [Van der Pol amplitude evolution](../../../../../../../van-der-pol-amplitude-evolution.md) yields

$$
\boxed{x(t;\varepsilon)=\frac{2\cos t}{\sqrt{1+3e^{-\varepsilon t}}}+O(\varepsilon),\qquad 0\leq t\leq C/\varepsilon.}
$$

The leading amplitude approaches the stable value two. The small initial-velocity discrepancy introduced by the slow amplitude derivative is removed by the first-order correction and does not affect this leading approximation.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 79](../../../../paper-79-split.md)
5. [Iii](../../../../split.md)
6. [2005](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
