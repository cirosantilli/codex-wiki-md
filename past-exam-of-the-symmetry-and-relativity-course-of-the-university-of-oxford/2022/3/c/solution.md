<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $v=|\mathbf v|>0$, decompose the [velocity](../../../../velocity.md) as $\mathbf u=\mathbf u_\parallel+\mathbf u_\perp$, parallel and perpendicular to $\mathbf v$. A rotation-free [Lorentz boost](../../../../lorentz-boost.md) gives the [velocity-addition formula](../../../../velocity-addition-formula.md)

$$
\mathbf w_\parallel=\frac{\mathbf u_\parallel-\mathbf v}{D},\qquad
\mathbf w_\perp=\frac{\mathbf u_\perp}{\gamma_vD},\qquad
D=1-\mathbf v\cdot\mathbf u/c^2.
$$

These two components are orthogonal, so

$$
\begin{aligned}
D^2|\mathbf w|^2
&=|\mathbf u_\parallel-\mathbf v|^2+(1-v^2/c^2)|\mathbf u_\perp|^2\\
&=|\mathbf u-\mathbf v|^2-\frac{v^2|\mathbf u_\perp|^2}{c^2}\\
&=|\mathbf u-\mathbf v|^2-\frac{|\mathbf v\times\mathbf u|^2}{c^2}.
\end{aligned}
$$

The last equality is [Lagrange's identity](../../../../lagrange-identity-for-the-cross-product.md) for the [cross product](../../../../cross-product.md). For physical [subluminal speeds](../../../../subluminal-speed.md), $D>0$, giving

$$
\boxed{|\mathbf w|=\frac{\sqrt{(\mathbf v-\mathbf u)\cdot(\mathbf v-\mathbf u)-|\mathbf v\times\mathbf u|^2/c^2}}{1-\mathbf v\cdot\mathbf u/c^2}.}
$$

The $\mathbf v=0$ case follows directly or by continuity. An independent form useful for checks is $1-|\mathbf w|^2/c^2=(1-u^2/c^2)(1-v^2/c^2)/D^2$, obtained from the transformed [four-velocity](../../../../four-velocity.md) normalization.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the symmetry and relativity course of the University of Oxford](../../../split.md)
5. [Symmetry and relativity course of the University of Oxford](../../../../symmetry-and-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
