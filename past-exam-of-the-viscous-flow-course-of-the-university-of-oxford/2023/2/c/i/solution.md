<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

At zero surface [shear stress](../../../../../shear-stress.md), the solution connected to part (a) is

$$
\boxed{f_0(\zeta)=\zeta.}
$$

Indeed, it has $f_0'=1$, $f_0''=f_0'''=0$ and $f_0(0)=0$. Insert the [regular perturbation](../../../../../regular-perturbation.md) $f=\zeta+\gamma f_1+O(\gamma^2)$ into the nonlinear [ordinary differential equation](../../../../../ordinary-differential-equation.md). The terms are

$$
f'''=\gamma f_1'''+O(\gamma^2),\qquad
ff''=\gamma\zeta f_1''+O(\gamma^2),\qquad
1-(f')^2=-2\gamma f_1'+O(\gamma^2).
$$

The coefficient of $\gamma$ therefore gives

$$
\boxed{f_1'''+\zeta f_1''-2f_1'=0.}
$$

Expanding the surface [boundary conditions](../../../../../boundary-condition.md) and the far-field matching condition gives

$$
\boxed{f_1(0)=0,\qquad f_1''(0)=1,\qquad
f_1'(\zeta)\longrightarrow0\quad(\zeta\to-\infty).}
$$

**The printed $+\infty$ limit is a sign error.** It is present in the native PDF on paper page 3, not introduced by transcription. The fluid occupies $z<0$, the [inner variable](../../../../../inner-variable.md) is $\zeta=z/\delta<0$, and part (b)(iii) correctly matches at $-\infty$. We retain that physical domain throughout. A change to the positive coordinate $\eta=-\zeta$ would also change the differential equation and surface [derivative](../../../../../derivative.md) signs; it cannot be made by changing only the far-field sign.

The inequality $\delta^2\ll\gamma$ ensures that effects discarded at order $\delta^2$ in the [boundary-layer scaling](../../../../../boundary-layer-scaling.md) are smaller than the retained order-$\gamma$ perturbation. The inequality $\gamma\ll1$ justifies this [regular perturbation](../../../../../regular-perturbation.md). The two conditions control different approximations.

## ↑ Ancestors (13)

1. [I](../i.md)
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
