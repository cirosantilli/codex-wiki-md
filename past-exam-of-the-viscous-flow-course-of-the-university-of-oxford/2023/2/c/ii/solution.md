<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $g=f_1'$. The [boundary value problem](../../../../../boundary-value-problem-split.md) becomes

$$
\boxed{g''+\zeta g'-2g=0,\qquad g'(0)=1,\qquad
g(\zeta)\longrightarrow0\quad(\zeta\to-\infty).}
$$

For $y_1=1+\zeta^2$, direct substitution gives $y_1''+\zeta y_1'-2y_1=2+2\zeta^2-2(1+\zeta^2)=0$. This growing [polynomial](../../../../../polynomial-split.md) solution is useful for [reduction of order](../../../../../reduction-of-order.md).

Write $g=y_1v$. Substitution into the [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation-split.md) cancels the terms proportional to $v$ and gives

$$
y_1v''+(2y_1'+\zeta y_1)v'=0.
$$

An [integrating factor](../../../../../integrating-factor.md) for this first-order equation for $v'$ yields

$$
v'(\zeta)=C\frac{e^{-\zeta^2/2}}{(1+\zeta^2)^2}.
$$

The far-field [boundary condition](../../../../../boundary-condition.md) selects the convergent [integral](../../../../../integral-split.md) from $-\infty$:

$$
g(\zeta)=C(1+\zeta^2)\int_{-\infty}^{\zeta}
\frac{e^{-s^2/2}}{(1+s^2)^2}\,ds.
$$

Any additional multiple of $1+\zeta^2$ would grow at $-\infty$. The chosen expression tends to zero: for $r=-\zeta\geq1$,

$$
0\leq\int_{-\infty}^{\zeta}\frac{e^{-s^2/2}}{(1+s^2)^2}\,ds
=\int_r^\infty\frac{e^{-t^2/2}}{(1+t^2)^2}\,dt
\leq\frac{e^{-r^2/2}}{r(1+r^2)^2}.
$$

Here $(1+t^2)^{-2}\leq(1+r^2)^{-2}$ and $\int_r^\infty e^{-t^2/2}\,dt\leq r^{-1}\int_r^\infty t e^{-t^2/2}\,dt$. Thus the far-field [boundary condition](../../../../../boundary-condition.md) is verified without a cancellation of large terms.

At $\zeta=0$, differentiating gives $g'(0)=C$, so $C=1$. Using the antiderivative supplied in the paper gives the explicit answer

$$
\boxed{g(\zeta)=\frac{\zeta}{2}e^{-\zeta^2/2}
+\frac{\sqrt{2\pi}}4(1+\zeta^2)
\left[1+\operatorname{erf}\!\left(\frac{\zeta}{\sqrt2}\right)\right],
\qquad \zeta\leq0.}
$$

Here $\operatorname{erf}$ is the [error function](../../../../../error-function.md). Finally,

$$
f_1(\zeta)=\int_0^{\zeta}g(s)\,ds
$$

recovers the unique correction satisfying $f_1(0)=0$. The decay bound also shows that $f_1$ approaches a finite constant at $-\infty$, as allowed by the normal [velocity](../../../../../velocity.md) matching. This is the [weak surface-shear perturbation of stagnation flow](../../../../../weak-surface-shear-perturbation-of-stagnation-flow.md).

If the printed $+\infty$ condition is instead imposed literally on a positive half-line, [reduction of order](../../../../../reduction-of-order.md) gives

$$
g_+(\zeta)=-(1+\zeta^2)\int_{\zeta}^{\infty}
\frac{e^{-s^2/2}}{(1+s^2)^2}\,ds,
\qquad g_+(0)=-\frac{\sqrt{2\pi}}4.
$$

It satisfies $g_+'(0)=1$ but grows as $\zeta\to-\infty$, so it cannot describe the fluid domain specified in this paper. This makes the consequence of the printed sign error explicit.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the viscous flow course of the University of Oxford](../../../../split.md)
6. [Viscous flow course of the University of Oxford](../../../../../viscous-flow-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
