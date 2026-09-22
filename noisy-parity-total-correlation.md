# Noisy parity total correlation

↑ **Parent:** [Parity constraint and total correlation](parity-constraint-and-total-correlation.md)

Keep $X,Y$ as [independent](independent-random-variables.md) fair [bits](bit.md), introduce an [independent](independent-random-variables.md) [Bernoulli random variable](bernoulli-distribution.md) $N$ with $\mathbb P(N=1)=\varepsilon$, and set $Z=X\mathbin\oplus Y\mathbin\oplus N$. The extra [bit](bit.md) flips the [integer parity](parity-mathematics.md) rule with [probability](probability.md) $\varepsilon$. For each even-[integer parity](parity-mathematics.md) triple the [probability](probability.md) is $(1-\varepsilon)/4$; for each odd-[integer parity](parity-mathematics.md) triple it is $\varepsilon/4$.

Every coordinate remains fair, and every pair remains [independent](independent-random-variables.md) for every $0\leq\varepsilon\leq1$. For example, after fixing $X$, the fair independent $Y$ makes $Y\mathbin\oplus N$ fair regardless of $\varepsilon$. A pair's [joint probability distribution](joint-probability-distribution.md) therefore does not change as noise destroys the three-way relation.

<a id="image-noise-changes-the-joint-parity-distribution-without-changing-any-pair-s-independence"></a>
![](total-correlation-noisy-parity-distributions.png)

**[Figure 11](#image-noise-changes-the-joint-parity-distribution-without-changing-any-pair-s-independence). Noise changes the joint parity distribution without changing any pair's independence**. Calculated [probability mass functions](probability-mass-function.md) for the stipulated three-[bit](bit.md) model at $\varepsilon=0,1/4,1/2$. Even-[integer parity](parity-mathematics.md) and odd-[integer parity](parity-mathematics.md) triples have different colors. The dashed line is the product of the three fair marginal [probability distributions](probability-distribution.md). These are theoretical [probabilities](probability.md), not measurements.

Knowing $X,Y$, uncertainty in $Z$ is exactly the uncertainty in $N$. The [chain rule for information entropy](chain-rule-for-information-entropy.md) gives

$$
H(X,Y,Z)=H(X,Y)+H(Z\mid X,Y)=2+h_2(\varepsilon),
$$

where $h_2$ is [binary entropy](binary-entropy.md). Hence

$$
\boxed{\operatorname{TC}(X,Y,Z)=1-h_2(\varepsilon).}
$$

At $\varepsilon=1/4$, the result is approximately $0.188722$ [bits](bit.md), although all three pairwise [mutual informations](mutual-information.md) are zero. At $\varepsilon=1/2$, all eight triples have [probability](probability.md) $1/8$, giving joint [independence](independent-random-variables.md) and zero [total correlation](total-correlation.md). At $\varepsilon=1$, the complementary [integer parity](parity-mathematics.md) rule is deterministic again, so [total correlation](total-correlation.md) returns to one [bit](bit.md).

<a id="image-total-correlation-detects-a-noisy-three-way-constraint-missed-by-pairwise-mutual-information"></a>
![](total-correlation-parity-noise-and-pairwise-information.png)

**[Figure 12](#image-total-correlation-detects-a-noisy-three-way-constraint-missed-by-pairwise-mutual-information). Total correlation detects a noisy three-way constraint missed by pairwise mutual information**. The exact formula $1-h_2(\varepsilon)$ for the stipulated [noisy parity total correlation](noisy-parity-total-correlation.md), plotted over $0\leq\varepsilon\leq1/2$. The [mutual information](mutual-information.md) of each pair is identically zero; joint [independence](independent-random-variables.md) occurs only at the right endpoint of this interval.

The example distinguishes "there is a dependence" from "a pair reveals it." Once $X,Y$ are known together, $Z$ is predictable at zero noise; knowing either one alone leaves a fair [bit](bit.md). [Total correlation](total-correlation.md) detects the joint departure from [independence](independent-random-variables.md), but does not by itself specify which variables cause which others.

## ↑ Ancestors (7)

1. [Parity constraint and total correlation](parity-constraint-and-total-correlation.md)
2. [Total correlation](total-correlation.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Joint entropy](joint-entropy.md)
- [Noisy parity total correlation](noisy-parity-total-correlation.md)
