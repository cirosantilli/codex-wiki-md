<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [moment-generating function](../../../../../../moment-generating-function.md) of a [mixture distribution](../../../../../../mixture-distribution.md) is the mixture of its component transforms, so

$$
\boxed{M_T(r)=1-q+qM_Z(r).}
$$

For the aggregate, positivity of every claim implies $S=0$ exactly when $N=0$. Choose

$$
p=\mathbb P(N=0)=G_N(0),\qquad q=1-p.
$$

If $q>0$, take $\widetilde N$ to have the [zero-truncated claim-count distribution](../../../../../../zero-truncated-claim-count-distribution.md), namely the conditional law of $N$ given $N>0$. Then

$$
\mathbb P(\widetilde N=n)=\frac{\mathbb P(N=n)}{1-p}\quad(n\ge1),
\qquad G_{\widetilde N}(z)=\frac{G_N(z)-p}{1-p}.
$$

Choose this count independently of a fresh independent claim-size sequence and put $Z=\sum_{i=1}^{\widetilde N}X_i$. Its [probability distribution](../../../../../../probability-distribution.md) is that of $S$ conditional on being positive. Thus the [hurdle decomposition of a positive random sum](../../../../../../hurdle-decomposition-of-a-positive-random-sum.md) gives

$$
M_S(r)=p+(1-p)G_{\widetilde N}(M_X(r))=1-q+qM_Z(r),
$$

and an independent [Bernoulli random variable](../../../../../../bernoulli-distribution.md) $B$ of success probability $q$ realizes $S\overset d=BZ$. This establishes the distributional representation, including that $Z$ is itself a positive [random sum of independent claims](../../../../../../random-sum-of-independent-claims.md). If $p=1$, the aggregate is identically zero; set $q=0$ and choose any positive $Z$, for example one claim. Conditioning the count on positivity is then unnecessary and would be undefined.

For the specified [geometric distribution](../../../../../../geometric-distribution.md) on the nonnegative integers,

$$
G_N(z)=\frac{1}{2-z},\qquad p=q=\frac12,\qquad
G_{\widetilde N}(z)=\frac{z}{2-z}.
$$

An [exponential distribution](../../../../../../exponential-distribution.md) of [expected value](../../../../../../expected-value.md) $\mu$ has transform $M_X(r)=(1-\mu r)^{-1}$. Substitution yields

$$
M_Z(r)=\frac{(1-\mu r)^{-1}}{2-(1-\mu r)^{-1}}
=\frac{1}{1-2\mu r},\qquad r<\frac{1}{2\mu}.
$$

Hence **$Z$ is exponential with rate $1/(2\mu)$ and expected value $2\mu$**. This is the [geometric sum of exponential variables](../../../../../../geometric-sum-of-exponential-variables.md) with a rescaling of the claim mean. Identification can also use the [uniqueness theorem for Laplace transforms of nonnegative random variables](../../../../../../uniqueness-theorem-for-laplace-transforms-of-nonnegative-random-variables.md) by taking $r\le0$.

The resulting [distribution function](../../../../../../cumulative-distribution-function.md) is

$$
\boxed{F_S(x)=\begin{cases}
0,&x<0,\\
1-\tfrac12e^{-x/(2\mu)},&x\ge0.
\end{cases}}
$$

Its jump of size $1/2$ at zero is important: the aggregate law is not a purely continuous [exponential distribution](../../../../../../exponential-distribution.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
