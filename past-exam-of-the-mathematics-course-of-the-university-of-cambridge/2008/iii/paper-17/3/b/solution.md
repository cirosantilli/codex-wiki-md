<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First recover the induced boundary metric from the [boundary distance function](../../../../../../boundary-distance-function.md). If $c(t)$ is a smooth boundary curve with $c(0)=x$ and $\dot c(0)=w\in T_x\partial M$, the local metric expansion of distance gives

$$
\lim_{t\to0}\frac{d_{g_i}(x,c(t))^2}{t^2}=g_i(w,w).
$$

One can obtain this expansion in local coordinates from the fact that the metric tends uniformly to its value at $x$; distances to nearby points have that constant metric's first-order norm. Equality of the two [boundary distance functions](../../../../../../boundary-distance-function.md) makes the two quadratic values equal for every boundary-tangent $w$. Polarization therefore recovers the full bilinear induced metric:

$$
h=g_1|_{T\partial M}=g_2|_{T\partial M}.
$$

This does not yet identify the metrics on normal vectors or mixed tangent-normal pairs.

Let $\nu_i$ be the inward unit normal for $g_i$. The [boundary normal coordinates](../../../../../../boundary-normal-coordinates.md)

$$
c_i(x,r)=\exp_x^{g_i}(r\nu_i(x)),\qquad 0\le r<\varepsilon,
$$

are [collar neighborhoods](../../../../../../collar-neighbourhood.md) for a common sufficiently small $\varepsilon$. The [Gauss lemma](../../../../../../gauss-s-lemma-riemannian-geometry.md) gives $c_i^*g_i=dr^2+h_i(r)$ with $h_i(0)=h$. Hence the local boundary-fixing map $c_2\circ c_1^{-1}$ already satisfies

$$
g_1=(c_2\circ c_1^{-1})^*g_2\quad\text{on }TM|_{\partial M},
$$

because both pulled-back metrics there are $dr^2+h$.

To justify a global [diffeomorphism](../../../../../../diffeomorphism.md), rather than assume a local collar map extends, interpolate the positive metrics by $g_s=(1-s)g_1+sg_2$, $0\le s\le1$. Their inward unit normals and exponential maps give smoothly varying collars

$$
C_s(x,r)=\exp_x^{g_s}(r\nu_s(x)).
$$

Compactness of $[0,1]\times\partial M$ gives a uniform collar size after shrinking $\varepsilon$. On the image of each collar define the time-dependent [vector field](../../../../../../vector-field.md)

$$
Z_s(C_s(x,r))=\partial_s C_s(x,r).
$$

Multiply it by a smooth cutoff which is one for small $r$ and zero before the collar's outer edge, and extend it by zero to the rest of $M$. This gives a smooth global time-dependent [vector field](../../../../../../vector-field.md). It vanishes on the boundary, because $C_s(x,0)=x$ for all $s$. Its flow $\Psi_s$ exists for the full interval and fixes the boundary. For sufficiently small fixed $r$, the curve $s\mapsto C_s(x,r)$ solves this flow equation, so uniqueness gives

$$
\Psi_s(c_1(x,r))=C_s(x,r).
$$

Here $C_0=c_1$ and $C_1=c_2$. Thus the final map $\psi=\Psi_1$ agrees with the local map from the $g_1$ collar to the $g_2$ collar near the boundary. In particular $D\psi$ fixes tangential vectors and sends $\nu_1$ to $\nu_2$ there. Since the tangent-normal splittings are orthogonal and the normals have unit length,

$$
\boxed{\psi|_{\partial M}=\operatorname{id},\qquad g_1=\psi^*g_2\text{ on }TM|_{\partial M}.}
$$

The construction only needs equality of the induced boundary metrics; the equal-distance hypothesis supplies that equality.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
