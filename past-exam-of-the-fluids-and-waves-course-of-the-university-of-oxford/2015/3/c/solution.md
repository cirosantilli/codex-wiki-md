<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The fixed upper and lower walls have zero normal [velocity](../../../../velocity.md). Since $v=\phi_y$, their [no-penetration boundary conditions](../../../../no-penetration-boundary-condition.md) are

$$
\boxed{\phi_y=0\quad\text{at }y=0,H.}
$$

For the moving end wall, use its level-set equation $F(x,y,t)=x-X(y,t)=0$. The [kinematic boundary condition](../../../../kinematic-boundary-condition.md) $DF/Dt=0$ gives the exact impermeability relation

$$
u=X_t+vX_y\quad\text{at }x=X(y,t).
$$

Both $v$ and $X_y$ are first order, so their product is second order. A [Taylor expansion](../../../../taylor-expansion.md) from $x=X$ to $x=0$ changes the first-order perturbation [velocity](../../../../velocity.md) only at second order as well. Thus

$$
\boxed{\phi_x(0,y,t)=X_t(y,t)=\epsilon\omega\cos(\omega t)\cos\frac{\pi y}H.}
$$

At infinity, select a bounded response with **no waves incident from $x=+\infty$**. A propagating [acoustic waveguide mode](../../../../acoustic-waveguide-mode.md) must satisfy the outgoing [radiation condition for a waveguide mode](../../../../radiation-condition-for-a-waveguide-mode.md), while a nonpropagating mode must decay. For a time dependence $e^{-i\omega t}$, a propagating axial factor has the form $e^{iqx}$, $q>0$, and obeys $\Phi_x-iq\Phi\to0$. An evanescent factor is $e^{-\alpha x}$, $\alpha>0$.

Requiring $\phi\to0$ for all frequencies would incorrectly exclude the radiated traveling waves. In this lossless channel they retain finite [amplitude](../../../../wave-amplitude.md) arbitrarily far downstream.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the fluids and waves course of the University of Oxford](../../../split.md)
5. [Fluids and waves course of the University of Oxford](../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
