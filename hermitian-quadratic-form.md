# Hermitian quadratic form

↑ **Parent:** [Hermitian operator](hermitian-operator.md)

A bounded [Hermitian operator](hermitian-operator.md) determines a [Hermitian form](hermitian-form.md) $b_T(x,y)=\langle Tx,y\rangle$ and its real-valued diagonal expression $q_T(x)=b_T(x,x)$. On a complex [Hilbert space](hilbert-space-split.md),

$$
q_T(\alpha x)=|\alpha|^2q_T(x).
$$

Thus it is a [quadratic form](quadratic-form-split.md) on the underlying real [vector space](vector-space-split.md); it is generally not a [quadratic form](quadratic-form-split.md) over the complex [field](field.md), whose scaling rule would involve $\alpha^2$. This distinction explains why replacing $x^*$ by $x^{\mathrm T}$ loses the geometry of a complex [inner product](inner-product-split.md).

For a finite-dimensional [Hermitian operator](hermitian-operator.md) with an [orthonormal basis](orthonormal-basis.md) of [eigenvectors](eigenvector.md) $e_j$ and corresponding [eigenvalues](eigenvalue.md) $\lambda_j$, the [spectral theorem](spectral-theorem.md) gives

$$
x=\sum_j c_je_j\quad\Longrightarrow\quad q_T(x)=\sum_j\lambda_j|c_j|^2.
$$

For a [unit vector](unit-vector.md), this is an average of the [eigenvalues](eigenvalue.md) with nonnegative weights summing to one. It is also the [Rayleigh quotient](rayleigh-quotient.md), so its minimum and maximum are the smallest and largest [eigenvalues](eigenvalue.md).

In the [Hermitian operator](hermitian-operator.md) diagram, take $x(\theta)=(\cos\theta,\sin\theta)^{\mathrm T}$ for $D,P$, and $x_H(\theta)=\cos\theta\,e_1+\sin\theta\,e_3$ for $H$. The computed curves are

$$
q_D(x(\theta))=\cos(2\theta),\quad q_P(x(\theta))=\cos^2\theta,\quad q_H(x_H(\theta))=\cos^2\theta+3\sin^2\theta.
$$

These paths illustrate the extremal values; the [spectral theorem](spectral-theorem.md) supplies the bounds for every complex [unit vector](unit-vector.md), including those outside the plotted paths.

## ↑ Ancestors (9)

1. [Hermitian operator](hermitian-operator.md)
2. [Adjoint operator](adjoint-operator.md)
3. [Riesz representation theorem](riesz-representation-theorem.md)
4. [Hilbert space](hilbert-space-split.md)
5. [Functional analysis](functional-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Hermitian operator](hermitian-operator.md)
