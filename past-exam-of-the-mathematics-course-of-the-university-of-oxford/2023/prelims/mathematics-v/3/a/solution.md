<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\Sigma$ be a piecewise smooth oriented [surface](../../../../../../topological-surface-split.md), and let $\mathbf F$ be continuously differentiable on an open neighbourhood of it. [Stokes theorem](../../../../../../stokes-theorem.md) states that

$$
\boxed{\oint_{\partial\Sigma}\mathbf F\cdot d\mathbf r
=\iint_\Sigma(\nabla\times\mathbf F)\cdot\mathbf n\,dS.}
$$

The [boundary orientation](../../../../../../boundary-orientation.md) is induced by the chosen [unit normal vector](../../../../../../unit-normal.md) through the [right-hand rule](../../../../../../right-hand-rule.md). Smoothness on a neighbourhood makes the spatial [partial derivatives](../../../../../../partial-derivative.md) in the [curl](../../../../../../curl.md) well defined.

Choose the outward [orientation of a surface](../../../../../../orientation-of-a-surface.md) on the lower half of the [ellipsoid](../../../../../../ellipsoid.md). At its lowest point the normal points down, so its boundary ellipse is traversed clockwise when viewed from above. Use

$$
\mathbf r(t)=(2\cos t,-3\sin t,0),\qquad0\leq t\leq2\pi.
$$

The [line integral](../../../../../../line-integral.md) is

$$
\begin{aligned}
\oint_{\partial\Sigma}\mathbf F\cdot d\mathbf r
&=\int_0^{2\pi}\bigl[(-6\sin t)(-2\sin t)+(6\cos t)(-3\cos t)\bigr]dt\\
&=12\pi-18\pi=\boxed{-6\pi}.
\end{aligned}
$$

For an independent [surface integral](../../../../../../surface-integral.md) calculation, first compute $\nabla\times\mathbf F=(2y,-2x,1)$. Parametrize the lower half by

$$
\mathbf R(u,v)=(2\sin u\cos v,3\sin u\sin v,-3\sqrt3\cos u),
\quad0\leq u\leq\frac\pi2,\quad0\leq v\leq2\pi.
$$

The outward vector [area element](../../../../../../area-element-of-a-surface.md) is

$$
\mathbf n\,dS=(\mathbf R_v\times\mathbf R_u)\,du\,dv
=\bigl(9\sqrt3\sin^2u\cos v,6\sqrt3\sin^2u\sin v,-6\sin u\cos u\bigr)\,du\,dv.
$$

Thus

$$
\begin{aligned}
\iint_\Sigma(\nabla\times\mathbf F)\cdot\mathbf n\,dS
&=\int_0^{\pi/2}\int_0^{2\pi}
\bigl(30\sqrt3\sin^3u\sin v\cos v-6\sin u\cos u\bigr)\,dv\,du\\
&=-12\pi\int_0^{\pi/2}\sin u\cos u\,du
=\boxed{-6\pi}.
\end{aligned}
$$

The two sides agree. Choosing the inward [unit normal vector](../../../../../../unit-normal.md) and its corresponding counterclockwise [boundary orientation](../../../../../../boundary-orientation.md) changes both answers to $6\pi$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
