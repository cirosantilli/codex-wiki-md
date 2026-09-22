# Krylov dimension from spectral components

↑ **Parent:** [Krylov subspace](krylov-subspace.md)

For a [diagonalizable](diagonalizable-matrix.md) finite-dimensional operator, write $v=\sum_j u_j$ with nonzero $u_j$ in distinct [eigenspaces](eigenspace.md) of eigenvalues $\lambda_j$. Then $A^rv=\sum_j\lambda_j^ru_j$. The [Vandermonde matrix](vandermonde-matrix.md) of the first $k$ powers is invertible for $k$ distinct eigenvalues, so these powers span exactly the $k$ independent components $u_j$. Thus the stabilized [Krylov subspace](krylov-subspace.md) dimension is $k$. It counts distinct spectral components, not the number of nonzero coefficients in an arbitrary eigenbasis: $A=I$, $v=e_1+e_2$ has Krylov dimension one. Equivalently it is the minimum number of eigenvectors needed when those vectors may be chosen freely.

## ↑ Ancestors (8)

1. [Krylov subspace](krylov-subspace.md)
2. [Conjugate gradient method](conjugate-gradient-method.md)
3. [Gradient descent](gradient-descent.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2/38a/solution.md)
