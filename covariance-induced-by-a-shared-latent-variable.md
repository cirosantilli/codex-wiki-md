# Covariance induced by a shared latent variable

↑ **Parent:** [Conditional independence](conditional-independence.md)

Let $A,B$ be [indicator random variables](indicator-random-variable.md) with [conditional independence](conditional-independence.md) given a [latent variable](latent-variable-split.md) $T$, and suppose $\mathbb E[A\mid T]=\mathbb E[B\mid T]=g(T)$. Then

$$
\operatorname{Cov}(A,B)=\operatorname{Var}(g(T))\geq0.
$$

For a short proof, [conditional independence](conditional-independence.md) gives $\mathbb E[AB\mid T]=g(T)^2$. The [law of total expectation](law-of-total-expectation.md) gives $\mathbb E[AB]=\mathbb E[g(T)^2]$ and $\mathbb E[A]=\mathbb E[B]=\mathbb E[g(T)]$. Subtract their product to obtain the claimed [variance](variance-split.md). Since $0\leq g(T)\leq1$, all the required [expected values](expected-value-split.md) exist.

In the two-environment example of [conditional independence](conditional-independence.md), $g(T)$ is $0.1$ or $0.9$ with equal [probabilities](probability.md). Hence $\mathbb E[g(T)]=0.5$ and $\operatorname{Var}(g(T))=((0.1-0.5)^2+(0.9-0.5)^2)/2=0.16$. The two trials have zero [conditional covariance](conditional-covariance.md) in either environment, yet their unconditional [covariance](covariance.md) is positive because their success [probabilities](probability.md) rise and fall together.

More generally, [square-integrable](square-integrable-function.md) [conditionally independent](conditional-independence.md) [random variables](random-variable-split.md) satisfy

$$
\operatorname{Cov}(A,B)
=\operatorname{Cov}\bigl(\mathbb E[A\mid T],\mathbb E[B\mid T]\bigr)
$$

by the [law of total covariance](law-of-total-covariance.md). Equal conditional means reduce this to the displayed [variance](variance-split.md); unequal conditional means need not give a nonnegative [covariance](covariance.md). The equal-mean result explains correlated component evolutionary states in a [coeval binary population](coeval-binary-population.md) without correlation between initial masses: variation in a shared environment can supply the entire [covariance](covariance.md).

## ↑ Ancestors (8)

1. [Conditional independence](conditional-independence.md)
2. [Independent random variables](independent-random-variables.md)
3. [Random variable](random-variable-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Bayes' theorem](bayes-theorem.md)
- [Conditional independence](conditional-independence.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-322/1/iii/solution.md)
