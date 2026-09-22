<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $T_i$ be an event time and $C_i$ a potential censoring time. Under [independent censoring](../../../../../independent-censoring.md), observe $Y_i=\min(T_i,C_i)$ and $\delta_i=\mathbf1\{T_i\leq C_i\}$. For an [exponential distribution](../../../../../exponential-distribution.md) of rate $\theta$, an observed failure contributes $\theta e^{-\theta Y_i}$ to the [survival likelihood](../../../../../survival-likelihood.md), whereas a [right-censored](../../../../../right-censoring.md) observation contributes $e^{-\theta Y_i}$. The censoring-law factors may be discarded when they are independent of $\theta$. Thus, writing $d=\sum_i\delta_i$ and $V=\sum_iY_i$ for total observed [person-time](../../../../../person-time.md),

$$
L(\theta)\propto\theta^d e^{-\theta V},\qquad
\ell'(\theta)=\frac d\theta-V,\qquad
\ell''(\theta)=-\frac d{\theta^2}.
$$

For $d,V>0$ the unique [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md) is

$$
\boxed{\widehat\theta=\frac dV.}
$$

Censored times belong in $V$: they record time during which failure was not observed. With $d=0$ and $V>0$, the [likelihood](../../../../../likelihood-function.md) decreases with $\theta$, so the supremum is at the boundary $\theta\downarrow0$; there is no positive interior estimate. This is [exponential-rate estimation from censored exposure](../../../../../exponential-rate-estimation-from-censored-exposure.md).

[Uninformative censoring](../../../../../independent-censoring.md) means that the potential censoring time supplies no information about the latent failure time after conditioning on the modeled variables. A study ending at a fixed follow-up duration independent of prognosis is an example of [administrative censoring](../../../../../administrative-censoring.md). [Informative censoring](../../../../../informative-censoring.md) occurs, for example, when a seriously deteriorating patient withdraws because of that deterioration and the prognostic information is omitted from the model. Under [informative censoring](../../../../../informative-censoring.md), those remaining in the [risk set](../../../../../risk-set.md) are selected by their future failure propensity, so the ordinary [survival likelihood](../../../../../survival-likelihood.md) and its estimate need not target the true rate.

Using the reported durations and flags as though they were valid [right-censored](../../../../../right-censoring.md) records gives

$$
\boxed{\widehat\theta_{\rm labelled}=\frac{500}{1031.6}\simeq0.48468.}
$$

Treating all durations as failures instead gives

$$
\boxed{\widehat\theta_{\rm complete}=\frac{1000}{1031.6}\simeq0.96937.}
$$

Relabelling has halved the event count without shortening any observed follow-up. The resulting estimate is therefore exactly half the complete-data estimate.

**This is not a simulation of uninformative ordinary right-censoring.** For a record declared censored at $Y_i$, ordinary [right censoring](../../../../../right-censoring.md) requires $T_i>Y_i$; the construction instead took $Y_i$ to be the simulated failure time itself. Keeping a failure time and hiding only its flag does not produce the minimum of that time and an independent earlier censoring time. Even choosing labels at random does not fix this: independence of a flag from the recorded duration is different from [independent censoring](../../../../../independent-censoring.md) of a latent event time. Indeed the labelled durations still have mean one while the failure fraction is one half, so their ordinary censored estimate converges to $1/2$, not the generating rate one. Thus it is not a valid uninformative censoring scheme for the intended failure distribution; strictly, it has not implemented ordinary right-censoring of those simulated failure times at all. One could reproduce the randomly labelled record distribution with independent latent event and censoring times both of rate $1/2$, but that would be a different failure model, not the claimed rate-one model. Calling the flags random is therefore insufficient to justify the target distribution or its censored likelihood. This is the [random relabelling is not independent right censoring](../../../../../random-relabelling-is-not-independent-right-censoring.md) issue.

A valid simulation draws independently $T\sim\operatorname{Exp}(1)$ and $C\sim\operatorname{Exp}(1)$, and records $(\min(T,C),\mathbf1\{T\leq C\})$. Since

$$
\Pr(C<T)=\int_0^\infty e^{-c}e^{-c}\,dc=\frac12,
$$

it gives [independent censoring](../../../../../independent-censoring.md) with the requested probability. Equivalently generate $T=-\log U$ and $C=-\log V$ from independent uniform random numbers. Another valid choice is fixed censoring at $\log2$, since $\Pr(T>\log2)=1/2$. These give a random censored fraction with expectation one half; they do not promise exactly 500 censored records. For the independent-exponential scheme, observed durations have rate two and mean one half, so $d/\sum Y_i$ correctly converges to one.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 37](../../paper-37-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
