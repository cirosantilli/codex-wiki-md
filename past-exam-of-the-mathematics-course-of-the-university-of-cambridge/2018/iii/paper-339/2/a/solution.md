<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a feasible vector, set $X=xx^T$. It is a [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md), and

$$
\operatorname{tr}(a_ia_i^TX)=a_i^Txx^Ta_i=(a_i^Tx)^2\le1,\qquad
\operatorname{tr}X=\|x\|_2^2.
$$

Thus every original feasible point supplies an equally valuable SDP feasible point. Dropping the rank-one restriction is the [semidefinite relaxation of slab-constrained quadratic maximization](../../../../../../semidefinite-relaxation-of-slab-constrained-quadratic-maximization.md), proving

$$
\boxed{p_{\rm SDP}^*\ge v^*.}
$$

The original PDF has $|a_i^Tx|\le1$; the absolute values are missing from the extracted TeX and are essential for this relaxation.

For the subsequent finite rounding argument, the constraint vectors must span $\mathbb R^n$. Otherwise a nonzero common-kernel vector $d$ makes both $x=td$ and $X=tdd^T$ unbounded feasible families, so both objective suprema are infinite. Under spanning, $H=\sum_i a_ia_i^T$ is a [positive-definite matrix](../../../../../../positive-definite-matrix.md) and

$$
\lambda_{\min}(H)\operatorname{tr}X\le\operatorname{tr}(HX)=\sum_i a_i^TXa_i\le m.
$$

The first inequality uses [positive semidefinite trace nonnegativity](../../../../../../positive-semidefinite-trace-nonnegativity.md). The SDP feasible set is closed and bounded, hence compact, so an optimum exists. Its trace is positive: a sufficiently small positive multiple of the identity is feasible when $n\ge1$. These facts justify the optimum and nonzero denominator used below. Assume $m,n\ge1$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
