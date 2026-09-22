<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Every feasible sign [vector](../../../../../../vector.md) gives the [rank-one matrix](../../../../../../rank-one-matrix.md) $X=xx^T$. It is a [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md), since $u^TXu=(u^Tx)^2\geq0$, and $X_{ii}=x_i^2=1$. The [matrix trace](../../../../../../matrix-trace.md) identity gives

$$
\operatorname{tr}(Axx^T)=x^TAx.
$$

Thus all original feasible objectives appear among the relaxed ones, proving

$$
\boxed{p_{\rm SDP}^*\geq v^*}.
$$

The [semidefinite relaxation of binary quadratic optimization](../../../../../../semidefinite-relaxation-of-binary-quadratic-optimization.md) drops the rank-one requirement and keeps the [elliptope](../../../../../../elliptope.md) constraints.

An optimal relaxed [matrix](../../../../../../matrix.md) exists. The feasible set is nonempty, since it contains $I$, and closed. Its two-by-two [principal minors](../../../../../../principal-minor.md) give $|X_{ij}|^2\leq X_{ii}X_{jj}=1$, so it is bounded and therefore [compact](../../../../../../compact-space.md). The linear objective attains its maximum. Also $\operatorname{tr}(AI)=0$ and hence $p_{\rm SDP}^*\geq0$, including the zero-objective case.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
