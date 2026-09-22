# Similarity transformation

↑ **Parent:** [Matrix similarity](matrix-similarity.md)

A [similarity transformation](similarity-transformation.md) replaces a [square matrix](square-matrix.md) by a similar [matrix](matrix.md). With the [change-of-basis matrix](change-of-basis-matrix.md) convention $x=Sy$, it sends $A$ to $B=S^{-1}AS$: reconstruct the input in old [coordinates](coordinate-linear-algebra.md), apply $A$, then extract the output's new [coordinates](coordinate-linear-algebra.md). These three operations explain the order of the factors.

The equivalent formula $A\mapsto SAS^{-1}$ uses $S$ as the conversion from old to new [coordinates](coordinate-linear-algebra.md), reversing the role assigned to $S$ above. For the opening example's numerical $S$, this opposite conversion gives $SAS^{-1}=\begin{pmatrix}2&3\\0&5\end{pmatrix}$. If the old [basis](basis.md) is $\mathcal E$, the new [basis vectors](basis-vector.md) in that convention are the columns of $S^{-1}$, namely $e_1$ and $-e_1+e_2$. Both formulas are [similarity transformations](similarity-transformation.md); the direction of the coordinate conversion decides which one describes a specified [basis](basis.md).

An especially useful form is the [intertwining operator](intertwining-operator.md) equation

$$
AS=SB.
$$

It says that applying $B$ before reconstruction by $S$ gives the same physical output as reconstructing first and applying $A$. Given an [invertible matrix](invertible-matrix.md) $S$, multiplying this equation by $S^{-1}$ proves [matrix similarity](matrix-similarity.md). Without invertibility, the equation alone does not prove [matrix similarity](matrix-similarity.md).

<a id="image-matrix-similarity-makes-coordinate-conversion-commute-with-the-action-of-a-linear-operator"></a>
![](matrix-similarity-intertwining-invariants.png)

**[Figure 22](#image-matrix-similarity-makes-coordinate-conversion-commute-with-the-action-of-a-linear-operator). Matrix similarity makes coordinate conversion commute with the action of a linear operator**. For the worked example, both routes give the old output [coordinate vector](coordinate-vector.md) $(4,5)^T$. The bottom strip records [matrix similarity invariants](matrix-similarity-invariants.md); the [eigenvector](eigenvector.md) tuple changes while reconstructing to the same vertical [vector](vector.md).

**Table of contents**

- [Similarity and the coordinate metric](similarity-and-the-coordinate-metric.md)
- [Positive diagonal symmetrization of a matrix](positive-diagonal-symmetrization-of-a-matrix.md)
- [Every automorphism of a full matrix algebra is inner](every-automorphism-of-a-full-matrix-algebra-is-inner.md)

## ↑ Ancestors (6)

1. [Matrix similarity](matrix-similarity.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (21)

- [Diagonal scaling of Gershgorin discs](diagonal-scaling-of-gershgorin-discs.md)
- [Dirac-to-Weyl gamma-matrix similarity transform](dirac-to-weyl-gamma-matrix-similarity-transform.md)
- [Eigenvalue deflation by an invariant subspace](eigenvalue-deflation-by-an-invariant-subspace.md)
- [Gamma matrix adjoint and transpose identities](gamma-matrix-adjoint-and-transpose-identities.md)
- [Gauge equivalence of injective matrix product state tensors](gauge-equivalence-of-injective-matrix-product-state-tensors.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-3/9b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3/17g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-1/7b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-4/1e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-301/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-301/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1/40e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-2/17b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-2/17/c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-2/10/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-2/10/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/9/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-1/6/b/solution.md)
- [Positive diagonal symmetrization of a matrix](positive-diagonal-symmetrization-of-a-matrix.md)
- [Right preconditioning](right-preconditioning.md)
- [Similarity transformation](similarity-transformation.md)
