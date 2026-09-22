<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First the common [boundary distance function](../../../../../../boundary-distance-function.md) determines the induced tangential [Riemannian metric](../../../../../../riemannian-metric.md). For a boundary curve $c(t)$ with $c(0)=x$ and $c'(0)=w\in T_x\partial M$, the local first-order distance expansion gives

$$
\lim_{t\to0}\frac{d_{g_i}(x,c(t))}{|t|}=|w|_{g_i}.
$$

For clarity, the upper bound follows from the length of the boundary curve. In a small coordinate neighbourhood the [Riemannian metric](../../../../../../riemannian-metric.md) is arbitrarily close to its value at $x$, so the length of any sufficiently short joining path is bounded below by that constant-metric displacement [norm](../../../../../../norm.md) with an arbitrarily small relative error. A minimizing short path cannot leave that neighbourhood. These two bounds prove the limit. Equality of the [boundary distance functions](../../../../../../boundary-distance-function.md) then gives $|w|_{g_1}=|w|_{g_2}$. The [polarization identity](../../../../../../polarization-identity.md) yields

$$
g_1|_{T\partial M}=g_2|_{T\partial M}=:h.
$$

This alone fixes no choice of normal coordinates, so a boundary-fixing gauge is needed to compare the full tangent-space [Riemannian metrics](../../../../../../riemannian-metric.md).

Let $n_i$ be the inward unit normals and let

$$
C_i(x,r)=\exp_x^{g_i}(r n_i(x))
$$

be sufficiently small [boundary normal coordinates](../../../../../../boundary-normal-coordinates.md). Their pullbacks have the form $C_i^*g_i=dr^2+h_i(r)$, with $h_i(0)=h$. On a collar define $\psi=C_2\circ C_1^{-1}$. It fixes the boundary, has $D\psi(w)=w$ for tangential $w$, and sends $n_1$ to $n_2$. For tangent-space vectors $w+a n_1$ and $z+b n_1$ at the boundary, therefore,

$$
(\psi^*g_2)(w+a n_1,z+b n_1)=h(w,z)+ab
=g_1(w+a n_1,z+b n_1).
$$

This proves the desired full [Riemannian metric](../../../../../../riemannian-metric.md) equality locally at the boundary.

We also justify extending this local identification to a global [diffeomorphism](../../../../../../diffeomorphism.md). Interpolate the positive [Riemannian metrics](../../../../../../riemannian-metric.md) by $g_s=(1-s)g_1+sg_2$, for $0\le s\le1$. Let $C_s$ be their inward unit-normal exponential collars. Compactness of the boundary and parameter interval gives a common small collar width for all $s$. The intermediate [Riemannian metrics](../../../../../../riemannian-metric.md) need not be simple; only these local collars are used.

On the image of $C_s$, define the time-dependent [vector field](../../../../../../vector-field.md)

$$
Y_s(C_s(x,r))=\chi(r)\,\partial_s C_s(x,r),
$$

where $\chi$ is one near zero and vanishes before the outer edge of the collar; extend $Y_s$ by zero elsewhere. This is a smooth [vector field](../../../../../../vector-field.md) on $M$, vanishing at the boundary because $C_s(x,0)=x$. Its time-dependent flow $\Psi_s$ is a global [diffeomorphism](../../../../../../diffeomorphism.md) fixing the boundary. For every sufficiently small fixed $r$, the curve $s\mapsto C_s(x,r)$ solves its equation, since $\chi(r)=1$. Uniqueness gives $\Psi_s(C_0(x,r))=C_s(x,r)$. Consequently $\Psi_1$ agrees near the boundary with $C_2C_1^{-1}$. Taking $\psi=\Psi_1$ proves

$$
\boxed{\psi|_{\partial M}=\mathrm{id},\qquad
\psi^*g_2=g_1\text{ on every }T_xM\ (x\in\partial M)}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
