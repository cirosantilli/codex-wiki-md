# Convergence criterion for a stationary iteration

↑ **Parent:** [Iteration matrix](iteration-matrix.md)

A [stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md) converges to its specified [fixed point](fixed-point.md) for every initial [vector](vector.md) if and only if its [iteration matrix](iteration-matrix.md) satisfies $\rho(H)<1$, where the [spectral radius](spectral-radius.md) is the largest [modulus](modulus.md) of an [eigenvalue](eigenvalue.md).[Math 221, Matrix Computations, Fall 2009; Basic iterative methods: theorem following the spectral-radius lemmas, before the Jacobi update](math-221-matrix-computations-fall-2009/notes-for-ma221-lecture-21-nov-10-2009.md)

For a [diagonalizable matrix](diagonalizable-matrix.md), write $H=V\Lambda V^{-1}$. Then $H^k=V\Lambda^kV^{-1}$, so each [eigenvector](eigenvector.md) coefficient tends to zero exactly when its [eigenvalue](eigenvalue.md) has [modulus](modulus.md) less than one. For a general [matrix](matrix.md), the [Jordan normal form](jordan-normal-form.md) gives the same result: a [Jordan block](jordan-block.md) $J=\lambda I+K$ with a [nilpotent matrix](nilpotent-matrix.md) $K$ of size $m$ satisfies

$$
J^k=\sum_{j=0}^{\min(k,m-1)}\binom{k}{j}\lambda^{k-j}K^j.
$$

If $0<|\lambda|<1$, every coefficient tends to zero because [exponential decay](exponential-decay.md) beats any fixed [polynomial](polynomial-split.md) in $k$; if $\lambda=0$, the block vanishes once $k\geq m$. Conversely, an [eigenvector](eigenvector.md) with $|\lambda|\geq1$ provides an initial error that cannot tend to zero. For a real [matrix](matrix.md) with complex [eigenvalues](eigenvalue.md), the same obstruction appears in the real [invariant subspace](invariant-subspace.md) spanned by the real and imaginary parts of an [eigenvector](eigenvector.md).

The words "every initial [vector](vector.md)" matter. For example, $H=\operatorname{diag}(3/2,1/2)$ fails the criterion, but $e^{(0)}=(0,1)^T$ still tends to zero. Here a generic initial error has a nonzero first coordinate and diverges; the exceptional errors lie on the second coordinate axis. With $H=\operatorname{diag}(-1,1/2)$, generic errors oscillate rather than diverge in [norm](norm.md), while the same exceptional axis still converges. Both are valid [matrix splittings](matrix-splitting.md) with $M=I$ and $A=I-H$. In general the convergent errors form the [direct sum](direct-sum.md) of the [generalized eigenspaces](generalized-eigenspace.md) for $|\lambda|<1$; if $\rho(H)\geq1$, this is a proper [linear subspace](vector-subspace.md).

A small [spectral radius](spectral-radius.md) describes eventual convergence, but does not imply that the [Euclidean norm](euclidean-norm.md) of the error decreases on every step for a [non-normal matrix](non-normal-matrix.md). An [operator norm](operator-norm.md) bound $\|H\|<1$ does give the stepwise estimate $\|e^{(k)}\|\leq\|H\|^k\|e^{(0)}\|$. For a real [symmetric matrix](symmetric-matrix.md), the [matrix 2-norm](matrix-2-norm.md) equals its [spectral radius](spectral-radius.md), making this particularly direct.

## ↑ Ancestors (8)

1. [Iteration matrix](iteration-matrix.md)
2. [Stationary iterative method for a linear system](stationary-iterative-method-for-a-linear-system.md)
3. [Numerical linear algebra](numerical-linear-algebra-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Gauss-Seidel convergence from diagonal dominance and positive definiteness](gauss-seidel-convergence-from-diagonal-dominance-and-positive-definiteness.md)
- [Jacobi method](jacobi-method.md)
- [Matrix splitting](matrix-splitting.md)
