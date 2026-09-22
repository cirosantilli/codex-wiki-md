<h1 id="39c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Since $A$ is diagonalizable over the complex numbers, write $x^{(0)}=\sum_i a_iv_i$. Provided iteration does not encounter zero, its direction is that of

$$
A^kx^{(0)}=\sum_i a_i\lambda_i^kv_i.
$$

With one strictly dominant [eigenvalue](../../../../../../eigenvalue.md) and $a_n\ne0$, all other contributions are smaller by factors $(|\lambda_i|/|\lambda_n|)^k$. The dominant [eigenvalue](../../../../../../eigenvalue.md) is real, since nonreal [eigenvalues](../../../../../../eigenvalue.md) of a real matrix occur in conjugate pairs of equal modulus. The normalized [power method](../../../../../../power-method.md) therefore converges to a signed unit [eigenvector](../../../../../../eigenvector.md) if $\lambda_n>0$, and alternates between opposite unit [eigenvectors](../../../../../../eigenvector.md) if $\lambda_n<0$. A quotient such as $(x^{(k)})^TAx^{(k)}$ approaches $\lambda_n$ in either case. If $a_n=0$, replace it by the largest active modulus; if $Ax^{(k)}=0$, the prescribed iteration is undefined.

With two dominant [eigenvalues](../../../../../../eigenvalue.md) of equal modulus and both components active, the iterates approach their real invariant plane rather than one direction. Distinct real equal-modulus [eigenvalues](../../../../../../eigenvalue.md) are $\rho,-\rho$ and produce a limiting two-cycle. A conjugate pair $\rho e^{\pm i\theta}$ produces a rotation in suitable coordinates on that plane: the normalized directions are periodic when the angle is rational relative to $2\pi$ and otherwise generally keep rotating without convergence. If the two [eigenvalues](../../../../../../eigenvalue.md) are equal and real, the initial projection is itself one [eigenvector](../../../../../../eigenvector.md) in their repeated eigenspace, and converges or alternates as in the single-value case; one orbit cannot recover every [independent](../../../../../../independent-random-variables.md) [eigenvector](../../../../../../eigenvector.md) of that eigenspace.

For distinct dominant values, retain unnormalized consecutive vectors $y,Ay,A^2y$ in the nearly invariant plane and solve

$$
A^2y=sAy-py.
$$

The roots of $\lambda^2-s\lambda+p$ estimate the two [eigenvalues](../../../../../../eigenvalue.md). Corresponding [eigenvectors](../../../../../../eigenvector.md) are $Ay-\lambda_2y$ and $Ay-\lambda_1y$, since applying $A$ and using the recurrence multiplies them by $\lambda_1$ and $\lambda_2$. This is [dominant eigenpair extraction from a two-step Krylov recurrence](../../../../../../dominant-eigenpair-extraction-from-a-two-step-krylov-recurrence.md). Equivalent extraction uses the $2\times2$ matrix of $A$ on the computed plane. It needs two [independent](../../../../../../independent-random-variables.md) iterates and nonzero projections onto both distinct [eigenvectors](../../../../../../eigenvector.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [39C](../../39c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
