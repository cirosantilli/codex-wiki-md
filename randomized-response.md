# Randomized response

↑ **Parent:** [Statistical inference](statistical-inference-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Randomized_response)

[Randomized response](randomized-response.md) masks which of two complementary binary questions a person answered. Suppose the sensitive property has [probability](probability.md) $p$, and independently the direct question is selected with known [probability](probability.md) $x$, while the complementary question is selected otherwise. Truthful answers then have yes [probability](probability.md) $q=xp+(1-x)(1-p)$. The investigator observes only the answer, preserving uncertainty about an individual's status while permitting population [statistical estimation](statistical-estimation.md) when $x\ne1/2$.

For $n$ independent responses, $Y\sim\operatorname{Bin}(n,q)$, and the affine [estimator](estimator.md) $\widetilde p=(Y/n-1+x)/(2x-1)$ is an [unbiased estimator](unbiased-estimator.md). Its [variance](variance-split.md) is $q(1-q)/[n(2x-1)^2]$, by the mean and [variance](variance-split.md) of a [binomial distribution](binomial-distribution.md). Equivalently the [variance](variance-split.md) is $p(1-p)/n+x(1-x)/[n(2x-1)^2]$, exposing the extra sampling uncertainty caused by the masking. At $x=1/2$, all $p$ produce $q=1/2$ and [identifiability](identifiability.md) fails. At $x=0$ or $1$, there is no masking and the extra variance vanishes.

Because $0\leq p\leq1$, [maximum likelihood estimation](maximum-likelihood-estimation-split.md) gives $\widehat p=\min(1,\max(0,\widetilde p))$. This follows by maximizing the [binomial likelihood](binomial-likelihood.md) over the interval $q\in[\min(x,1-x),\max(x,1-x)]$ and then inverting its monotone affine parametrization. Clipping can introduce [bias](bias-of-an-estimator.md): for $n=1$, $x=3/4$ and $p=0$, the clipped estimate has mean $1/4$.

## ↑ Ancestors (5)

1. [Statistical inference](statistical-inference-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-options-i-course-of-the-university-of-oxford/2006/o/o2/solution.md)
- [Randomized response](randomized-response.md)
