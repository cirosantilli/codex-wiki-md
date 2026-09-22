<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Condition on the [claim count](../../../../../claim-count.md). The empty [random sum of independent claims](../../../../../random-sum-of-independent-claims.md) is zero, and independence gives $\mathbb E[e^{tS}\mid N=n]=M_X(t)^n$. Therefore the [random-sum transform identity](../../../../../random-sum-transform-identity.md) is

$$
\boxed{M_S(t)=\sum_{n=0}^{\infty}\mathbb P(N=n)M_X(t)^n=G_N(M_X(t)),}
$$

wherever the composition is finite. This follows directly from the [law of total expectation](../../../../../law-of-total-expectation.md), rather than replacing the random count by its mean.

Put $q=1-p$. For the specified [negative binomial distribution](../../../../../negative-binomial-distribution.md), the [negative binomial series](../../../../../negative-binomial-series.md) gives $G_N(z)=[p/(1-qz)]^k$. A rate-$\lambda$ [exponential distribution](../../../../../exponential-distribution.md) has [moment-generating function](../../../../../moment-generating-function.md) $M_X(t)=\lambda/(\lambda-t)$. Hence

$$
M_S(t)=\left(\frac{p(\lambda-t)}{p\lambda-t}\right)^k
=\left(p+q\frac{p\lambda}{p\lambda-t}\right)^k,\qquad t<p\lambda.
$$

The last expression is exactly the [moment-generating function](../../../../../moment-generating-function.md) of a [compound binomial distribution](../../../../../compound-binomial-distribution.md) with independent count and severities

$$
\boxed{\widetilde N\sim\operatorname{Binomial}(k,1-p),\qquad\widetilde X_j\sim\operatorname{Exp}(p\lambda).}
$$

The [moment-generating function](../../../../../moment-generating-function.md) exists in a neighborhood of zero, so its uniqueness identifies the distributions. In particular, the new [claim sizes](../../../../../claim-size.md) have mean $1/(p\lambda)$, not $1/\lambda$, and both aggregate distributions have an atom $p^k$ at zero. This is the [negative-binomial sum of exponential claims](../../../../../negative-binomial-sum-of-exponential-claims.md) representation with the severity rate explicitly retained.

Conditional on $N=n\ge1$, the aggregate has [Erlang distribution](../../../../../erlang-distribution.md) with density $\lambda^n s^{n-1}e^{-\lambda s}/(n-1)!$ on $s>0$. Repeated [integration by parts](../../../../../integration-by-parts.md) of its tail gives

$$
\mathbb P(S>x\mid N=n)=e^{-\lambda x}\sum_{j=0}^{n-1}\frac{(\lambda x)^j}{j!}.
$$

Indeed, after substituting $v=\lambda s$, the integral $\int_{\lambda x}^{\infty}e^{-v}v^{n-1}\,dv/(n-1)!$ reduces recursively to the corresponding integral with exponent $n-2$, terminating at $e^{-\lambda x}$. Applying the [law of total probability](../../../../../law-of-total-probability.md) yields the original infinite [mixture distribution](../../../../../mixture-distribution.md) tail

$$
\mathbb P(S>x)=\sum_{n=1}^{\infty}p_n e^{-\lambda x}\sum_{j=0}^{n-1}\frac{(\lambda x)^j}{j!},\qquad x>0.
$$

Applying the same argument to the [compound binomial distribution](../../../../../compound-binomial-distribution.md) gives instead the [finite Erlang-mixture tail for a negative-binomial exponential aggregate](../../../../../finite-erlang-mixture-tail-for-a-negative-binomial-exponential-aggregate.md):

$$
\boxed{\mathbb P(\widetilde S>x)=\sum_{n=1}^{k}\binom{k}{n}q^n p^{k-n}e^{-p\lambda x}\sum_{j=0}^{n-1}\frac{(p\lambda x)^j}{j!}.}
$$

The two tails are equal. **The binomial representation replaces an infinite sum by a finite exact calculation**, eliminating the need to choose a claim-count truncation and control its omitted tail. The inner sums can be evaluated recursively, using $a_{j+1}=a_j(p\lambda x)/(j+1)$ for their exponential-weighted terms.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
