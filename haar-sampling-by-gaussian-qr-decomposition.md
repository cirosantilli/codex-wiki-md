# Haar sampling by Gaussian QR decomposition

↑ **Parent:** [Haar measure](haar-measure.md)

Generate a real $n$-by-$n$ [matrix](matrix.md) $G$ with [independent](independent-random-variables.md) entries having the [standard normal distribution](standard-normal-distribution.md). Take its [QR decomposition](qr-decomposition.md) with positive diagonal in the [upper triangular matrix](upper-triangular-matrix.md) factor, $G=QR$. The [orthogonal matrix](orthogonal-matrix.md) $Q$ has normalized [Haar measure](haar-measure.md) on the full [orthogonal group](orthogonal-group.md) $O(n)$. If a numerical factorization returns $Q_0R_0$, set $S=\operatorname{diag}(\operatorname{sgn}R_{0,ii})$ and return $Q_0S$. The signs are nonzero [almost surely](almost-sure-convergence.md): successively drawn [Gaussian](normal-distribution.md) columns have [probability](probability.md) zero of lying in the proper [linear subspace](vector-subspace.md) spanned by earlier columns.

For correctness, every fixed [orthogonal matrix](orthogonal-matrix.md) $U$ preserves the standard [Gaussian](normal-distribution.md) column density and column [independence](independent-random-variables.md), so $UG$ and $G$ have the same [probability distribution](probability-distribution-split.md). The positive-diagonal [QR decomposition](qr-decomposition.md) is unique: two decompositions would give an [orthogonal matrix](orthogonal-matrix.md) that is also an [upper triangular matrix](upper-triangular-matrix.md) with positive diagonal, hence the identity. Therefore $Q(UG)=UQ(G)$ and $Q(G)$ has a left-invariant probability law. Uniqueness of normalized [Haar measure](haar-measure.md) on the [compact group](compact-group.md) $O(n)$ identifies that law. Each [determinant](determinant.md) sign has [probability](probability.md) $1/2$ by reflection invariance.

## ↑ Ancestors (8)

1. [Haar measure](haar-measure.md)
2. [Measure](measure-split.md)
3. [Measure theory](measure-theory-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-random-matrix-theory-course-of-the-university-of-oxford/2025/3/d/solution.md)
