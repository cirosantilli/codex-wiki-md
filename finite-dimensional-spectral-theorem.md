# Finite-dimensional spectral theorem

↑ **Parent:** [Self-adjoint operator](self-adjoint-operator.md)

Every [self-adjoint operator](self-adjoint-operator.md) on a finite-dimensional real or complex [inner product space](inner-product-space.md) has an [orthonormal eigenbasis](orthonormal-eigenbasis.md), and all its [eigenvalues](eigenvalue.md) are real. In orthonormal coordinates, a real [symmetric matrix](symmetric-matrix.md) has the form $A=Q\Lambda Q^T$, with $Q$ an [orthogonal matrix](orthogonal-matrix.md) and $\Lambda$ a real [diagonal matrix](diagonal-matrix.md). A complex [Hermitian matrix](hermitian-operator.md) instead has $A=U\Lambda U^*$, with $U$ a [unitary matrix](unitary-matrix.md) and $U^*$ its [conjugate transpose](conjugate-transpose.md). These are the self-adjoint cases of the [spectral theorem](spectral-theorem.md); Axler gives the real and complex finite-dimensional statements in Section 7B.[Sheldon Axler, Linear Algebra Done Right, fourth edition, Section 7B, Theorems 7.29 and 7.31; accessed 2026-10-11](https://linear.axler.net/LADR4e.pdf)

An [orthonormal eigenbasis](orthonormal-eigenbasis.md) turns a seemingly coupled [linear map](linear-map.md) into independent [scalar multiplications](scalar-multiplication.md) while preserving [lengths](length.md) and [angles](angle.md). If $x=\sum_j c_je_j$ and $Ae_j=\lambda_je_j$, then

$$
Ax=\sum_j\lambda_jc_je_j,\qquad
\|x\|^2=\sum_j|c_j|^2,\qquad
x^*Ax=\sum_j\lambda_j|c_j|^2.
$$

The last identity removes every cross term from the [quadratic form](quadratic-form.md). The [eigenvalues](eigenvalue.md) tell us whether it is positive, negative, or mixed in sign, and the [eigenvectors](eigenvector.md) identify the corresponding directions. This connects [positive-definite matrices](positive-definite-matrix.md), [quadratic forms](quadratic-form.md), and the [Hermitian Rayleigh quotient range](hermitian-rayleigh-quotient-range.md).

For a fully computed example, take

$$
A=\begin{pmatrix}2&1\\1&2\end{pmatrix},\qquad
e_+=\frac1{\sqrt2}\begin{pmatrix}1\\1\end{pmatrix},\qquad
e_-=\frac1{\sqrt2}\begin{pmatrix}-1\\1\end{pmatrix}.
$$

Direct multiplication gives $Ae_+=3e_+$ and $Ae_-=e_-$. Their [dot product](dot-product.md) is zero and each has [norm](norm.md) one. Thus

$$
Q=\frac1{\sqrt2}\begin{pmatrix}1&-1\\1&1\end{pmatrix},\qquad
Q^TAQ=\begin{pmatrix}3&0\\0&1\end{pmatrix}.
$$

Writing $x=ce_++de_-$ changes $x^TAx=2x_1^2+2x_1x_2+2x_2^2$ into $3c^2+d^2$. Its [level set](level-set.md) $x^TAx=1$ is therefore an [ellipse](ellipse.md) with semiaxis lengths $1/\sqrt3$ and $1$, along $e_+$ and $e_-$. The coordinates change, but the [ellipse](ellipse.md) does not: [orthogonal diagonalization](orthogonal-diagonalization-of-a-real-symmetric-matrix.md) reveals its existing geometry.

<a id="image-an-orthonormal-eigenbasis-removes-the-cross-term-from-a-quadratic-form-and-reveals-the-axes-of-its-ellipse"></a>
![](spectral-theorem-ellipse-coordinates.png)

**[Figure 3](#image-an-orthonormal-eigenbasis-removes-the-cross-term-from-a-quadratic-form-and-reveals-the-axes-of-its-ellipse). An orthonormal eigenbasis removes the cross term from a quadratic form and reveals the axes of its ellipse**.

For distinct [eigenvalues](eigenvalue.md), orthogonality follows at once from self-adjointness: $\lambda\langle u,v\rangle=\langle Au,v\rangle=\langle u,Av\rangle=\mu\langle u,v\rangle$. Within a repeated [eigenspace](eigenspace.md), choose an [orthonormal basis](orthonormal-basis.md); arbitrarily chosen [eigenvectors](eigenvector.md) of the same [eigenvalue](eigenvalue.md) need not be orthogonal. One outline of the full argument finds an [eigenvector](eigenvector.md), observes that its [orthogonal complement](orthogonal-complement.md) is invariant, and repeats in that smaller space. Merely having real [eigenvalues](eigenvalue.md) is weaker: $\begin{pmatrix}2&1\\0&1\end{pmatrix}$ has two real [eigenvalues](eigenvalue.md), but its [eigenvectors](eigenvector.md) $(1,0)^T$ and $(-1,1)^T$ are not orthogonal.

**Table of contents**

- [Multiplicity-free complete dyadic spectrum](multiplicity-free-complete-dyadic-spectrum.md)
- [Orthonormal eigenbasis](orthonormal-eigenbasis.md)
- [Spectral projection of a self-adjoint matrix](spectral-projection-of-a-self-adjoint-matrix.md)

## ↑ Ancestors (7)

1. [Self-adjoint operator](self-adjoint-operator.md)
2. [Operator theory](linear-operator-theory-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (17)

- [Cumulative coherence bound for restricted isometry](cumulative-coherence-bound-for-restricted-isometry.md)
- [Gershgorin bounds for symmetric matrices](gershgorin-bounds-for-symmetric-matrices.md)
- [Gershgorin circle theorem](gershgorin-circle-theorem.md)
- [Hermitian Rayleigh quotient range](hermitian-rayleigh-quotient-range.md)
- [Orthonormal eigenbasis](orthonormal-eigenbasis.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-36/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-36/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/37e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-36/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-4/10e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-323/3/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-1/7b/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3/9f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-335/3/i/solution.md)
- [Rayleigh quotient](rayleigh-quotient.md)
- [Real spectral theorem](real-spectral-theorem.md)
