<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Gauss lemma](../../../../../../gauss-s-lemma-riemannian-geometry.md) says that, for $v,w\in T_pM$ for which the [exponential map](../../../../../../exponential-map-riemannian-geometry.md) is defined,

$$
\boxed{\left\langle(d\exp_p)_v v,(d\exp_p)_v w\right\rangle_{\exp_p(v)}=\langle v,w\rangle_p.}
$$

In particular radial and angular directions are orthogonal, and the radial direction retains its length.

Take the variation through [geodesics](../../../../../../geodesic.md) $\alpha(t,s)=\exp_p(t(v+sw))$, and put $T=\partial_t\alpha$, $J=\partial_s\alpha$. The [Levi-Civita connection](../../../../../../levi-civita-connection.md) is metric compatible and [torsion-free](../../../../../../torsion-free-connection.md), so $\nabla_tJ=\nabla_sT$. Each $t$-curve is a [geodesic](../../../../../../geodesic.md), hence $\nabla_tT=0$, and its constant squared speed is $|v+sw|_p^2$. Therefore

$$
\frac{d}{dt}\langle T,J\rangle
=\langle T,\nabla_tJ\rangle
=\langle T,\nabla_sT\rangle
=\frac12\partial_s|T|^2
=\langle v+sw,w\rangle_p.
$$

At $t=0$ the variation starts at the fixed point $p$, so $J(0,s)=0$. Integrating from $0$ to $1$ and setting $s=0$ gives the displayed identity, because $T(1,0)=(d\exp_p)_v v$ and $J(1,0)=(d\exp_p)_v w$.

In [geodesic normal coordinates](../../../../../../geodesic-normal-coordinates.md) based on an [orthonormal basis](../../../../../../orthonormal-basis.md) at $p$, choose $v=x$ and $w$ to be the $j$th coordinate vector. The lemma gives

$$
g_{ij}(x)x^i=x_j,\qquad\boxed{g^{ij}(x)x_i=x_j}.
$$

These identities also hold at $x=0$ by continuity. They are the radial identities required in part (b).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
