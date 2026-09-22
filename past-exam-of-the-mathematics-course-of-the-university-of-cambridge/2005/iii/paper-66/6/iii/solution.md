<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let the point light be at $L$. For a [subdivision curve](../../../../../../subdivision-curve.md) point $C(t)$, its projected shadow lies on the ray beyond the [subdivision curve](../../../../../../subdivision-curve.md):

$$
R_t(\lambda)=L+\lambda(C(t)-L),\qquad\lambda>1.
$$

The shadow is the first intersection of that ray with the receiving [subdivision surface](../../../../../../subdivision-surface.md) after the [subdivision curve](../../../../../../subdivision-curve.md) point. Thus solve

$$
F(u,v,\lambda;t)=S(u,v)-L-\lambda(C(t)-L)=0
$$

and retain the smallest admissible $\lambda$. This is the defining equation for [shadow tracing for a subdivision curve](../../../../../../shadow-tracing-for-a-subdivision-curve.md).

First organize the [subdivision surface](../../../../../../subdivision-surface.md) patches into a [bounding volume hierarchy](../../../../../../bounding-volume-hierarchy.md). For a restricted [subdivision curve](../../../../../../subdivision-curve.md) interval, rays through its enclosing volume define an enclosing ray cone from $L$; [subdivision surface](../../../../../../subdivision-surface.md) bounds that do not meet this cone can be rejected. Refine surviving [subdivision curve](../../../../../../subdivision-curve.md) intervals and [subdivision surface](../../../../../../subdivision-surface.md) patches. For a fixed $t$, isolate all possible ray intersections using those bounds, then correct each regular candidate with the [Jacobian matrix](../../../../../../jacobian-matrix.md) for the [Newton method](../../../../../../newton-s-method-in-optimization.md)

$$
J=[S_u,S_v,-(C(t)-L)].
$$

The [scalar triple product](../../../../../../scalar-triple-product.md) shows that $J$ is invertible exactly when $n\cdot(C(t)-L)\ne0$. Enforce the patch domain and $\lambda>1$ throughout correction, and choose the smallest valid $\lambda$. Bounds or validated root isolation, rather than a fixed list of [subdivision curve](../../../../../../subdivision-curve.md) samples, are needed if every shadow component is to be found.

Once a regular intersection is known, follow it as $t$ changes. Differentiating $F=0$ gives a useful predictor:

$$
\boxed{J\begin{pmatrix}u'\\v'\\\lambda'\end{pmatrix}=\lambda C'(t),\qquad Q'(t)=S_u\,u'+S_v\,v'=\lambda C'(t)+\lambda'(C(t)-L).}
$$

Take a small predictor step in $(u,v,\lambda)$ and apply a [Newton method](../../../../../../newton-s-method-in-optimization.md) correction at the new [subdivision curve](../../../../../../subdivision-curve.md) parameter. Move through patch adjacency with its chart transition; shrink steps when [derivatives](../../../../../../derivative.md) or error estimates change rapidly. Subdivide further and test a geometric curve-to-chord bound to approximate the resulting shadow trace to a chosen tolerance.

Surface-boundary crossings terminate or clip a trace. If a ray has no admissible [subdivision surface](../../../../../../subdivision-surface.md) intersection, that [subdivision curve](../../../../../../subdivision-curve.md) parameter contributes no shadow on $S$. At grazing contact the Jacobian is singular, so use interval subdivision and root isolation to detect the event and seed any outgoing branches. If several intersections are possible, recheck which is first; facing the light locally is helpful but is not a proof of global uniqueness. Open-curve endpoints and closed-curve seams must also be accounted for. With a compact represented geometry, transversal intersections and validated subdivision bounds, this algorithm traces every visible component; a purely sampled implementation gives only a tolerance-dependent approximation and cannot certify arbitrary tiny missed components.

For a directional light, replace the ray by $C(t)+\lambda d$ for a fixed propagation vector $d$ and $\lambda>0$. The intersection equation becomes $S-C-\lambda d=0$, with Jacobian $[S_u,S_v,-d]$ and continuation right-hand side $C'(t)$. The same enquiries and event handling apply.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
