# Chernoff information for complementary Bernoulli distributions

↑ **Parent:** [Chernoff information](chernoff-information.md)

Let $P$ be the [Bernoulli distribution](bernoulli-distribution.md) with success probability $0.2$ and $Q$ the [Bernoulli distribution](bernoulli-distribution.md) with success probability $0.8$. For $0\leq s\leq1$,

$$
Z(s)=0.2^s0.8^{1-s}+0.8^s0.2^{1-s}.
$$

The two summands have product $0.16$. Their [arithmetic mean](arithmetic-mean.md) is at least their [geometric mean](geometric-mean.md), with equality at $s=1/2$. Thus

$$
\boxed{C(P,Q)=-\ln0.8\simeq0.22314355\ \text{nats per observation}.}
$$

The same argument gives $C=-\ln(2\sqrt{p(1-p)})$ for complementary parameters $0<p<1$. At $p=1/2$ the laws agree and $C=0$.

<a id="image-chernoff-complementary-coin-affinity"></a>
![](chernoff-complementary-coin-affinity.png)

**[Figure 9](#image-chernoff-complementary-coin-affinity). Chernoff affinity and Chernoff information for two complementary coin laws**. Original computed example, with success probabilities $0.2$ and $0.8$. The affinity is minimized at $s=1/2$; the best negative-log affinity is $-\ln0.8$.

With equal [prior probabilities](prior-probability.md), count the successes $K$ among $n$ observations. The [likelihood ratio](likelihood-ratio.md) is $Q^{\otimes n}/P^{\otimes n}=4^{2K-n}$, so choose $Q$ when $K>n/2$ and $P$ when $K<n/2$. If $n$ is even, either decision or a fair tie randomization gives the same average error at $K=n/2$. Under $P$, $K$ has the [binomial distribution](binomial-distribution.md) with parameters $n,0.2$. Symmetry therefore gives the exact optimal average error

$$
p_n^*=\sum_{k>n/2}\binom nk0.2^k0.8^{n-k}
+\frac12\mathbf1_{\{n\text{ even}\}}\binom n{n/2}0.2^{n/2}0.8^{n/2}.
$$

The last term applies only for even $n$; it represents half the tie probability. Direct finite [sums](sum.md) give $p_1^*=0.2$, $p_5^*=0.05792$ and $p_{20}^*\simeq0.00157912$. **Twenty observations reduce the optimal average error to about 0.158%.** The [finite-sample Chernoff error bound](finite-sample-chernoff-error-bound.md) at $n=20$ is $\tfrac12(0.8)^{20}\simeq0.00576461$, a guarantee rather than the exact error.

<a id="image-chernoff-coin-testing-error-decay"></a>
![](chernoff-coin-testing-error-decay.png)

**[Figure 10](#image-chernoff-coin-testing-error-decay). Exact repeated-coin error, the finite-sample Chernoff error bound, and the limiting error exponent**. Original finite-binomial calculations under two fixed independent coin laws with equal priors. The first panel uses a [logarithmic scale](logarithmic-scale.md). The normalized negative log error approaches $C(P,Q)$; finite-sample error need not equal the simple exponential.

Reducing the exact error from $p_{20}^*$ to $p_{50}^*\simeq1.29363\times10^{-6}$ illustrates the value of repeated evidence. The example assumes a single fixed coin law throughout the experiment. If repeated sensor readings share an unmodelled common error, increasing their number need not supply this much independent information.

## ↑ Ancestors (7)

1. [Chernoff information](chernoff-information.md)
2. [Binary hypothesis testing in information theory](binary-hypothesis-testing-in-information-theory.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Chernoff information](chernoff-information.md)
