<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [Haar sampling by Gaussian QR decomposition](../../../../haar-sampling-by-gaussian-qr-decomposition.md):

- Generate an $n$-by-$n$ real [matrix](../../../../matrix.md) $G$ with [independent](../../../../independent-random-variables.md) entries having the [standard normal distribution](../../../../standard-normal-distribution.md).
- Compute a [QR decomposition](../../../../qr-decomposition.md) $G=Q_0R_0$ with $Q_0$ an [orthogonal matrix](../../../../orthogonal-matrix.md) and $R_0$ an [upper triangular matrix](../../../../upper-triangular-matrix.md).
- Put $S=\operatorname{diag}(\operatorname{sgn}(R_{0,11}),\ldots,\operatorname{sgn}(R_{0,nn}))$ and return $\boxed{M=Q_0S}$. Then $G=MR$ with $R=SR_0$ having strictly positive diagonal.

The [matrix](../../../../matrix.md) $G$ is invertible [almost surely](../../../../almost-sure-convergence.md). Indeed, successively sampled [Gaussian](../../../../normal-distribution.md) columns have [probability](../../../../probability.md) zero of lying in the proper [linear subspace](../../../../vector-subspace.md) spanned by the previous columns. Thus the diagonal signs used above exist with [probability](../../../../probability.md) one. Equivalently, apply the [Gram-Schmidt process](../../../../gram-schmidt-process.md) to the columns, always dividing each residual by its positive [Euclidean norm](../../../../euclidean-norm.md); this produces $M$ directly.

To prove uniformity, fix $H\in O(n)$. Each column of $G$ has density proportional to $e^{-\lVert x\rVert^2/2}$, so [orthogonal transformations](../../../../orthogonal-transformation.md) preserve its [probability distribution](../../../../probability-distribution-split.md). Column [independence](../../../../independent-random-variables.md) therefore gives $HG\overset{\mathrm d}=G$.

The [QR decomposition](../../../../qr-decomposition.md) with positive diagonal is unique: if $G=Q_1R_1=Q_2R_2$, then $Q_2^TQ_1=R_2R_1^{-1}$ is both an [orthogonal matrix](../../../../orthogonal-matrix.md) and an [upper triangular matrix](../../../../upper-triangular-matrix.md), hence diagonal with entries $\pm1$. Its diagonal entries are positive, so it is the identity. It follows that the orthogonal factor of $HG=HMR$ is $HM$. Therefore

$$
\boxed{HM\overset{\mathrm d}=M\quad\text{for every }H\in O(n).}
$$

By uniqueness of normalized [Haar measure](../../../../haar-measure.md) on the [compact group](../../../../compact-group.md) $O(n)$, the returned [matrix](../../../../matrix.md) has exactly the required [probability distribution](../../../../probability-distribution-split.md). Reflection invariance gives each [determinant](../../../../determinant.md) sign [probability](../../../../probability.md) $1/2$, so the algorithm samples both components of the [orthogonal group](../../../../orthogonal-group.md). The positive-diagonal correction is essential when a numerical [QR decomposition](../../../../qr-decomposition.md) chooses its own signs.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the random matrix theory course of the University of Oxford](../../../split.md)
5. [Random matrix theory course of the University of Oxford](../../../../random-matrix-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
