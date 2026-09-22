# Orthogonal projection matrix

↑ **Parent:** [Orthogonal projection onto a finite-dimensional subspace](orthogonal-projection-onto-a-finite-dimensional-subspace.md)

A [matrix](matrix.md) represents a [linear projection](projection-linear-algebra.md) when applying it twice has the same effect as applying it once. For an [orthogonal projection](orthogonal-projection.md) with the standard [Hermitian inner product](hermitian-inner-product.md) on $\mathbb C^m$, the additional condition is that the [conjugate transpose](conjugate-transpose.md) equals the original [matrix](matrix.md):

$$
P^2=P=P^\dagger.
$$

Thus $P$ is both [idempotent](idempotent.md) and a [Hermitian matrix](hermitian-operator.md). Over the [real numbers](real-number.md) this says $P^2=P=P^T$. Its [image of a linear map](image-of-a-linear-map.md) is the retained [linear subspace](vector-subspace.md), while its [kernel of a linear map](kernel-of-a-linear-map.md) is the [orthogonal complement](orthogonal-complement.md): [vectors](vector.md) in the image are unchanged, and [vectors](vector.md) in the kernel become zero.

For a [matrix](matrix.md) $A$ with [full column rank](full-column-rank.md), projecting onto its [column space](column-space.md) gives

$$
P=A(A^\dagger A)^{-1}A^\dagger.
$$

The invertibility of $A^\dagger A$ follows from [linear independence](linear-independence.md) of the columns. If those columns are an [orthonormal set](orthonormal-set.md), $A^\dagger A=I$ and $P=AA^\dagger$. These formulas and the conditions $P^2=P=P^T$ in the real case are developed in [MIT 18.06SC, Projections onto Subspaces, pp. 1–3](https://www.ocw.mit.edu/courses/18-06sc-linear-algebra-fall-2011/00e9c8f0eafedeab21a3d079a17ed3d8_MIT18_06SCF11_Ses2.2sum.pdf).

For the line spanned by $e=(1,2)^T$,

$$
P=\frac{ee^T}{e^Te}
=\frac15\begin{pmatrix}1&2\\2&4\end{pmatrix},
\qquad
P(3,1)^T=(1,2)^T.
$$

In particular, $Pe=e$ and $P(2,-1)^T=0$. The [eigenvalues](eigenvalue.md) are $1$ on the retained direction and $0$ on the removed direction. This exposes the meaning of an [orthogonal projection](orthogonal-projection.md) as retaining selected components, rather than stretching them.

Symmetry refers to the specified [inner product](inner-product.md). In the real weighted setting, the formula becomes $P_M=A(A^TMA)^{-1}A^TM$ and satisfies $P_M^2=P_M$ and $P_M^TM=MP_M$. For the preceding weighted line example,

$$
P_M=\frac18\begin{pmatrix}4&2\\8&4\end{pmatrix}.
$$

It is not symmetric under the ordinary [transpose](transpose.md), but it is an [orthogonal projection](orthogonal-projection.md) for the [weighted Euclidean inner product](weighted-euclidean-inner-product.md). The matrix criterion $P=P^\dagger$ should therefore be used with the standard [Hermitian inner product](hermitian-inner-product.md), not silently transferred to a different geometry.

**Table of contents**

- [Transverse projection operator](transverse-projection-operator.md)

## ↑ Ancestors (7)

1. [Orthogonal projection onto a finite-dimensional subspace](orthogonal-projection-onto-a-finite-dimensional-subspace.md)
2. [Inner product](inner-product.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (28)

- [All-ones matrix](all-ones-matrix.md)
- [Complex Grassmannian as orthogonal projections](complex-grassmannian-as-orthogonal-projections.md)
- [Davis-Kahan curvature lemma](davis-kahan-curvature-lemma.md)
- [Fantope](fantope.md)
- [Fitted values](fitted-values.md)
- [Frobenius norm](frobenius-norm.md)
- [Ky Fan maximum principle](ky-fan-maximum-principle.md)
- [Mean-vector prediction risk](mean-vector-prediction-risk.md)
- [Moore-Penrose inverse](moore-penrose-inverse.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-16/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-1/8a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-41/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-44/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-32/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-37/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-30/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3/20h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-1/18d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-339/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-2/18h/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-1/7b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-1/7b/d/solution.md)
- [Penrose equations](penrose-equations.md)
- [Sign rounding bound for a unit eigenvector](sign-rounding-bound-for-a-unit-eigenvector.md)
- [Sum of squares in ANOVA](sum-of-squares-in-anova.md)
- [Unbiased Gaussian projection risk estimate](unbiased-gaussian-projection-risk-estimate.md)
- [Unknown-variance risk estimation in a saturated Gaussian model](unknown-variance-risk-estimation-in-a-saturated-gaussian-model.md)
