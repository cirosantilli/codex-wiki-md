# Total correlation

↑ **Parent:** [Information theory](information-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Total_correlation)

[Total correlation](total-correlation.md) measures how much dependence is lost when a joint [probability distribution](probability-distribution-split.md) is replaced by the product of its marginal [probability distributions](probability-distribution-split.md). It compares the uncertainty of the separate coordinates with the uncertainty of the whole [random vector](random-vector.md). The distinction matters because an exact relation can involve three variables while leaving every pair [independent](independent-random-variables.md).

For [random variables](random-variable-split.md) $X_1,\ldots,X_n$ with finite [alphabets](alphabet.md), define

$$
\boxed{\operatorname{TC}(X_1,\ldots,X_n)
=\sum_{i=1}^n H(X_i)-H(X_1,\ldots,X_n)
=D\!\left(P_{X_1,\ldots,X_n}\middle\Vert\bigotimes_{i=1}^n P_{X_i}\right).}
$$

Here $H$ is [information entropy](information-entropy-split.md), the entropy of the full [random vector](random-vector.md) is [joint entropy](joint-entropy.md), and $D$ is [relative entropy](kullback-leibler-divergence.md). Base-two [logarithms](logarithm.md) give [bits](bit.md); [natural logarithms](natural-logarithm.md) give [nats](nat-unit.md). The product law retains every marginal [probability distribution](probability-distribution-split.md) but discards their dependence.[Abstract, printed p. 66: total correlation for the partition into individual variables](information-theoretical-analysis-of-multivariate-correlation-by-satosi-watanabe.md) A positive joint [probability](probability.md) guarantees positive marginal [probabilities](probability.md) at that outcome, so the displayed [relative entropy](kullback-leibler-divergence.md) is finite in this finite-alphabet setting.

For two variables, [total correlation](total-correlation.md) is exactly [mutual information](mutual-information.md). For three or more, it can detect a constraint that all pairwise [mutual informations](mutual-information.md) miss. [Relative entropy nonnegativity](relative-entropy-nonnegativity.md) gives $\operatorname{TC}\geq0$, with equality exactly when the coordinates are jointly [independent random variables](independent-random-variables.md).

As the simplest contrast, three [independent](independent-random-variables.md) fair [bits](bit.md) have three [bits](bit.md) of [joint entropy](joint-entropy.md) and zero [total correlation](total-correlation.md). If all three coordinates instead copy the same fair [bit](bit.md), their separate [information entropies](information-entropy-split.md) still sum to three [bits](bit.md), but their [joint entropy](joint-entropy.md) is only one [bit](bit.md). Their [total correlation](total-correlation.md) is therefore two [bits](bit.md). The separate uncertainties count the same underlying choice three times.

**Table of contents**

- [Parity constraint and total correlation](parity-constraint-and-total-correlation.md)
  - [Noisy parity total correlation](noisy-parity-total-correlation.md)
- [Chain decomposition of total correlation](chain-decomposition-of-total-correlation.md)
- [Relative entropy to a product law](relative-entropy-to-a-product-law.md)
- [Scope and scale of total correlation](scope-and-scale-of-total-correlation.md)
- [Historical source for total correlation](historical-source-for-total-correlation.md)

## ↑ Ancestors (5)

1. [Information theory](information-theory-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Chain decomposition of total correlation](chain-decomposition-of-total-correlation.md)
- [Joint entropy](joint-entropy.md)
- [Noisy parity total correlation](noisy-parity-total-correlation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-224/4/a/solution.md)
- [Poisson approximation bound for dependent Bernoulli variables](poisson-approximation-bound-for-dependent-bernoulli-variables.md)
- [Relative entropy to a product law](relative-entropy-to-a-product-law.md)
- [Scope and scale of total correlation](scope-and-scale-of-total-correlation.md)
- [Total correlation](total-correlation.md)
