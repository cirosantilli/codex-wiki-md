# Power method

↑ **Parent:** [Operator theory](linear-operator-theory-split.md)

Iterate $q^{(k+1)}=Aq^{(k)}/\|Aq^{(k)}\|$. For a [self-adjoint operator](self-adjoint-operator.md) with a unique [dominant eigenvalue](dominant-eigenvalue.md) separated in [modulus](modulus.md) from the others, a starting [vector](vector.md) that is [nonorthogonal](nonorthogonal-vectors.md) to its dominant [eigenvector](eigenvector.md) gives convergence of the eigendirection at the spectral-ratio rate. For a general [diagonalizable matrix](diagonalizable-matrix.md), the condition is a nonzero coefficient in the dominant component of its [eigenbasis](eigenbasis.md), detected by the corresponding [left eigenvector](left-eigenvector.md); an ordinary [dot product](dot-product.md) with the right [eigenvector](eigenvector.md) does not generally detect that coefficient.

The power method is [power iteration](power-iteration.md); its convergence depends on the dominant spectral component of the starting vector.

For example, $B=\begin{pmatrix}2&1\\0&1\end{pmatrix}$ has dominant right [eigenvector](eigenvector.md) $(1,0)^T$ and a dominant [left eigenvector](left-eigenvector.md) $(1,1)^T$. The starting [vector](vector.md) $q^{(0)}=(-1,1)^T/\sqrt2$ has nonzero [dot product](dot-product.md) with the right [eigenvector](eigenvector.md), but $Bq^{(0)}=q^{(0)}$: it stays forever in the [eigenspace](eigenspace.md) for the smaller [eigenvalue](eigenvalue.md) $1$. Its coefficient along the dominant direction is zero, as the left [eigenvector](eigenvector.md) detects. An [orthonormal eigenbasis](orthonormal-eigenbasis.md) makes the two tests agree in the self-adjoint case.

**Table of contents**

- [Dominant eigenpair extraction from a two-step Krylov recurrence](dominant-eigenpair-extraction-from-a-two-step-krylov-recurrence.md)
- [Quadratic Rayleigh-quotient improvement for the power method](quadratic-rayleigh-quotient-improvement-for-the-power-method.md)
- [Active spectrum of the power method](active-spectrum-of-the-power-method.md)
- [Inverse iteration](inverse-iteration.md)
  - [Convergence of fixed-shift inverse iteration](convergence-of-fixed-shift-inverse-iteration.md)
    - [Sign behavior of fixed-shift inverse iteration](sign-behavior-of-fixed-shift-inverse-iteration.md)
- [Subspace iteration](subspace-iteration.md)
  - [Dominant invariant subspace](dominant-invariant-subspace.md)
  - [Power method with a dominant eigenvalue cluster](power-method-with-a-dominant-eigenvalue-cluster.md)

## ↑ Ancestors (6)

1. [Operator theory](linear-operator-theory-split.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Active spectrum of the power method](active-spectrum-of-the-power-method.md)
- [Diagonalizable matrix](diagonalizable-matrix.md)
- [Nonorthogonal vectors](nonorthogonal-vectors.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4/39c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/41e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-3/40c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-3/40c/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-4/40a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-4/40a/b/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-1/41b/a/solution.md)
- [Power iteration](power-iteration.md)
- [Spectral gap](spectral-gap.md)
