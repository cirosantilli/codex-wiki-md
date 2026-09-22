<h1 id="b/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Long-wave geometry makes vertical acceleration small, so [pressure](../../../../pressure-split.md) is approximately hydrostatic, $p=p_{\rm atm}+\rho g(h-z)$. The leading horizontal [velocity](../../../../velocity.md) is nearly depth-independent. Integrating [incompressibility](../../../../incompressible-flow.md) through the depth and using the impermeable bed and kinematic free-surface condition gives $\boxed{h_t+(hu)_x=0}$. The horizontal [Euler equation](../../../../euler-equations-for-an-inviscid-fluid-split.md) then gives $\boxed{u_t+uu_x+gh_x=0}$.

Linearizing about a uniform resting layer gives wave speed $\boxed{c=\sqrt{gh}}$. Since $h=c^2/g$, the nonlinear equations can be written $c_t+uc_x+(c/2)u_x=0$ and $u_t+uu_x+2cc_x=0$. Combining them verifies

$$
\boxed{[\partial_t+(u\pm c)\partial_x](u\pm2c)=0.}
$$

Let $c_0=\sqrt{gh_0}$ and $V\geq0$ be the receding wall's speed, so its position is $x=-Vt$ and its fluid [velocity](../../../../velocity.md) condition is $u=-V$. The outward-moving rarefaction has the other invariant fixed at its resting value, $u-2c=-2c_0$. In its varying part, [self-similarity](../../../../self-similarity.md) gives $x/t=u+c$. Therefore

$$
\boxed{c=\frac{x/t+2c_0}{3},\qquad u=\frac23(x/t-c_0).}
$$

The wall-adjacent state has $u=-V$ and $c=c_w=c_0-V/2$. Its right-going [characteristic curve](../../../../characteristic-curve.md) speed is $c_0-3V/2$, whereas the undisturbed head travels at $c_0$. The complete solution in the fluid $x>-Vt$ is

$$
\boxed{(u,c)=\begin{cases}
(-V,c_0-V/2),&-V<x/t<c_0-3V/2,\\
(\tfrac23(x/t-c_0),\tfrac13(x/t+2c_0)),&c_0-3V/2\leq x/t\leq c_0,\\
(0,c_0),&x/t>c_0.
\end{cases}}
$$

Both edges match continuously and the wall [velocity](../../../../velocity.md) condition holds. The assumption $V^2<4gh_0$ means $V<2c_0$, giving positive wall depth and placing the fan tail to the right of the wall by speed $c_w>0$. The depth everywhere is $h=c^2/g$. This is a [shallow-water rarefaction from a receding wall](../../../../shallow-water-rarefaction-from-a-receding-wall.md).

## ↑ Ancestors (12)

1. [7](../7.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the theoretical mechanics course of the University of Oxford](../../../split.md)
5. [Theoretical mechanics course of the University of Oxford](../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
