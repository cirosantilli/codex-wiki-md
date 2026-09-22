# Spectral projection of a self-adjoint matrix

↑ **Parent:** [Finite-dimensional spectral theorem](finite-dimensional-spectral-theorem.md)

For a finite-dimensional [Hermitian matrix](hermitian-operator.md) $A$, its spectral projection $P_\lambda$ is the [orthogonal projection](orthogonal-projection.md) onto the [eigenspace](eigenspace.md) for $\lambda$. In an [orthonormal eigenbasis](orthonormal-eigenbasis.md), the displayed sum is over every basis [vector](vector.md) with that [eigenvalue](eigenvalue.md). The projection is independent of the choice of basis within a repeated [eigenspace](eigenspace.md). For distinct [eigenvalues](eigenvalue.md) $\lambda,\mu$,

$$
P_\lambda^*=P_\lambda,\qquad P_\lambda^2=P_\lambda,\qquad
P_\lambda P_\mu=0,\qquad
\sum_\lambda P_\lambda=I,\qquad A=\sum_\lambda\lambda P_\lambda.
$$

This is the [spectral decomposition](spectral-decomposition.md) grouped by distinct [eigenvalues](eigenvalue.md): decompose a [vector](vector.md) into orthogonal pieces, then scale each piece. For the matrix $A=\begin{pmatrix}2&1\\1&2\end{pmatrix}$,

$$
P_3=\frac12\begin{pmatrix}1&1\\1&1\end{pmatrix},\qquad
P_1=\frac12\begin{pmatrix}1&-1\\-1&1\end{pmatrix},\qquad A=3P_3+P_1.
$$

Thus $P_3(1,0)^T=(1/2,1/2)^T$ and $P_1(1,0)^T=(1/2,-1/2)^T$: the two pieces add back to $(1,0)^T$. Squaring the matrix simply squares each scalar, $A^2=9P_3+P_1$, and similarly the [matrix exponential](matrix-exponential.md) is $e^{tA}=e^{3t}P_3+e^tP_1$. [Spectral projections of a self-adjoint matrix](spectral-projection-of-a-self-adjoint-matrix.md) turn repeated [matrix](matrix.md) calculations into [scalar](scalar.md) calculations on fixed [vector subspaces](vector-subspace.md).

## ↑ Ancestors (8)

1. [Finite-dimensional spectral theorem](finite-dimensional-spectral-theorem.md)
2. [Self-adjoint operator](self-adjoint-operator.md)
3. [Operator theory](linear-operator-theory-split.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Orthonormal eigenbasis](orthonormal-eigenbasis.md)
