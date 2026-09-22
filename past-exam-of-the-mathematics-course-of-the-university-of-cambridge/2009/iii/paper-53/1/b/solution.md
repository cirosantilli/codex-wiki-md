<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The stated condition is the definition of an [extreme point](../../../../../../extreme-point.md) in the convex set of [density matrices](../../../../../../density-matrix.md). Suppose first that $\rho=|\psi\rangle\langle\psi|$ with $\|\psi\|=1$, and consider any [convex combination](../../../../../../convex-combination.md) $\rho=\sum_i a_i\rho_i$ with all $a_i>0$. For every $|w\rangle$ [orthogonal](../../../../../../orthogonal-vectors.md) to $|\psi\rangle$,

$$
0=\langle w|\rho|w\rangle=\sum_i a_i\langle w|\rho_i|w\rangle.
$$

Every term is nonnegative, so $\langle w|\rho_i|w\rangle=0$ for each $i$. To see that this implies $\rho_iw=0$, expand $\rho_i=\sum_j\mu_j|u_j\rangle\langle u_j|$, $\mu_j\geq0$. The equality $\sum_j\mu_j|\langle u_j|w\rangle|^2=0$ implies $\mu_j\langle u_j|w\rangle=0$ for every $j$, which kills $\rho_iw$. Thus each [density matrix](../../../../../../density-matrix.md) $\rho_i$ vanishes on $\psi^\perp$. By self-adjointness its range lies in the line $\mathbb C\psi$, so $\rho_i=c_i|\psi\rangle\langle\psi|$. Its unit [trace](../../../../../../matrix-trace.md) forces $c_i=1$, establishing the required purity.

Conversely, suppose $\rho$ is not rank one. In its [spectral decomposition](../../../../../../spectral-decomposition.md), at least two [eigenvalues](../../../../../../eigenvalue.md) are positive. Select a normalized eigenvector $|e_1\rangle$ with positive [eigenvalue](../../../../../../eigenvalue.md) $\lambda_1$; then $0<\lambda_1<1$. Define

$$
\sigma=\frac{\rho-\lambda_1|e_1\rangle\langle e_1|}{1-\lambda_1}.
$$

The remaining [eigenvalues](../../../../../../eigenvalue.md) show that $\sigma$ is a [density matrix](../../../../../../density-matrix.md). The decomposition $\rho=\lambda_1|e_1\rangle\langle e_1|+(1-\lambda_1)\sigma$ is a [convex combination](../../../../../../convex-combination.md) of two different [density matrices](../../../../../../density-matrix.md), neither equal to $\rho$. This violates the given purity condition. Hence the [extreme points of the density-operator state space](../../../../../../extreme-points-of-the-density-operator-state-space.md) obey

$$
\boxed{\rho\text{ is pure}\iff\rho=|\psi\rangle\langle\psi|\text{ for a normalized }|\psi\rangle.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
