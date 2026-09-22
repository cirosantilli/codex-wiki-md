# Trans-dimensional annealing for penalized likelihood

↑ **Parent:** [Reversible-jump Markov chain Monte Carlo](reversible-jump-markov-chain-monte-carlo.md)

To minimize $E_j(\theta)=2k_j-2\ell_j(\theta)$ over models with different parameter dimensions, sample from a target proportional to $w_j e^{-E_j(\theta)/(2T)}$ and cool $T$. A dimension-matching proposal augments the smaller model by auxiliary variables, transforms them bijectively into the larger parameter vector, and includes the proposal [probability density function](probability-density-function.md) and absolute [Jacobian determinant](jacobian-determinant.md) in the [Metropolis–Hastings acceptance probability](metropolis-hastings-acceptance-probability.md). For a positive Poisson [mean](expected-value.md) $\lambda$ and normal parameters $(\mu,v)$, one convenient transformation is

$$
u\sim N(0,\tau^2),\qquad(\mu,v)=(\lambda+u,\lambda),
\qquad(\lambda,u)=(v,\mu-v).
$$

Its absolute [Jacobian determinant](jacobian-determinant.md) is one. If the forward and reverse model-jump selection [probabilities](probability.md) are $b$ and $d$, the Poisson-to-normal ratio is

$$
R=\frac{w_Nd}{w_Pb\,q(u)}
\exp\!\left[-\frac{E_N(\lambda+u,\lambda)-E_P(\lambda)}{2T}\right].
$$

The reverse ratio is its reciprocal at the inverse map. This enforces [detailed balance](detailed-balance.md). When the target is proper and the annealing chain explores it adequately, the low-temperature laws concentrate on the minimum [Akaike information criterion](akaike-information-criterion.md), rather than the maximum marginal model evidence. [Likelihoods](likelihood-function.md) compared across models must describe the same observed data with a compatible reference measure.

**Table of contents**

- [Binomial-normal reversible-jump annealing](binomial-normal-reversible-jump-annealing.md)

## ↑ Ancestors (8)

1. [Reversible-jump Markov chain Monte Carlo](reversible-jump-markov-chain-monte-carlo.md)
2. [Markov chain Monte Carlo](markov-chain-monte-carlo.md)
3. [Bayesian statistics](bayesian-statistics.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47/6/solution.md)
