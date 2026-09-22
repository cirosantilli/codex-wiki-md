<h1 id="26k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set $\boxed{\beta=1/(1-\alpha)=1/r}$. For fixed $t>0$ and large $n$,

$$
\mathbb P\bigl(n^{1/r}(\widehat\theta_n-\theta)>t\bigr)
=\left(1-\frac{t^r}{n}\right)^n\longrightarrow\boxed{e^{-t^r}}.
$$

This [endpoint maximum likelihood for a singular location density](../../../../../../endpoint-maximum-likelihood-for-a-singular-location-density.md) calculation gives a [Weibull distribution](../../../../../../weibull-distribution.md) with shape $r$. The estimator is a [consistent estimator](../../../../../../consistency-statistics.md), and its error has order $n^{-1/r}$, faster than the $n^{-1/2}$ error of $\widetilde\theta_n$. Its [bias](../../../../../../bias-of-an-estimator.md) is asymptotic to $\Gamma(1+1/r)n^{-1/r}$ and its [mean squared error](../../../../../../mean-squared-error.md) to $\Gamma(1+2/r)n^{-2/r}$, versus a positive constant times $n^{-1}$ for the sample-mean estimator. Thus **the minimum estimator is preferable for its much faster convergence**, despite its positive finite-sample [bias](../../../../../../bias-of-an-estimator.md). This is a nonregular support-dependent model; ordinary regular-model efficiency bounds do not apply.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [26K](../../26k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
