<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [reversible-jump Markov chain Monte Carlo](../../../../../../../reversible-jump-markov-chain-monte-carlo.md) calculation compares normalized model-specific densities. The fixed-order posterior written only up to proportionality in part (a) omits normalizing factors that depend on $k$ and therefore cannot simply be canceled between dimensions. Moreover, the printed question does not specify the model-order [prior distribution](../../../../../../../prior-probability.md) or the probabilities of selecting birth and death moves. Denote those by $p_k$, $b_k$ and $d_k$, respectively, retaining them in the answer.

Put $s=\sigma^2$, $c=n^{-1}\sum_i x_i^{k+1}$, $v_i=x_i^{k+1}-c$, and $r=y-X_k\beta$. The [centered polynomial birth move in reversible-jump sampling](../../../../../../../centered-polynomial-birth-move-in-reversible-jump-sampling.md) changes the fitted vector by $zv$, so its new residual is $r'=r-zv$. Therefore

$$
\|r'\|^2-\|r\|^2=-2zv^Tr+z^2v^Tv.
$$

The map from $(\beta_0,\ldots,\beta_k,z)$ to $(\beta'_0,\ldots,\beta'_{k+1})$ has ones down the diagonal and a single additional entry $-c$ in the intercept row. Its [Jacobian determinant](../../../../../../../jacobian-determinant.md) is one.

Write $Q_k=(\beta-\mu_k)^T\Sigma_k^{-1}(\beta-\mu_k)$ and $Q_{k+1}=(\beta'-\mu_{k+1})^T\Sigma_{k+1}^{-1}(\beta'-\mu_{k+1})$. The normalized [multivariate normal distribution](../../../../../../../multivariate-normal-distribution.md) prior ratio is

$$
\frac{\pi_{k+1}(\beta')}{\pi_k(\beta)}
=(2\pi)^{-1/2}\sqrt{\frac{|\Sigma_k|}{|\Sigma_{k+1}|}}
 \exp\left[-\tfrac12(Q_{k+1}-Q_k)\right].
$$

Divide also by the forward proposal density $q(z)=(2\pi\sigma_\beta^2)^{-1/2}e^{-z^2/(2\sigma_\beta^2)}$. The common [inverse-gamma distribution](../../../../../../../inverse-gamma-distribution.md) prior for $s$ and the common normal-likelihood normalization cancel, since $s$ stays fixed. The forward acceptance ratio is consequently

$$
R_+=\frac{p_{k+1}d_{k+1}}{p_kb_k}\,
\sigma_\beta\sqrt{\frac{|\Sigma_k|}{|\Sigma_{k+1}|}}
\exp\left[
\frac{zv^Tr-z^2v^Tv/2}{s}
-\frac{Q_{k+1}-Q_k}{2}
+\frac{z^2}{2\sigma_\beta^2}
\right],\qquad
\boxed{A_+=\min(1,R_+).}
$$

Here $\sigma_\beta>0$ is the proposal standard deviation. If equal model priors and symmetric birth/death selection are explicitly adopted, their ratios become one; they are not determined by the PDF. The expression assumes the same hyperparameters for the variance prior in both models, as in part (a). A dimension-dependent variance prior would contribute its own ratio.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
