<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Linearize about fluid at rest, with mean [free surface](../../../../../free-surface.md) $y=0$ and mean bottom $y=-d$. Regard $a$, $\eta$ and the perturbation [velocity potential](../../../../../velocity-potential.md) as first-order quantities. A [Taylor expansion](../../../../../taylor-expansion.md) from $y=\eta$ to $y=0$ produces products of first-order quantities, as do $\phi_x\eta_x$ and $|\nabla\phi|^2$. Discarding these second-order terms gives the [linearized free-surface boundary conditions](../../../../../linearized-free-surface-boundary-conditions.md)

$$
\boxed{\phi_y=\eta_t,\qquad\phi_t+g\eta=0\quad(y=0).}
$$

Equivalently, differentiate the second condition in time and substitute the first to obtain $\phi_{tt}+g\phi_y=0$ at $y=0$.

The bottom is also impermeable and moving. Its exact [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) follows from $D(y-h)/Dt=0$:

$$
\phi_y=h_t+\phi_xh_x\quad(y=h).
$$

Here $h_t=-akc\cos(k(x-ct))$, while $\phi_xh_x$ and the change from evaluating $\phi_y$ at $h$ to evaluating it at $-d$ are second order. Hence

$$
\boxed{\phi_y(x,-d,t)=-akc\cos(k(x-ct)).}
$$

The interior [Laplace equation](../../../../../laplace-equation.md) remains $\phi_{xx}+\phi_{yy}=0$ on $-d<y<0$. This [linearization](../../../../../linearization.md) requires small slopes and small resulting excursions as well as $a\ll d$; close to [resonance](../../../../../resonance.md) a small prescribed bottom displacement can produce a response too large for it.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
