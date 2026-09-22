# Moment matching for a beta prior

↑ **Parent:** [Beta distribution](beta-distribution.md)

[Moment matching for a beta prior](moment-matching-for-a-beta-prior.md) turns a desired [mean](expected-value-split.md) and [variance](variance-split.md) for an unknown [probability](probability.md) into the parameters of a [beta distribution](beta-distribution.md) [prior](prior-probability.md). Choose $0<m<1$ and

$$
0<v<m(1-m).
$$

Solving the [beta distribution](beta-distribution.md) [mean](expected-value-split.md) and [variance](variance-split.md) identities gives

$$
\kappa=\frac{m(1-m)}v-1,\qquad\alpha=m\kappa,\qquad\beta=(1-m)\kappa.
$$

The strict upper bound on the [variance](variance-split.md) makes $\kappa>0$, so both parameters are positive. Substitution gives [mean](expected-value-split.md) $\mathbb E[P]=m$ and [variance](variance-split.md) $\operatorname{Var}(P)=v$ exactly. A smaller specified [variance](variance-split.md) at fixed [mean](expected-value-split.md) produces a more concentrated [prior distribution](prior-probability.md).

For example, a desired [prior](prior-probability.md) [mean](expected-value-split.md) $m=0.3$ and [variance](variance-split.md) $v=0.01$ give $\kappa=0.21/0.01-1=20$, hence the [beta distribution](beta-distribution.md) [prior](prior-probability.md) $\operatorname{Beta}(6,14)$. With the same [mean](expected-value-split.md) and [variance](variance-split.md) $v=0.035$, the calculation instead gives $\kappa=5$ and the broader [beta distribution](beta-distribution.md) [prior](prior-probability.md) $\operatorname{Beta}(1.5,3.5)$. Both appear in the concentration diagram above.

The excluded boundary cases have clear meanings. Zero [variance](variance-split.md) would require $P=m$ with certainty, not a [beta distribution](beta-distribution.md) with finite positive parameters. At the other boundary, any [random variable](random-variable-split.md) $P\in[0,1]$ satisfies $P^2\leq P$, hence [variance](variance-split.md) at most $m(1-m)$; equality requires $P$ to take only the endpoint values zero and one. This is a [Bernoulli distribution](bernoulli-distribution.md), not a [beta distribution](beta-distribution.md). Thus $v\geq m(1-m)$ cannot be matched by positive finite parameters, and $m=0$ or $m=1$ is also excluded.

After observing $n=h+t>0$ [Bernoulli trials](bernoulli-trial.md), the [Beta-binomial conjugacy](beta-binomial-conjugacy.md) makes the [posterior](bayesian-posterior.md) [mean](expected-value-split.md) a weighted average of the [prior](prior-probability.md) [mean](expected-value-split.md) $m$ and observed [binomial proportion](binomial-proportion.md) $h/n$:

$$
\mathbb E[P\mid h,t]=\frac{\alpha+h}{\kappa+n}=\frac{\kappa}{\kappa+n}m+\frac{n}{\kappa+n}\frac hn.
$$

This formula gives $\kappa$ a precise interpretation as the [prior](prior-probability.md)'s weight relative to the [sample size](sample-size.md) in this [posterior](bayesian-posterior.md) [mean](expected-value-split.md). It does not require fictitious observed counts: the [beta distribution](beta-distribution.md) parameters can be any positive real numbers. For the eight-head, two-tail example above, $\kappa=4$ and $m=1/2$, so the [posterior](bayesian-posterior.md) [mean](expected-value-split.md) is $(4\cdot1/2+10\cdot0.8)/14=5/7$.

// Target: statistical-inference.bigb

## ↑ Ancestors (7)

1. [Beta distribution](beta-distribution.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Moment matching for a beta prior](moment-matching-for-a-beta-prior.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/4/i/solution.md)
- [Prior probability](prior-probability.md)
