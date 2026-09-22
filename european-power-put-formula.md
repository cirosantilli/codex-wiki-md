# European power put formula

↑ **Parent:** [Power put option](power-put-option.md)

In the dividend-free [Black-Scholes model](black-scholes-model.md), let $\tau=T-t>0$, $K>0$, $S>0$, $\sigma>0$ and

$$
d_j=\frac{\log(S/K)+[r+(j-\tfrac12)\sigma^2]\tau}{\sigma\sqrt\tau}.
$$

Then the displayed [finite sum](finite-sum.md) prices the [European option](european-contingent-claim.md) with [power put option](power-put-option.md) payoff. Here $\Phi$ is the [standard normal distribution function](standard-normal-distribution-function.md). Indeed, $\log S_T$ conditionally has a [normal distribution](normal-distribution.md) with mean $\log S+(r-\sigma^2/2)\tau$ and [variance](variance-split.md) $\sigma^2\tau$. Expand $(K-S_T)^n$ by the [binomial theorem](binomial-theorem.md) on $S_T<K$ and apply the lower [truncated lognormal moment](truncated-lognormal-moment.md) to each term. Equivalently,

$$
P_n=e^{-r\tau}\mathbb E[(K-SY)_+^n],\qquad Y=\exp[(r-\sigma^2/2)\tau+\sigma\sqrt\tau Z],\quad Z\sim N(0,1).
$$

This [expectation](expected-value-split.md) representation proves monotonicity and convexity in $S$. It also gives $P_n(0,t)=K^ne^{-r\tau}$ and $P_n(S,t)\to0$ as $S\to\infty$ by the [dominated convergence theorem](dominated-convergence-theorem.md). For positive $S$ the [lognormal distribution](log-normal-distribution.md) smoothing makes the price smooth and strictly positive.

## ↑ Ancestors (9)

1. [Power put option](power-put-option.md)
2. [Put option](put-option.md)
3. [Contingent claim](contingent-claim.md)
4. [Fundamental theorem of asset pricing](fundamental-theorem-of-asset-pricing-split.md)
5. [Mathematical finance](mathematical-finance-split.md)
6. [Mathematical optimization](mathematical-optimization-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford/2023/2/b/i/solution.md)
- [Truncated lognormal moment](truncated-lognormal-moment.md)
