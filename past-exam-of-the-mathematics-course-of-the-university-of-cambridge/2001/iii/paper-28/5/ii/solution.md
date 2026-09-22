<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the standard additive [multinomial logistic regression](../../../../../../multinomial-logistic-regression.md), use the final satisfaction category as baseline and write

$$
\log\frac{p_{ijkl}}{p_{ijkL}}=\alpha_l+a_{il}+b_{jl}+c_{kl},\qquad l<L.
$$

Set a reference effect to zero for each covariate factor. Define $\eta_{ijkl}=\alpha_l+a_{il}+b_{jl}+c_{kl}$ for $l<L$, and $\eta_{ijkL}=0$. The probabilities are

$$
p_{ijkl}=\frac{e^{\eta_{ijkl}}}{\sum_me^{\eta_{ijkm}}}.
$$

Substitution into the conditional [log-likelihood](../../../../../../log-likelihood.md) gives

$$
\ell=\sum_{l<L}\left[\alpha_ln_{+++l}+\sum_i a_{il}n_{i++l}+\sum_jb_{jl}n_{+j+l}+\sum_kc_{kl}n_{++kl}\right]-\sum_{ijk}N_{ijk}\log\sum_me^{\eta_{ijkm}}+\log h(n).
$$

The second term depends on the parameters and the fixed stratum totals, not on any additional within-stratum cell allocation. The [Fisher-Neyman factorization theorem](../../../../../../fisher-neyman-factorization-theorem.md) therefore proves that

$$
\boxed{(n_{+++l},n_{i++l},n_{+j+l},n_{++kl})_{l<L}\text{ are sufficient for the additive multinomial-logit model}.}
$$

These margins contain linear redundancies; after reference constraints an equivalent independent statistic has dimension

$$
(L-1)[1+(I-1)+(J-1)+(K-1)]=2(1+2+3+1)=14.
$$

Hence its residual degrees of freedom are $24(3-1)-14=34$. In the equivalent [Poisson surrogate for a conditional multinomial model](../../../../../../poisson-surrogate-for-a-conditional-multinomial-model.md), include a separate stratum intercept $\gamma_{ijk}$ and response interactions with each individual covariate. The 24 nuisance intercepts plus 14 response parameters give 38 parameters in 72 Poisson cells, again 34 residual degrees of freedom. Since the stratum totals are fixed in the conditional experiment, they need not be included as random sufficient statistics there; they do belong to the unconditional Poisson model's sufficient margins.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
