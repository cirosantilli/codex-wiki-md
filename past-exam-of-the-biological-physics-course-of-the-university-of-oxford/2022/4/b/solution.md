<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $v>0$ and the displayed [potential energy](../../../../potential-energy.md) to be the position-dependent mechanical [free energy](../../../../thermodynamic-free-energy.md) $G(x)$ of a bound motor. On the descending ramp $G'= -G_0/x_1$, and on the ascending ramp $G'=G_0/(P-x_1)$. Thus the [force](../../../../force-split.md) conditional on being bound is

$$
\boxed{F_{\rm bound}(x)=-G'(x)=\begin{cases}
G_0/x_1,&0<x<x_1,\\
-G_0/(P-x_1),&x_1<x<P.
\end{cases}}
$$

It is periodic, piecewise constant and undefined at idealized sharp corners; the corners have zero measure in averages. An unbound motor has zero [force](../../../../force-split.md).

A cohort transported through position $x$ obeys $d/dt=v\,d/dx$. Its bound [probability](../../../../probability.md) therefore satisfies

$$
vB'=k_1(1-B)-k_2B\quad(0<x<x_1),\qquad
vB'=-k_2B\quad(x_1<x<P).
$$

Define $B_0=k_1/(k_1+k_2)$, $\alpha=(k_1+k_2)/v$, $\beta=k_2/v$, $a=e^{-\alpha x_1}$ and $q=e^{-\beta(P-x_1)}$. The exact periodic [steady state](../../../../steady-state.md) includes a small carry-over $b_{\rm in}=B(0)=B(P)$:

$$
b_{\rm in}=\frac{qB_0(1-a)}{1-aq},\qquad
B(x)=\begin{cases}
B_0+(b_{\rm in}-B_0)e^{-\alpha x},&0<x<x_1,\\
\displaystyle\frac{B_0(1-a)}{1-aq}e^{-\beta(x-x_1)},&x_1<x<P.
\end{cases}
$$

These expressions follow by solving each first-order [ordinary differential equation](../../../../ordinary-differential-equation.md), requiring continuity at $x_1$, and imposing periodicity.

The stipulated $v\ll k_2(P-x_1)$ implies $q\ll1$, so the incoming bound fraction is exponentially small. Dropping it gives the simpler intended forms

$$
\boxed{B(x)\simeq\begin{cases}
B_0(1-e^{-\alpha x}),&0<x<x_1,\\
B_0(1-e^{-\alpha x_1})e^{-\beta(x-x_1)},&x_1<x<P.
\end{cases}}
$$

The occupancy rises towards $B_0$ on the binding interval, then decays over length $v/k_2$ outside it. The mean [force](../../../../force-split.md) per member of the full ensemble at a given position is $B(x)F_{\rm bound}(x)$, distinct from the [force](../../../../force-split.md) per bound motor. The right panels of [c](../../1/c.md) show both the occupancy and the conditional [force](../../../../force-split.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
