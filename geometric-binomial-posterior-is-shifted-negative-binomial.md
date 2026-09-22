# Geometric-binomial posterior is shifted negative binomial

↑ **Parent:** [Geometric count under Bernoulli thinning](geometric-count-under-bernoulli-thinning.md)

Let $\mathbb P(X=n)=p(1-p)^n$ for $n\geq0$ and $Y\mid X=n\sim\operatorname{Binomial}(n,q)$, with $0<p,q<1$. Write $D=p+q-pq$. Summing the joint [probability mass function](probability-mass-function.md) with the differentiated [geometric series](geometric-series.md) identity $\sum_{n=k}^\infty\binom nk t^{n-k}=(1-t)^{-k-1}$ gives $\mathbb P(Y=k)=(p/D)((1-p)q/D)^k$. By [Bayes' theorem](bayes-theorem.md),

$$
\mathbb P(X=n\mid Y=k)=\binom nk D^{k+1}(1-D)^{n-k},\qquad n\geq k.
$$

Thus $X-k$, given $Y=k$, has the failure-count [negative binomial distribution](negative-binomial-distribution.md) for $k+1$ successes and success parameter $D$. Its [conditional expectation](conditional-expectation.md) is $k+(k+1)(1-D)/D$ for $X$ itself. The shift by $k$, the number of retained successes, must be retained when identifying the posterior [distribution](distribution-mathematical-analysis.md).

## ↑ Ancestors (9)

1. [Geometric count under Bernoulli thinning](geometric-count-under-bernoulli-thinning.md)
2. [Geometric distribution](geometric-distribution.md)
3. [Discrete probability distribution](discrete-probability-distribution-split.md)
4. [Probability distribution](probability-distribution-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/discrete-mathematics-continuous-mathematics-and-probability-resit/7/b/ii/solution.md)
