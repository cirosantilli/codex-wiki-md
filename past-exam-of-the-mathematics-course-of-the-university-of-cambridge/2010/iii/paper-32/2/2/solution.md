<h1 id="2/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Set $S_n=\sum_{i=1}^nY_i$ and $a_n=\sum_{i=1}^n2^{-i}=1-2^{-n}$. For the [Poisson distribution](../../../../../../poisson-distribution.md) observations, factors independent of $\theta$ can be removed from the [likelihood function](../../../../../../likelihood-function.md), leaving

$$
L_n(\theta)\propto\theta^{S_n}e^{-a_n\theta},\qquad \ell_n(\theta)=S_n\log\theta-a_n\theta+\text{constant}.
$$

When $S_n>0$, the [log-likelihood](../../../../../../log-likelihood.md) derivative is $S_n/\theta-a_n$ and its second derivative is negative. The unique positive [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) is therefore

$$
\boxed{\widehat\theta_n=\frac{S_n}{1-2^{-n}}\quad(S_n>0).}
$$

There is a genuine boundary qualification: if $S_n=0$, the [likelihood](../../../../../../likelihood-function.md) decreases strictly on $\theta>0$, so **no maximum is attained in the stated open parameter space**. On the closure $\theta\ge0$, its maximizer is $0$. Defining the usual extended [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) by the same displayed formula for every $S_n$ allows its [statistical consistency](../../../../../../consistency-statistics.md) to be examined; the all-zero event cannot be ignored because its probability does not tend to zero.

Indeed, sums of independent [Poisson distribution](../../../../../../poisson-distribution.md) variables give $S_n\sim\operatorname{Poi}(\theta a_n)$, so

$$
\mathbb P_\theta\bigl(|\widehat\theta_n-\theta|>\theta/2\bigr)\ge\mathbb P_\theta(S_n=0)=e^{-\theta a_n}\longrightarrow e^{-\theta}>0.
$$

Thus **the extended maximum-likelihood estimator is inconsistent**. More precisely, $S_n$ increases to $S_\infty=\sum_{i\ge1}Y_i$, and $\mathbb E S_\infty=\theta<\infty$ shows that this total count is finite almost surely. Its distribution is [Poisson distribution](../../../../../../poisson-distribution.md) with mean $\theta$, by taking limits of the finite-sum laws. Hence

$$
\widehat\theta_n\longrightarrow S_\infty\sim\operatorname{Poi}(\theta)\quad\text{almost surely}.
$$

This [finite-exposure Poisson inconsistency](../../../../../../finite-exposure-poisson-inconsistency.md) leaves a nondegenerate random limit even with infinitely many observations. Correspondingly, the total [Fisher information](../../../../../../fisher-information-matrix.md) is $a_n/\theta\to1/\theta$, rather than diverging. The common-distribution hypothesis in the introductory [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation.md) theorem is absent here.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2](../../2.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
