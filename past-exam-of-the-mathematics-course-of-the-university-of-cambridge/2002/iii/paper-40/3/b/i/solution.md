<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The order prior and [probabilities](../../../../../../../probability.md) of choosing upward or downward moves are not specified, so include them explicitly. Let $\rho_k$ be the model-order prior [probability](../../../../../../../probability.md), $b_k$ the birth-selection [probability](../../../../../../../probability.md) at order $k$, and $d_{k+1}$ the reverse death-selection [probability](../../../../../../../probability.md). Denote the correctly normalized coefficient prior by $p_k(a)$ and the [probability density function](../../../../../../../probability-density-function.md) of $z\sim N(0,\sigma_a^2)$ by $q(z)$. Common variance-prior factors cancel since $v=\sigma^2$ is unchanged.

Put $m=n^{-1}\sum_i x_i^{k+1}$, $r=y-X_ka$, and $w_i=x_i^{k+1}-m$. The [centered polynomial birth move in reversible-jump sampling](../../../../../../../centered-polynomial-birth-move-in-reversible-jump-sampling.md) gives $X_{k+1}a'=X_ka+zw$, so the residual-sum-of-squares change is

$$
\|r-zw\|^2-\|r\|^2=z^2w^Tw-2zw^Tr.
$$

The map $(a_0,a_1,\ldots,a_k,z)\mapsto(a_0-mz,a_1,\ldots,a_k,z)$ is triangular with [determinant](../../../../../../../determinant.md) one. Thus the [reversible-jump Markov chain Monte Carlo](../../../../../../../reversible-jump-markov-chain-monte-carlo.md) ratio is

$$
R=\frac{\rho_{k+1}d_{k+1}}{\rho_k b_k}\frac{p_{k+1}(a')}{p_k(a)q(z)}\exp\left(\frac{2zw^Tr-z^2w^Tw}{2v}\right),\qquad\alpha_\uparrow=\min(1,R).
$$

For an entirely explicit Gaussian expression, define $Q_k=(a-\mu_k)^T\Sigma_k^{-1}(a-\mu_k)$ and $Q_{k+1}=(a'-\mu_{k+1})^T\Sigma_{k+1}^{-1}(a'-\mu_{k+1})$. Dividing the two normalized Gaussian priors and the proposal [probability density function](../../../../../../../probability-density-function.md) gives

$$
\boxed{\alpha_\uparrow=\min\left\{1,\frac{\rho_{k+1}d_{k+1}}{\rho_kb_k}\sigma_a\sqrt{\frac{|\Sigma_k|}{|\Sigma_{k+1}|}}\exp\left[\frac{2zw^Tr-z^2w^Tw}{2v}-\frac{Q_{k+1}-Q_k}{2}+\frac{z^2}{2\sigma_a^2}\right]\right\}.}
$$

Equal model-order priors and equal birth/death selection [probabilities](../../../../../../../probability.md) remove the first ratio, if that is the intended convention. Dropping the order-dependent normal-prior constants instead would give the wrong acceptance rule.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
