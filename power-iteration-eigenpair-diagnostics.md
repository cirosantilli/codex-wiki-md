# Power iteration eigenpair diagnostics

↑ **Parent:** [Power iteration](power-iteration.md)

For each [unit vector](unit-vector.md) iterate compute the [Rayleigh quotient](rayleigh-quotient.md) $\rho_k=x_k^*Ax_k$ and the [eigenpair residual](eigenpair-residual.md) $r_k=Ax_k-\rho_kx_k$. Use the same multiplication $Ax_k$ for both diagnostics and the next normalized iterate. For any complex [matrix](matrix.md), this [Rayleigh quotient](rayleigh-quotient.md) minimizes $\|Ax_k-\mu x_k\|_2$ over complex [scalars](scalar.md) $\mu$, because $x_k^*r_k=0$. Under [power iteration convergence for a diagonalizable matrix](power-iteration-convergence-for-a-diagonalizable-matrix.md), $\rho_k\to\lambda_1$ and $\|r_k\|_2\to0$, even when the [vectors](vector.md) alternate signs or phases.[§3, PDF p. 3: approximate eigenvector equation and Rayleigh quotient](numerical-analysis-spring-2022/power-iteration-2022-03-07-lecture-notes.md)

A dimensionless stopping quantity is

$$
\eta_k=\frac{\|r_k\|_2}{\|A\|_2+|\rho_k|},
$$

when the denominator is positive; $\|A\|_2$ is the [operator norm](operator-norm.md), and a known upper bound may replace it if computing it is costly. A small [eigenpair residual](eigenpair-residual.md) certifies a small [backward error of an approximate eigenpair](backward-error-of-an-approximate-eigenpair.md), but does not establish that the [eigenvalue](eigenvalue.md) found is dominant.

For a [Hermitian matrix](hermitian-operator.md) with [orthonormal eigenbasis](orthonormal-eigenbasis.md) $u_j$, write $x_k=\sum_j a_ju_j$. Then the independently useful identity

$$
\|r_k\|_2^2=\sum_j|a_j|^2|\lambda_j-\rho_k|^2
$$

shows that some [eigenvalue](eigenvalue.md) lies within $\|r_k\|_2$ of $\rho_k$. If a specific target [eigenvalue](eigenvalue.md) $\lambda_1$ is separated from all the others by $\delta_k=\min_{j>1}|\lambda_j-\rho_k|>0$, it also gives $\varepsilon_k\le\|r_k\|_2/\delta_k$. This separation is measured from the computed [Rayleigh quotient](rayleigh-quotient.md); it differs from the dominant-[modulus](modulus.md) [spectral gap](spectral-gap.md). For a [nonnormal matrix](non-normal-matrix.md), the same [orthogonal](orthogonal-vectors.md) expansion is unavailable and a small [eigenpair residual](eigenpair-residual.md) alone need not imply a comparably small distance to the [spectrum](spectrum-functional-analysis.md).

## ↑ Ancestors (7)

1. [Power iteration](power-iteration.md)
2. [Numerical linear algebra](numerical-linear-algebra-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
