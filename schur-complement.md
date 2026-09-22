# Schur complement

↑ **Parent:** [Linear algebra](linear-algebra-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schur_complement)

For a [block matrix](block-matrix.md) $M=\begin{pmatrix}A&B\\C&D\end{pmatrix}$ with $A$ an [invertible matrix](invertible-matrix.md), the [Schur complement](schur-complement.md) of $A$ in $M$ is $S=D-CA^{-1}B$. It is the effective coefficient [matrix](matrix.md) for the remaining variables after [block elimination](block-elimination.md). The definition requires invertibility of $A$, but not of $S$ or $M$. Its size is that of $D$, even when $B$ and $C$ are rectangular [matrices](matrix.md).

In the original example under [block matrix inverse](block-matrix-inverse.md), $D=5$ becomes $S=19/6$ because changing the remaining variable also changes the two variables solved through $A$. This is what makes a [Schur complement](schur-complement.md) more informative than simply deleting rows and columns. It retains their mediated effect, and its [matrix inverse](matrix-inverse-split.md) is the corresponding block of $M^{-1}$ when the [block matrix inverse](block-matrix-inverse.md) exists.

The same elimination appears when minimizing a [quadratic form](quadratic-form-split.md). The [Schur complement as a minimized quadratic form](schur-complement-as-a-minimized-quadratic-form.md) gives a geometric example; the [Schur complement determinant identity](schur-complement-determinant-identity.md) gives an exact test for an [invertible matrix](invertible-matrix.md).

**Table of contents**

- [Schur complement as a minimized quadratic form](schur-complement-as-a-minimized-quadratic-form.md)
- [Schur complement determinant identity](schur-complement-determinant-identity.md)
- [Schur complement formula for a diagonal resolvent entry](schur-complement-formula-for-a-diagonal-resolvent-entry.md)

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (49)

- [Block elimination](block-elimination.md)
- [Block matrix inverse](block-matrix-inverse.md)
- [Buscher dual of a metric with vanishing two-form](buscher-dual-of-a-metric-with-vanishing-two-form.md)
- [Cholesky decomposition](cholesky-decomposition.md)
- [Choosing a different block pivot](choosing-a-different-block-pivot.md)
- [Columnwise partial pivoting](columnwise-partial-pivoting.md)
- [Complement theta number](complement-theta-number.md)
- [Elimination graph](elimination-graph.md)
- [Fill-in](fill-in.md)
- [Free adjoint-scalar propagator in scalar-dependent gauge fixing](free-adjoint-scalar-propagator-in-scalar-dependent-gauge-fixing.md)
- [Handle-slide isolation of a cancelling pair](handle-slide-isolation-of-a-cancelling-pair.md)
- [LDL decomposition](ldl-decomposition.md)
- [Leaf elimination of a tree-pattern positive-definite matrix](leaf-elimination-of-a-tree-pattern-positive-definite-matrix.md)
- [Matrix decomposition](matrix-decomposition.md)
- [Minimum degree algorithm](minimum-degree-algorithm.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-2/14e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-32/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-32/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-13/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-60/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-27/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-43/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-46/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-18/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-10/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-31/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-31/3/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-48/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-32/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-116/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219/3/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-304/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-339/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-344/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-1/5b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-339/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-209/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-111/2/c/solution.md)
- [Perfect elimination ordering](perfect-elimination-ordering.md)
- [Safe pivots for tridiagonal elimination](safe-pivots-for-tridiagonal-elimination.md)
- [Schur complement](schur-complement.md)
- [Schur complement as a minimized quadratic form](schur-complement-as-a-minimized-quadratic-form.md)
- [Schur complement determinant identity](schur-complement-determinant-identity.md)
- [Smooth completing-square proof of the Morse lemma](smooth-completing-square-proof-of-the-morse-lemma.md)
- [Sparse elimination of a four-leaf star](sparse-elimination-of-a-four-leaf-star.md)
- [Sparse Gaussian elimination](sparse-gaussian-elimination.md)
- [Sylvester's criterion](sylvester-s-criterion.md)
- [Time-reversal invariance of a path Jacobian](time-reversal-invariance-of-a-path-jacobian.md)
