<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $s=\sigma^2$ and $\vartheta=(s,\tau_1,\ldots,\tau_m)$. With [conditional independence](../../../../../../conditional-independence.md) of the binary observations given the latent [function](../../../../../../function-split.md), define

$$
L(\vartheta)=\int\ell(F)\varphi_{C_\vartheta}(F)\,dF,
\qquad \ell(F)=\prod_{i=1}^n\Phi((2y_i-1)F_i).
$$

The [prior distribution](../../../../../../prior-probability.md) is specified on the precision $s^{-1}$, not on $s$. Its [Jacobian determinant](../../../../../../jacobian-determinant.md) gives

$$
p(\vartheta)=s^{-2}e^{-1/s}\prod_{j=1}^m e^{-\tau_j},\qquad s>0,\ \tau_j>0,
$$

and the marginal [posterior density](../../../../../../posterior-density.md) is proportional to $p(\vartheta)L(\vartheta)$. Working instead with precision or logarithmic coordinates is possible, provided all corresponding [Jacobian determinants](../../../../../../jacobian-determinant.md) are included.

Choose an [importance sampling](../../../../../../importance-sampling.md) density $g_\vartheta$ covering the support of $\ell(F)\varphi_{C_\vartheta}(F)$, draw $F_1,\ldots,F_M$ independently from it, and use the nonnegative [unbiased likelihood estimator](../../../../../../unbiased-likelihood-estimator.md)

$$
\widehat L(\vartheta)=\frac1M\sum_{j=1}^M
\frac{\ell(F_j)\varphi_{C_\vartheta}(F_j)}{g_\vartheta(F_j)}.
$$

Each summand integrates to $L(\vartheta)$, proving unbiasedness. A simple always-valid choice is the latent Gaussian [prior distribution](../../../../../../prior-probability.md), $g_\vartheta=\varphi_{C_\vartheta}$, when the [covariance matrix](../../../../../../covariance-matrix.md) is nonsingular. Then the estimator is just the average of the bounded values $\ell(F_j)\in(0,1)$. For duplicate inputs, sample only the distinct latent values and multiply all likelihood contributions at each common input. A Gaussian approximation to the latent [posterior distribution](../../../../../../bayesian-posterior.md), or its mixture with the Gaussian [prior distribution](../../../../../../prior-probability.md), can reduce relative [variance](../../../../../../variance-split.md) while keeping complete support. Its approximation does not replace the exact weights.

The [pseudo-marginal Metropolis–Hastings algorithm](../../../../../../pseudo-marginal-metropolis-hastings-algorithm.md) stores both the current $\vartheta$ and its estimator randomness $u$; write their sampling law as $m_\vartheta(u)$. Propose $\vartheta'\sim q(\vartheta,\cdot)$, independently generate $u'\sim m_{\vartheta'}$, compute $\widehat L(\vartheta',u')$, and accept the pair with

$$
\boxed{\alpha=1\wedge
\frac{p(\vartheta')\widehat L(\vartheta',u')q(\vartheta',\vartheta)}
{p(\vartheta)\widehat L(\vartheta,u)q(\vartheta,\vartheta')}.}
$$

Here $q(\vartheta,\vartheta')$ denotes the proposal [probability density function](../../../../../../probability-density-function.md) from $\vartheta$ to $\vartheta'$. On rejection retain both the old parameter and the old likelihood estimate. Initialize with a positive estimate. One must not independently refresh the denominator after rejection.

Correctness follows from the extended [posterior density](../../../../../../posterior-density.md)

$$
\widetilde\pi(\vartheta,u)\propto
p(\vartheta)\widehat L(\vartheta,u)m_\vartheta(u).
$$

The pair proposal is $q(\vartheta,\vartheta')m_{\vartheta'}(u')$. Its [Metropolis–Hastings acceptance probability](../../../../../../metropolis-hastings-acceptance-probability.md) simplifies to the displayed ratio, since the auxiliary densities cancel. Hence [detailed balance](../../../../../../detailed-balance.md) holds for $\widetilde\pi$. Integrating over $u$ gives $p(\vartheta)L(\vartheta)$ by unbiasedness, so the parameter [marginal distribution](../../../../../../marginal-distribution.md) is exactly the intended [posterior distribution](../../../../../../bayesian-posterior.md) for any fixed positive $M$. This is exactness of the stationary target, not independent exact samples or a guarantee of rapid convergence. Large relative [variance](../../../../../../variance-split.md) of the likelihood estimates can produce long holding times, so marginalizing $F$ does not by itself guarantee an improvement in [mixing time](../../../../../../mixing-time-of-a-markov-chain.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
