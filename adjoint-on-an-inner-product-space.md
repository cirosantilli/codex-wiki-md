# Adjoint on an inner product space

↑ **Parent:** [Adjoint operator](adjoint-operator.md)

On a complex [inner product space](inner-product-space.md) $V$, with the [inner product](inner-product-split.md) conjugate-linear in its first argument, an everywhere-defined linear map $T:V\to V$ admits an adjoint on $V$ if there is a linear map $T^*:V\to V$ satisfying

$$
\langle Tx,y\rangle=\langle x,T^*y\rangle\qquad(x,y\in V).
$$

The adjoint, when it exists, is unique: the difference of two candidate values at $y$ is orthogonal to every vector and hence to itself. In a [finite-dimensional vector space](finite-dimensional-vector-space.md), it always exists, and its matrix in an [orthonormal basis](orthonormal-basis.md) is the conjugate transpose. In a space that is not complete, existence must instead be checked.

The identity $\langle Tx,y\rangle=\langle x,Ty\rangle$ for every $x,y\in V$ supplies such an adjoint directly, namely $T^*=T$. This algebraic statement should be distinguished from [self-adjointness](self-adjoint-operator.md) of a [linear operator](linear-operator.md) on a completed [Hilbert space](hilbert-space-split.md), which additionally compares the domains of an operator and its Hilbert-space adjoint. The [Gaussian polynomial operator](gaussian-polynomial-operator.md) is a useful example where the identity holds on the entire polynomial [inner product space](inner-product-space.md) and can be used on every finite-dimensional invariant polynomial subspace.

## ↑ Ancestors (8)

1. [Adjoint operator](adjoint-operator.md)
2. [Riesz representation theorem](riesz-representation-theorem.md)
3. [Hilbert space](hilbert-space-split.md)
4. [Functional analysis](functional-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Gaussian polynomial operator](gaussian-polynomial-operator.md)
- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-2-course-of-the-university-of-oxford/2007/2/solution.md)
- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-2-course-of-the-university-of-oxford/2012/2/b/solution.md)
- [Solution](past-exam-of-the-linear-algebra-course-of-the-university-of-oxford/2017/3/b/ii/solution.md)
