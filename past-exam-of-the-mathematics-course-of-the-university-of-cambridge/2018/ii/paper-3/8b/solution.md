<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

The kinetic energy of the three unit masses is $\frac12\sum_i\dot x_i^2$. Expanding the potential gives

$$
V=\frac12\left(3\sum_{i=1}^3x_i^2-2\sum_{i<j}x_ix_j\right).
$$

Thus the [small-oscillation mass and stiffness matrices](../../../../../small-oscillation-mass-and-stiffness-matrices.md) are

$$
\boxed{
T=I_3,\qquad
V=
\begin{pmatrix}
3&-1&-1\\
-1&3&-1\\
-1&-1&3
\end{pmatrix}
=4I_3-J,
}
$$

where $J$ is the all-ones matrix.

The vector $(1,1,1)^T$ is an [eigenvector](../../../../../eigenvector.md) of the stiffness matrix with [eigenvalue](../../../../../eigenvalue.md) $1$. Every vector orthogonal to it has coordinate sum zero and is an eigenvector with eigenvalue $4$. Since $T=I$, the [generalized eigenvalue problem for small oscillations](../../../../../generalized-eigenvalue-problem-for-small-oscillations.md) gives $\omega^2$ equal to these eigenvalues. One orthonormal choice of [normal modes](../../../../../normal-mode.md) is

$$
\begin{array}{c|c}
\text{mode}&\text{angular frequency}\\ \hline
\dfrac1{\sqrt3}(1,1,1)&1\\[4pt]
\dfrac1{\sqrt2}(1,-1,0)&2\\[4pt]
\dfrac1{\sqrt6}(1,1,-2)&2.
\end{array}
$$

The last two may be replaced by any orthonormal basis of the sum-zero plane because the frequency is degenerate. Hence **the normal frequencies are $\boxed{1,2,2}$.**

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
