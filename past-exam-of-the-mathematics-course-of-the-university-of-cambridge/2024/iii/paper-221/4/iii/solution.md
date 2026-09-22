<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Condition on the independent external sample, and abbreviate $\delta_\pi=\widehat\pi_m-\pi$ and $\delta_\mu=\widehat\mu_m-\mu$. Expanding the [plug-in estimator](../../../../../../plug-in-estimator.md) around the true nuisance functions gives

$$
\widehat\beta-\beta
=(\mathbb P_n-P)\{(A-\pi)(Y-\mu)\}
+P(\delta_\pi\delta_\mu)+R_{n,m},
$$

where $\sqrt nR_{n,m}=o_p(1)$ because the two nuisance mean squared errors vanish, the evaluation sample is independent of the nuisance fits, $A$ is bounded, and $Y$ has bounded support. The linear term is the empirical average of the [influence function](../../../../../../influence-function.md), so the [central limit theorem](../../../../../../central-limit-theorem.md) gives

$$
\sqrt n(\mathbb P_n-P)\{(A-\pi)(Y-\mu)\}
\xrightarrow dN(0,\operatorname{Var}\psi).
$$

The remaining bias obeys the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md)

$$
|P(\delta_\pi\delta_\mu)|
\leq\sqrt{\operatorname{MSE}(\widehat\pi_m)
\operatorname{MSE}(\widehat\mu_m)}.
$$

Thus the claimed conclusion follows under the standard product-rate condition

$$
n\operatorname{MSE}(\widehat\pi_m)
\operatorname{MSE}(\widehat\mu_m)\longrightarrow0,
$$

equivalently $\sqrt n\sqrt{\operatorname{MSE}(\widehat\pi_m)operatorname{MSE}(\widehat\mu_m)}\to0$. [Slutsky theorem](../../../../../../slutsky-theorem.md) then yields

$$
\sqrt n(\widehat\beta-\beta)
\xrightarrow dN(0,\operatorname{Var}(\psi(X,A,Y))).
$$

As printed, the paper instead assumes only $\sqrt n\operatorname{MSE}(\widehat\pi_m)\operatorname{MSE}(\widehat\mu_m)\to0$, which is insufficient with its stated definition of MSE. For example, deterministic nuisance errors of size $n^{-3/16}$ have both MSEs equal to $n^{-3/8}$ and satisfy the printed condition, while the scaled product bias is $\sqrt n\,n^{-3/8}=n^{1/8}$. The result therefore requires the stronger condition above, or “MSE” in the printed rate must be read as root mean squared error.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
