<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [tensor-product surface basis](../../../../../tensor-product-surface-basis.md) is formed from two independent univariate basis families $\phi_i(u)$ and $\psi_j(v)$ on separate parameter intervals. Given a rectangular [control net](../../../../../control-net.md) $p_{ij}$, its [parametric surface](../../../../../parametric-surface.md) is

$$
\boxed{S(u,v)=\sum_i\sum_jp_{ij}\phi_i(u)\psi_j(v).}
$$

The parameters and indices vary independently over a product domain. The representation can be evaluated first in either parameter, giving a convenient computational advantage. Assume a finite basis, or locally finite [spline](../../../../../spline-mathematics.md) bases, so differentiation and summation below are justified locally.

For positivity, if each factor basis is nonnegative, then $\phi_i(u)\psi_j(v)\ge0$. If both factors are strictly positive at a point, their product is strictly positive there. Nonnegative weights are the usual geometric meaning of positivity; zero boundary weights are allowed. With [partition of unity](../../../../../partition-of-unity.md), this gives the local [convex hull](../../../../../convex-hull.md) enclosure of the active [control points](../../../../../control-point.md).

For continuity, suppose the first family is $C^r$ and the second $C^s$, including matching derivatives across their respective [spline knots](../../../../../spline-knot.md). On every polynomial piece, and by matching at the knot lines,

$$
\partial_u^p\partial_v^qS(u,v)
=\sum_{i,j}p_{ij}\phi_i^{(p)}(u)\psi_j^{(q)}(v),
\qquad 0\le p\le r,\quad0\le q\le s.
$$

Every factor on the right is continuous in its own variable, so its product is jointly continuous. Thus **all these mixed derivatives are continuous**, in particular the surface is jointly $C^{\min(r,s)}$. The separate coordinate smoothness can be better: $r$ orders in $u$ and $s$ in $v$. For piecewise polynomials of degrees $d_u,d_v$, an interior knot of multiplicity $k$ in the first factor normally gives $C^{d_u-k}$ matching in $u$, inherited along that knot line; similarly for $v$. The statement is an inherited lower bound. Special [control points](../../../../../control-point.md) can cancel derivative jumps, so a particular surface may be smoother than a generic member of its basis.

For summation to unity, independent summation factors exactly:

$$
\boxed{\sum_{i,j}\phi_i(u)\psi_j(v)
=\left(\sum_i\phi_i(u)\right)\left(\sum_j\psi_j(v)\right)=1.}
$$

This also explains why translations of all [control points](../../../../../control-point.md) translate the surface by the same vector, as in [affine equivariance of a geometric basis](../../../../../affine-equivariance-of-a-geometric-basis.md). These three arguments establish [tensor-product inheritance of geometric basis properties](../../../../../tensor-product-inheritance-of-geometric-basis-properties.md) directly from the factor identities.

A [triangular Bézier patch](../../../../../triangular-bezier-patch.md) is a non-tensor-product example. For barycentric parameters $u,v,w\ge0$ with $u+v+w=1$, a quadratic patch is

$$
S=u^2p_{200}+v^2p_{020}+w^2p_{002}
+2uvp_{110}+2uwp_{101}+2vwp_{011}.
$$

The six basis functions have total degree two and sum to $(u+v+w)^2=1$. Their index constraint and triangular parameter domain do not arise from two independently indexed univariate factors on a rectangle. An individual triangular polynomial could be embedded in another larger representation, but this triangular basis and [control net](../../../../../control-net.md) are not a tensor-product surface definition.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
