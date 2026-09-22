<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $t_i=x_i^T\beta$ and $s_i=2Y_i-1\in\{-1,1\}$. The [probit regression](../../../../../../probit-model.md) likelihood is $\prod_i\Phi(s_it_i)$, so with the stated normal prior,

$$
\log p(\beta\mid Y)=\text{constant}-\frac{\|\beta\|^2}{2\sigma^2}+\sum_i\log\Phi(s_ix_i^T\beta).
$$

Differentiating gives the [probit posterior score](../../../../../../probit-posterior-score.md)

$$
\boxed{g(\beta)=-\frac\beta{\sigma^2}+\sum_i s_ix_i\frac{\phi(s_ix_i^T\beta)}{\Phi(s_ix_i^T\beta)}.}
$$

Equivalently, the $i$th likelihood term is $x_i\phi(t_i)[Y_i/\Phi(t_i)-(1-Y_i)/(1-\Phi(t_i))]$. The prior's gradient is essential.

This [posterior density](../../../../../../posterior-density.md) is smooth, positive everywhere, and bounded above by a constant times the Gaussian prior, since the likelihood is at most one and has positive normalizing constant. Its derivatives are integrable: differentiating a likelihood factor gives a bounded normal density, and differentiating the prior gives a linear factor times a Gaussian. Integration by parts therefore yields

$$
\mathbb E[g_j(\beta)\mid Y]=\int_{\mathbb R^p}\partial_jp(\beta\mid Y)\,d\beta=0.
$$

Thus each component has a known zero [expected value](../../../../../../expected-value.md) and can be used as a [posterior score control variate](../../../../../../posterior-score-control-variate.md). This identity differentiates the posterior density in the random parameter; it is distinct from the usual [mean-zero score identity](../../../../../../mean-zero-score-identity.md) for a likelihood under repeated sampling.

The requisite second moments are finite. For $t\geq0$, $\phi(t)/\Phi(t)$ is bounded. For $t<0$,

$$
\Phi(t)\geq\int_{t-1}^t\phi(u)\,du\geq\phi(t-1),\qquad
\frac{\phi(t)}{\Phi(t)}\leq e^{-t+1/2}.
$$

Hence the score grows at most exponentially in $\|\beta\|$, and the Gaussian upper bound on the posterior gives finite second moments. For a fixed vector $a$, averaging $h(\beta)-a^Tg(\beta)$ is therefore an unbiased [Monte Carlo estimator](../../../../../../monte-carlo-estimator.md) of the same mean; suitable coefficients can reduce its [variance](../../../../../../variance-split.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
