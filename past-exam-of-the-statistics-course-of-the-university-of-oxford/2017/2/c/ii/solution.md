<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Under the [null hypothesis](../../../../../null-hypothesis.md), the full model has two free positive [statistical parameters](../../../../../statistical-parameter.md) and the constrained model has one. The [Wilks theorem](../../../../../wilks-theorem.md) therefore gives

$$
W=-2\log\Lambda\xrightarrow d\chi^2_1
$$

as both sample sizes tend to infinity, with $n/(n+m)$ tending to a number strictly between zero and one. For the observed $t$, calculate

$$
w_{\rm obs}=2\left[n\log\frac{n}{(n+m)t}+m\log\frac{m}{(n+m)(1-t)}\right].
$$

The large-sample [p-value](../../../../../p-value.md) is the upper-tail [probability](../../../../../probability.md)

$$
\boxed{p_{\rm approx}=1-F_{\chi^2_1}(w_{\rm obs})
=2\{1-\Phi(\sqrt{w_{\rm obs}})\},}
$$

where $\Phi$ is the [cumulative distribution function](../../../../../cumulative-distribution-function.md) of the [standard normal distribution](../../../../../standard-normal-distribution.md). The last equality uses the fact that the square of a [standard normal random variable](../../../../../standard-normal-random-variable.md) has a [chi-squared distribution](../../../../../chi-squared-distribution.md) with one [statistical degree of freedom](../../../../../statistical-degrees-of-freedom.md). Values of $T$ on either side of $n/(n+m)$ are already included by the transformation to $W$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
