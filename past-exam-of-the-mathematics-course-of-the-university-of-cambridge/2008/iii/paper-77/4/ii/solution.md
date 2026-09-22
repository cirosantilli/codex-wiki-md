<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a regular [parametric surface](../../../../../../parametric-surface.md) $P(u,v)$, form $N=P_u\times P_v$, $n=N/\lVert N\rVert$ and define the offset evaluator

$$
\boxed{P_d(u,v)=P(u,v)+d\,n(u,v).}
$$

It is already a [parametric surface](../../../../../../parametric-surface.md) with the same parameter domain, even if its coordinates no longer belong to the original polynomial or rational patch family. Point interrogation requires evaluations of $P,P_u,P_v$ and one normalization. For tangent or [normal vector](../../../../../../normal-vector.md) interrogation, differentiate the evaluator. For example,

$$
N_u=P_{uu}\times P_v+P_u\times P_{uv},\qquad n_u=\frac{(I-nn^T)N_u}{\lVert N\rVert},\qquad (P_d)_u=P_u+d n_u,
$$

and similarly for $v$. The offset [normal vector](../../../../../../normal-vector.md) is the normalized [cross product](../../../../../../cross-product.md) $(P_d)_u\times(P_d)_v$ wherever it is nonzero. These derivatives also support intersection, projection and curvature calculations by the usual methods for [parametric surfaces](../../../../../../parametric-surface.md). For a [variable normal offset](../../../../../../variable-normal-offset.md), add $d_u n$ and $d_v n$ to the corresponding tangent derivatives.

With [shape operator](../../../../../../shape-operator.md) $W=-Dn$, the constant-distance offset differential is $DP_d=(I-dW)DP$. Along a principal direction its factor is $1-d\kappa_i$, where $\kappa_i$ is a [principal curvature](../../../../../../principal-curvature.md). Consequently regular interrogation fails at $d\kappa_i=1$; on regular pieces the offset principal curvatures are $\kappa_i/(1-d\kappa_i)$ with the continued normal orientation. Global self-intersections can occur even when both local factors are nonzero. **Evaluate and differentiate the base surface and its normalized normal; an exact conversion back to the original patch type is unnecessary.**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
