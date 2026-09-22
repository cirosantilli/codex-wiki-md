# Hoeffding sample size for Bernoulli frequencies

↑ **Parent:** [Hoeffding inequality](hoeffding-inequality.md)

Let $B_1,\ldots,B_n$ be [independent and identically distributed](independent-and-identically-distributed-random-variables.md) [Bernoulli random variables](bernoulli-distribution.md) with success [probability](probability.md) $p$, and let $\widehat p_n=n^{-1}\sum_iB_i$ be their observed frequency, a [sample mean](sample-mean.md). Since every [interval](interval-mathematics.md) width is one, $V=n$. Substituting $t=n\varepsilon$ into the [Hoeffding inequality](hoeffding-inequality.md) gives

$$
\mathbb P(\widehat p_n-p\geq\varepsilon)\leq e^{-2n\varepsilon^2},\qquad \mathbb P(|\widehat p_n-p|\geq\varepsilon)\leq\min\{1,2e^{-2n\varepsilon^2}\}.
$$

For tolerance $0<\varepsilon<1$ and failure [probability](probability.md) $0<\delta<1$, solving $2e^{-2n\varepsilon^2}\leq\delta$ yields the sufficient [sample size](sample-size.md)

$$
\boxed{n\geq\left\lceil\frac{\log(2/\delta)}{2\varepsilon^2}\right\rceil.}
$$

Here $\log$ is the [natural logarithm](natural-logarithm.md). For $\varepsilon=0.05$ and $\delta=0.05$, **$n=738$ guarantees an error smaller than $0.05$ with [probability](probability.md) at least $0.95$**, for every $p\in[0,1]$. The two-sided bound at this [sample size](sample-size.md) is approximately $0.0499440$. A specified single direction instead needs $n\geq\lceil\log(1/\delta)/(2\varepsilon^2)\rceil$, or $600$ for these choices. Halving the tolerance multiplies the unrounded sufficient [sample size](sample-size.md) by four; reducing the failure [probability](probability.md) tenfold adds $\log(10)/(2\varepsilon^2)$ before rounding.

This is a conservative sufficient [sample size](sample-size.md), not a necessary minimum. For a specified $p$, the count $K=\sum_iB_i$ has a [binomial distribution](binomial-distribution.md), whose exact upper [tail probability](tail-probability.md) is

$$
\mathbb P(K\geq k)=\sum_{j=k}^n\binom njp^j(1-p)^{n-j},\qquad k\in\{0,\ldots,n\}.
$$

For $k>np$, the [Hoeffding inequality](hoeffding-inequality.md) bounds this by $\exp[-2(k-np)^2/n]$. An arbitrary frequency threshold uses $k=\lceil n(p+\varepsilon)\rceil$; if $k>n$, the [event](event.md) is impossible. The discreteness of the count and its [variance](variance-split.md) $np(1-p)$ can make the exact [tail probability](tail-probability.md) substantially smaller. At $n=100$, $p=1/2$, $k=60$, the exact upper [tail probability](tail-probability.md) is about $0.0284440$, while the bound is $e^{-2}\approx0.135335$. At $p=1/10$, $k=20$, the same deviation $\varepsilon=0.1$ gives the same bound but an exact upper [tail probability](tail-probability.md) about $0.00197856$.

<a id="image-exact-binomial-distribution-tails-compared-with-the-hoeffding-inequality"></a>
![](hoeffding-binomial-tail-comparison.png)

**[Figure 6](#image-exact-binomial-distribution-tails-compared-with-the-hoeffding-inequality). Exact binomial distribution tails compared with the Hoeffding inequality**. Two original specified models, each with $n=100$ [independent](independent-random-variables.md) [Bernoulli trials](bernoulli-trial.md). Each dot includes its integer threshold $K\geq k$, with horizontal coordinate $\varepsilon=k/n-p$. Exact finite sums are evaluated with rational arithmetic before conversion for plotting. The [Hoeffding inequality](hoeffding-inequality.md) uses the width one in both panels; it does not use the smaller [variance](variance-split.md) at $p=1/10$. These are model probabilities, not measured frequencies.

## ↑ Ancestors (8)

1. [Hoeffding inequality](hoeffding-inequality.md)
2. [Concentration inequality](concentration-inequality.md)
3. [Probability inequality](probability-inequality-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Hoeffding confidence interval](hoeffding-confidence-interval.md)
- [Hoeffding lemma](hoeffding-lemma.md)
