<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First establish the limiting law needed by the [delta method](../../../../../delta-method.md). For fixed $t$, put $u_n=1/2+t/\sqrt n$ and let $N_n$ count how many of the $U_i$ are at most $u_n$. Then $N_n$ has a [binomial distribution](../../../../../binomial-distribution.md) with [expectation](../../../../../expected-value-split.md) $n/2+t\sqrt n$ and [variance](../../../../../variance-split.md) $n/4-t^2$. The event $M_U\leq u_n$ is exactly $N_n\geq(n+1)/2$. Its standardized threshold tends to $-2t$, so the [central limit theorem](../../../../../central-limit-theorem.md) for these binomial counts gives

$$
\Pr\!\left(\sqrt n(M_U-1/2)\leq t\right)\longrightarrow\Phi(2t).
$$

Here $\Phi$ is the [cumulative distribution function](../../../../../cumulative-distribution-function.md) of the [standard normal distribution](../../../../../standard-normal-distribution.md). Equivalently,

$$
\sqrt n(M_U-1/2)\xrightarrow{d}N(0,1/4).
$$

Use the usual local regularity for the [delta method](../../../../../delta-method.md): $f$ is continuous at the population [median](../../../../../median.md) $\theta$ and $f(\theta)>0$. The [inverse function theorem](../../../../../inverse-function-theorem.md), applied at $F(\theta)=1/2$, gives

$$
\left.\frac{d}{du}F^{-1}(u)\right|_{u=1/2}=\frac1{f(\theta)}.
$$

Therefore

$$
\boxed{\sqrt n(M_X-\theta)\xrightarrow{d}
N\!\left(0,\frac1{4f(\theta)^2}\right).}
$$

The [asymptotic normality](../../../../../asymptotic-normality.md) gives the requested leading [variance](../../../../../variance-split.md) approximation

$$
\boxed{\operatorname{avar}(M_X)=\frac1{4n f(\theta)^2}.}
$$

Here the variance parameter for the rescaled limiting law is $1/(4f(\theta)^2)$, while the source states the corresponding $1/n$ approximation for the unscaled [estimator](../../../../../estimator.md). Strict increase of $F$ alone does not force $f(\theta)>0$; that local condition is needed for this form of the [asymptotic distribution of a sample median](../../../../../asymptotic-distribution-of-a-sample-median.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
