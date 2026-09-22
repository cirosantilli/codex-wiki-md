<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First construct a centred [Gaussian process](../../../../../../gaussian-process.md) on the countable dyadic set with [covariance function](../../../../../../covariance-function.md) $\mathbb E(B_sB_t)=\min(s,t)$. These consistent finite-dimensional [normal distributions](../../../../../../normal-distribution.md) exist because, for coefficients $a_j$,

$$
\sum_{i,j}a_ia_j\min(t_i,t_j)=\int_0^1\left(\sum_ja_j\mathbf1_{\{u\leq t_j\}}\right)^2du\geq0;
$$

the [Kolmogorov extension theorem](../../../../../../kolmogorov-extension-theorem.md) realizes them on one [probability space](../../../../../../probability-space.md). Every increment has the [normal distribution](../../../../../../normal-distribution.md) $N(0,|t-s|)$, so for every finite $p\geq1$,

$$
\|B_t-B_s\|_p=(\mathbb E|Z|^p)^{1/p}|t-s|^{1/2}.
$$

Use the preceding estimate with $\beta=1/2$, $p>2$ and $0<\alpha<1/2-1/p$. It yields an [almost surely](../../../../../../almost-sure-convergence.md) [Hölder continuous](../../../../../../holder-condition.md) extension from the dense dyadic set to $[0,1]$. Approximate arbitrary times by dyadic times; continuity of the paths and of the Gaussian [covariance function](../../../../../../covariance-function.md) preserves all finite-dimensional laws. Disjoint increments are jointly Gaussian with zero cross-covariances, hence [independent](../../../../../../independent-random-variables.md), with the required variances. Together with $B_0=0$ and continuity, this constructs [Brownian motion](../../../../../../brownian-motion-split.md).

For any $\alpha<1/2$, choose $p$ large enough. Taking a countable increasing sequence of exponents tending to $1/2$ gives **simultaneous Hölder regularity of every order $\alpha<1/2$** on a common probability-one set; the same argument on each compact time interval gives local [Brownian Hölder regularity](../../../../../../brownian-holder-regularity.md). This method does not give the endpoint exponent. In fact that endpoint fails: if a path had a finite $1/2$-[Hölder seminorm](../../../../../../holder-seminorm.md) $K$, all its $2^n$ adjacent normalized increments at level $n$ would have magnitude at most $K$. These are [independent](../../../../../../independent-random-variables.md) standard [normal random variables](../../../../../../gaussian-random-variable.md), so for a fixed integer $m$ the probability that their maximum is at most $m$ is $\mathbb P(|Z|\leq m)^{2^n}\to0$. The event of a finite $K$ is contained in the union over $m$ of events with this bound at every level, each of probability zero. Thus **Brownian paths are not $1/2$-Hölder continuous on $[0,1]$ almost surely**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
