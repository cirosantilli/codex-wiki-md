<h1 id="1/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [bounded linear operator](../../../../../../../continuous-linear-operator.md) $K:U\to V$ between [Hilbert spaces](../../../../../../../hilbert-space-split.md), a [least-squares solution](../../../../../../../least-squares-solution-of-a-linear-inverse-problem.md) of data $f$ is a minimizer of the residual [norm](../../../../../../../norm.md):

$$
\bar u\in\arg\min_{u\in U}\|Ku-f\|_V^2.
$$

The [minimum-norm least-squares solution](../../../../../../../minimum-norm-least-squares-solution.md) is the one of smallest $U$-norm among these minimizers. Equivalently it is the unique [least-squares solution](../../../../../../../least-squares-solution-of-a-linear-inverse-problem.md) in $\mathcal N(K)^\perp$. If the equation is consistent, this is the smallest-norm exact solution.

Let $P$ be the [orthogonal projection](../../../../../../../orthogonal-projection.md) onto $\overline{\mathcal R(K)}$. The [orthogonal decomposition by a closed subspace](../../../../../../../orthogonal-decomposition-by-a-closed-subspace.md) gives

$$
\|Ku-f\|^2=\|Ku-Pf\|^2+\|(I-P)f\|^2.
$$

The first term has infimum zero by the definition of closure; that infimum is attained exactly if $Pf\in\mathcal R(K)$. This proves the [least-squares existence criterion](../../../../../../../least-squares-existence-criterion.md):

$$
\boxed{\text{least-squares solutions exist}\iff f\in\mathcal R(K)\oplus\mathcal R(K)^\perp.}
$$

They exist for every datum precisely when the range is closed. Once a solution exists, all solutions differ by elements of the closed [null space](../../../../../../../kernel-of-a-linear-map.md), and projecting onto its [orthogonal complement](../../../../../../../orthogonal-complement.md) gives the unique minimum-norm solution.

For a counterexample to existence, take $K:\ell^2\to\ell^2$, $(Ku)_j=u_j/j$, and $f_j=1/j$. The range is dense, so the least residual infimum is zero; finite truncations realize residuals tending to zero. But an exact preimage would have every coordinate equal to one and would not belong to $\ell^2$. Thus no least-squares minimizer exists for this datum.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
