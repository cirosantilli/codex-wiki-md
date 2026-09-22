<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Split the [string embedding map](../../../../../string-embedding-map.md) into its constant [worldsheet zero mode](../../../../../worldsheet-zero-mode.md) and orthogonal fluctuations, $X^\mu=x^\mu+X'^\mu$. The kinetic operator has no inverse on the constant mode, while its inverse on $X'$ is the [worldsheet Green function](../../../../../worldsheet-green-function.md) $G$. Completing the square in the [Gaussian functional integral](../../../../../gaussian-functional-integral.md) gives

$$
\int\mathcal DX'\,e^{-S[X']-\int J\cdot X'}
\propto\exp\left(\frac12\int_{\Sigma\times\Sigma}d^2z\,d^2w\,J(z)G(z,w)J(w)\right).
$$

The remaining ordinary integral is

$$
\int d^Dx\,e^{-x^\mu\int_\Sigma d^2zJ_\mu(z)},
$$

which proves (1), up to a source-independent [functional determinant](../../../../../functional-determinant.md).

To insert $n$ [tachyon vertex operators](../../../../../tachyon-vertex-operator.md), choose

$$
J_\mu(z,\bar z)=-i\sum_{j=1}^nk_{j\mu}\delta^{(2)}(z-z_j).
$$

The zero-mode integral produces target-space momentum conservation,

$$
(2\pi)^D\delta^{(D)}\left(\sum_jk_j\right).
$$

In the nonzero-mode integral, discard the coincident self-contractions by [normal ordering](../../../../../normal-ordering.md). With $G(z,w)=-(\alpha'/2)\log|z-w|^2$, the remaining pairwise contractions produce the [Koba-Nielsen factor](../../../../../koba-nielsen-factor.md), so

$$
\boxed{
\left\langle\prod_{j=1}^ne^{ik_j\cdot X(z_j,\bar z_j)}\right\rangle
\propto(2\pi)^D\delta^{(D)}\left(\sum_jk_j\right)
\prod_{i<j}|z_i-z_j|^{\alpha'k_i\cdot k_j}
}.
$$

For three closed-string tachyons on the sphere, $k_i^2=4/\alpha'$ and $\sum_i k_i=0$, hence $\alpha'k_i\cdot k_j=-2$ for $i\ne j$. The matter correlator is therefore $|z_{12}z_{13}z_{23}|^{-2}$. Gauge fixing the sphere's [Möbius transformation](../../../../../mobius-transformation.md) group fixes three insertion points and supplies the [bc ghost system](../../../../../bc-system.md) correlator $|z_{12}z_{13}z_{23}|^2$, exactly cancelling this position dependence. Thus

$$
\boxed{\mathcal A_3=C_{S^2}g_c^3(2\pi)^D\delta^{(D)}(k_1+k_2+k_3)}.
$$

Here each vertex contributes one closed-string coupling $g_c$, $C_{S^2}$ contains the sphere vacuum normalization and conventions, the [worldsheet zero mode](../../../../../worldsheet-zero-mode.md) gives the momentum delta function, the nonzero modes give the [Koba-Nielsen factor](../../../../../koba-nielsen-factor.md), and the ghost determinant divides by the conformal Killing group. Since $C_{S^2}\propto g_s^{-2}$ and $g_c\propto g_s$, the net [string genus expansion](../../../../../string-genus-expansion.md) dependence is $g_s$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 306](../../paper-306-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
