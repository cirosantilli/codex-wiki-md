<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The original PDF specifies a [geometric distribution](../../../../../../geometric-distribution.md) on $\{0,1,\ldots\}$, with probabilities $pq^k$. Its [probability generating function](../../../../../../probability-generating-function.md) is $p/(1-qz)$. By [independence](../../../../../../independent-random-variables.md), the total original claim count $K=\sum_iN_i$ has

$$
G_K(z)=\left(\frac p{1-qz}\right)^n,
\qquad
\mathbb P(K=k)=\binom{n+k-1}{k}p^nq^k,\quad k\ge0.
$$

The coefficient follows from the [negative binomial series](../../../../../../negative-binomial-series.md). Thus **one representation uses independent unit-rate [exponential distribution](../../../../../../exponential-distribution.md) steps and a [negative binomial distribution](../../../../../../negative-binomial-distribution.md) count $K$**.

There is a second useful [random sum of independent claims](../../../../../../random-sum-of-independent-claims.md) representation. For one policy, the [random-sum transform identity](../../../../../../random-sum-transform-identity.md) gives

$$
M_{T_i}(u)=\frac{p}{1-q/(1-u)}=\frac{p(1-u)}{p-u}=p+q\frac p{p-u},\qquad u<p.
$$

This is the [mixture distribution](../../../../../../mixture-distribution.md) of zero with probability $p$ and a rate-$p$ [exponential distribution](../../../../../../exponential-distribution.md) with probability $q$. Consequently

$$
\boxed{T\overset d=\sum_{j=1}^B Y_j,\qquad B\sim\operatorname{Binomial}(n,q),\quad Y_j\sim\operatorname{Exp}(p),}
$$

with the [binomial distribution](../../../../../../binomial-distribution.md) count independent of the independent steps. Equality follows by multiplying the [moment-generating functions](../../../../../../moment-generating-function.md). This is a [negative-binomial sum of exponential claims](../../../../../../negative-binomial-sum-of-exponential-claims.md).

When $n=2$, the three values of $B$ give

$$
\mathcal L(T)=p^2\delta_0+2pq\operatorname{Exp}(p)+q^2\operatorname{Erlang}(2,p).
$$

Thus the zero mass is $\boxed{b=p^2}$, and the conditional positive [probability density function](../../../../../../probability-density-function.md) is

$$
\boxed{\widetilde f_T(x)=\frac{p^2e^{-px}}{1-p^2}(2q+q^2x),\qquad x>0.}
$$

Its integral is $(2pq+q^2)/(1-p^2)=1$. Equivalently the positive-component [cumulative distribution function](../../../../../../cumulative-distribution-function.md) is

$$
\widetilde F_T(x)=1-e^{-px}\left(1+\frac{pq^2x}{1-p^2}\right),\qquad x\ge0,
$$

so $F_T(x)=p^2+(1-p^2)\widetilde F_T(x)$. For $x<0$, $F_T(x)=0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
