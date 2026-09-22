<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $h_{ij}$ for the spatial [metric tensor](../../../../../../../metric-tensor.md) and lower the [shift vector](../../../../../../../shift-vector.md) with $h_{ij}$. For the negative-shift convention, the four-dimensional metric and its inverse have components

$$
g_{00}=-N^2+N_iN^i,\quad g_{0i}=-N_i,\quad g_{ij}=h_{ij},\qquad g^{00}=-N^{-2},\quad g^{0i}=-N^iN^{-2}.
$$

The normal has covariant components $n_\mu=(-N,0,0,0)$, so $n_\mu n^\mu=-1$ and it annihilates every tangent vector to the spatial slice. Since $n_i=0$, its [covariant derivative](../../../../../../../covariant-derivative.md) gives $n_{i;j}=N\Gamma^0{}_{ij}$ and therefore $K_{ij}=-N\Gamma^0{}_{ij}$.

Compute the required [Christoffel symbol](../../../../../../../christoffel-symbol.md) using the symmetric connection formula. Its time-index term and spatial-index term combine to give

$$
\Gamma^0{}_{ij}=\frac{1}{2N^2}\left(\dot h_{ij}+\partial_iN_j+\partial_jN_i-N^k(\partial_i h_{jk}+\partial_jh_{ik}-\partial_kh_{ij})\right).
$$

The spatial expression in parentheses is $\dot h_{ij}+D_iN_j+D_jN_i$, where $D$ is the [covariant derivative](../../../../../../../covariant-derivative.md) of $h$. Thus the [extrinsic curvature with a negative shift](../../../../../../../extrinsic-curvature-with-a-negative-shift.md) is

$$
\boxed{K_{ij}=-\frac{1}{2N}(\dot h_{ij}+D_iN_j+D_jN_i).}
$$

This derivation fixes both signs from the actual [3+1 decomposition of spacetime](../../../../../../../3-plus-1-decomposition-of-spacetime.md), rather than transferring a formula using the opposite [shift vector](../../../../../../../shift-vector.md) convention. The connection formula used here has $g_{\lambda\kappa,\nu}$ as its second differentiated term; the printed repeated-index version is a typographical error.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 312](../../../../paper-312-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
