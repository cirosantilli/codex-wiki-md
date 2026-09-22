<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $h_{ij}={}^{(3)}g_{ij}$ for the positive spatial [metric tensor](../../../../../../../metric-tensor.md) and $h^{ij}$ for its inverse. Expanding the [3+1 decomposition](../../../../../../../3-plus-1-decomposition-of-spacetime.md) gives $g_{00}=N^2-h_{ij}N^iN^j$, $g_{0i}=-h_{ij}N^j$ and $g_{ij}=-h_{ij}$. The inverse is

$$
\boxed{g^{00}=N^{-2},\qquad g^{0i}=-N^iN^{-2},\qquad
g^{ij}=-h^{ij}+N^iN^jN^{-2}.}
$$

For example, $g^{00}g_{00}+g^{0i}g_{i0}=1$, and $g^{00}g_{0j}+g^{0i}g_{ij}=0$. The spatial block similarly gives $g^{i0}g_{0j}+g^{ik}g_{kj}=\delta^i{}_j$. These checks determine all blocks without treating the spatial block alone as the inverse of the four-metric.

Raising the normal covector with this inverse [metric tensor](../../../../../../../metric-tensor.md) yields

$$
\boxed{n^\mu=(N^{-1},-N^iN^{-1}).}
$$

Take $N>0$ so it is future-pointing. Its norm is $n_\mu n^\mu=1$. The [spatial projection tensor](../../../../../../../spatial-projection-tensor.md) obeys $P^\mu{}_\nu n^\nu=0$, and multiplication gives

$$
P^\mu{}_\alpha P^\alpha{}_\nu
=\delta^\mu{}_\nu-2n^\mu n_\nu+n^\mu(n_\alpha n^\alpha)n_\nu
=\boxed{P^\mu{}_\nu}.
$$

Thus it is an [idempotent](../../../../../../../idempotent.md) [linear projection](../../../../../../../projection-linear-algebra.md) onto vectors tangent to the spatial [hypersurface](../../../../../../../hypersurface.md). The negative spatial components of the spacetime [metric tensor](../../../../../../../metric-tensor.md) do not change this idempotence.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 53](../../../../paper-53-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
