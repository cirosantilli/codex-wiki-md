<h1 id="m/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The independent identically distributed [central limit theorem](../../../../central-limit-theorem.md) states that for independent identically distributed [random variables](../../../../random-variable-split.md) $U_k$ with finite [mean](../../../../expected-value-split.md) $\mu$ and positive finite [variance](../../../../variance-split.md) $\sigma^2$,

$$
\frac{\sum_{k=1}^nU_k-n\mu}{\sigma\sqrt n}\ \xrightarrow{d}\ N(0,1).
$$

For $0<u<1$, [continuity](../../../../continuous-function.md), strict monotonicity and the endpoint limits of the [cumulative distribution function](../../../../cumulative-distribution-function.md) give a unique $x=F^{-1}(u)$. Then $P(F(X)\le u)=P(X\le x)=F(x)=u$. Thus $Y=F(X)$ has the [uniform distribution](../../../../continuous-uniform-distribution.md) on $(0,1)$, by the [probability integral transform](../../../../probability-integral-transform.md).

For $W=-\log(1-Y)$, $P(W\le w)=1-e^{-w}$ when $w\ge0$, and it is zero otherwise. Therefore its [probability density function](../../../../probability-density-function.md) is $e^{-w}\chi_{(0,\infty)}(w)$: the [exponential distribution](../../../../exponential-distribution.md) of rate one. By [integration by parts](../../../../integration-by-parts.md), $E[W]=1$ and $E[W^2]=2$, so $\operatorname{Var}(W)=1$.

The variables $W_k=-\log(1-F_k(X_k))$ are independent because they are separate measurable functions of independent [random variables](../../../../random-variable-split.md). The [probability integral transform](../../../../probability-integral-transform.md) makes all of them identically distributed as $\operatorname{Exp}(1)$, even though the $X_k$ need not be identically distributed. The displayed $Z_n$ is exactly $n^{-1/2}\sum_{k=1}^n(W_k-1)$. The [central limit theorem](../../../../central-limit-theorem.md) therefore gives

$$
\boxed{Z_n\xrightarrow{d}N(0,1).}
$$

## ↑ Ancestors (12)

1. [4](../4.md)
2. [M](../../m.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
