<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a timelike tangent $v=dx/du$, put $L=\sqrt{-g(v,v)}>0$ and $\mathscr L=L^2/2=-g(v,v)/2$, and use the [Euler-Lagrange equations](../../../../../../euler-lagrange-equation.md). For the quadratic [geodesic Lagrangian](../../../../../../geodesic-lagrangian.md), they reduce to

$$
\frac d{du}(g_{\mu\nu}v^\nu)-\frac12\partial_\mu g_{\alpha\beta}v^\alpha v^\beta=0,
\qquad \nabla_vv=0.
$$

Here the first equation has been multiplied by an irrelevant minus sign. For the length Lagrangian, its derivatives are $L^{-1}$ times those of $\mathscr L$, and differentiating that factor yields instead

$$
\boxed{\nabla_vv=\frac{\dot L}{L}\,v.}
$$

This is the [unparametrized geodesic equation](../../../../../../unparametrized-geodesic-equation.md), the key to why [timelike length and energy have the same geodesic images](../../../../../../timelike-length-and-energy-have-the-same-geodesic-images.md). Define [proper time](../../../../../../proper-time.md) locally by $d\tau/du=L>0$ and put $w=dx/d\tau=v/L$. The product rule then gives $\nabla_ww=L^{-2}[\nabla_vv-(\dot L/L)v]=0$ and $g(w,w)=-1$. Conversely an affinely parametrized timelike [geodesic](../../../../../../geodesic.md) has constant $L$, by [metric compatibility](../../../../../../metric-compatibility.md), and therefore satisfies both equations.

Thus **the two variational problems have the same oriented timelike geodesic images, after reparametrization**. They do not have exactly the same parametrized solutions with an arbitrary fixed $u$: in [Minkowski spacetime](../../../../../../minkowski-spacetime.md), $t(u)=u^2$, $\mathbf x=0$, $u>0$, satisfies the length equation but not the quadratic equation. The timelike assumption excludes $L=0$, where this argument and the length derivative would fail.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
