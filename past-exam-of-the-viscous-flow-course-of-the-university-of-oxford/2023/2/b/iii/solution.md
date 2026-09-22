<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

With $u=xf'(\zeta)$ and $W=-f(\zeta)$, [incompressibility](../../../../../incompressible-flow.md) is automatic because $u_x=f'$ and $W_\zeta=-f'$. In the streamwise [boundary-layer equation](../../../../../boundary-layer-equation.md),

$$
u u_x+W u_\zeta=x(f')^2-xff'',\qquad
u_{\zeta\zeta}=xf'''.
$$

Equating coefficients of $x$ gives

$$
(f')^2-ff''=1+f''',\qquad
\boxed{f'''+ff''+1-(f')^2=0.}
$$

This coefficient comparison determines the equation even though the streamwise equation vanishes identically at the [stagnation point](../../../../../stagnation-point.md) $x=0$.

The [no-penetration boundary condition](../../../../../no-penetration-boundary-condition.md) gives $f(0)=0$, the surface [shear stress](../../../../../shear-stress.md) gives $xf''(0)=\gamma x$, and matching the tangential [velocity](../../../../../velocity.md) to the [outer solution](../../../../../outer-expansion.md) gives $f'\to1$. Thus

$$
\boxed{f(0)=0,\qquad f''(0)=\gamma,\qquad
f'(\zeta)\longrightarrow1\quad(\zeta\to-\infty).}
$$

If the correction $f'-1$ is integrable at the far end, then $f=\zeta+O(1)$ there, which is consistent with $W\sim-\zeta$. The small-[shear stress](../../../../../shear-stress.md) solution below has precisely this property.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
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
