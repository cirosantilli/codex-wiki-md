# Shared random rate gives dependent point counts

↑ **Parent:** [Constant intensity does not imply independence](constant-intensity-does-not-imply-independence.md)

Draw one [random variable](random-variable-split.md) $R$, taking values zero and two with equal [probabilities](probability.md). Conditional on $R$, generate a [Poisson point process](poisson-point-process-split.md) on the real line with constant rate $R$. This is a [Cox process](cox-process.md) directed by the [random measure](random-measure.md) $R\,dx$: the same rate is shared by every window. It is a locally finite [simple point process](simple-point-process.md) and a [stationary point process](stationary-point-process.md). The [law of total expectation](law-of-total-expectation.md) gives $\mu(A)=\mathbb E[R]|A|=|A|$; the [law of total variance](law-of-total-variance.md) and [law of total covariance](law-of-total-covariance.md) give, for bounded [Borel sets](borel-set.md) $A,B$ with $A\cap B=\varnothing$,

$$
\operatorname{Var}(\Pi(A))=|A|+|A|^2,\qquad
\operatorname{Cov}(\Pi(A),\Pi(B))=|A||B|.
$$

The conditional [covariance](covariance.md) vanishes by [independence](independent-random-variables.md), but the shared conditional means fluctuate together. This distinguishes conditional from unconditional [independence](independent-random-variables.md).[Section 13.2, equation (13.7) and Proposition 13.6, printed p. 130: Cox mean measures and the extra directing-measure variance](lectures-on-the-poisson-process-by-gunter-last-and-others.md)

For a window of length $L$, the exact [probability mass function](probability-mass-function.md) is

$$
\mathbb P(N_W=k)=\frac12\mathbf1_{\{k=0\}}+\frac12 e^{-2L}\frac{(2L)^k}{k!},\qquad k=0,1,2,\ldots.
$$

In particular, its [void probability functional](void-probability-functional.md) is $(1+e^{-2L})/2$, compared with $e^{-L}$ for the unit-rate [Poisson point process](poisson-point-process-split.md). Whole realizations can be empty or comparatively crowded, while their mean density remains one. This example demonstrates shared-rate [statistical dependence](statistical-dependence.md), rather than a model of short-range offspring clusters.

## ↑ Ancestors (8)

1. [Constant intensity does not imply independence](constant-intensity-does-not-imply-independence.md)
2. [Intensity measure of a point process](intensity-measure-of-a-point-process.md)
3. [Point process](point-process.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Constant intensity does not imply independence](constant-intensity-does-not-imply-independence.md)
