# Hilbert space completion

↑ **Parent:** [Hilbert space](hilbert-space-split.md)

The Hilbert space completion of an [inner product space](inner-product-space.md) $V$ is a [Hilbert space](hilbert-space-split.md) containing an isometric dense copy of $V$. It can be constructed from [Cauchy sequences](cauchy-sequence.md) in $V$, identifying two sequences when the norm of their difference tends to zero.

The space of [finitely supported sequences](finitely-supported-sequence.md) with the [l2 sequence space](l2-sequence-space.md) [norm](norm.md) illustrates the need for completion. Let $u^{(n)}=(1,1/2,\ldots,1/n,0,\ldots)$. For $m>n$,

$$
\|u^{(m)}-u^{(n)}\|_2^2=\sum_{k=n+1}^{m}\frac1{k^2}\leq\int_n^{\infty}\frac{dx}{x^2}=\frac1n.
$$

This is a [Cauchy sequence](cauchy-sequence.md), but its coordinatewise [limit](limit-of-a-function.md) $(1/k)_{k\geq1}$ is not finitely supported. It belongs to the [l2 sequence space](l2-sequence-space.md), which is the completion. The same construction permits infinitely many small components while controlling their total squared size. An infinite [orthonormal basis](orthonormal-basis.md) of a [Hilbert space](hilbert-space-split.md) consequently permits norm-convergent series; a [Hamel basis](basis.md) represents each [vector](vector.md) by a finite sum, so these two uses of "basis" must be distinguished.

**Table of contents**

- [Mean-square completion of trigonometric polynomials](mean-square-completion-of-trigonometric-polynomials.md)

## ↑ Ancestors (6)

1. [Hilbert space](hilbert-space-split.md)
2. [Functional analysis](functional-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Gupta-Bleuler null-state quotient](gupta-bleuler-null-state-quotient.md)
- [Hilbert projection theorem](hilbert-projection-theorem.md)
- [Mean-square completion of trigonometric polynomials](mean-square-completion-of-trigonometric-polynomials.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-5/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-203/4/a/ii/solution.md)
- [Positive semidefinite Hermitian form](positive-semidefinite-hermitian-form.md)
