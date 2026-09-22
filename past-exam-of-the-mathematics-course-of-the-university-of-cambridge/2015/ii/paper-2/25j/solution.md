<h1 id="25j/solution">Solution</h1>

↑ **Parent:** [25J](../25j.md)

For $n\geq1$, the binomial [log-likelihood](../../../../../log-likelihood.md) is $X\log\theta+(n-X)\log(1-\theta)$ plus a constant. Its maximizer, including endpoints, is **$\widehat\theta_{\rm MLE}=X/n$**. For $0<\theta<1$, the [Fisher information](../../../../../fisher-information-matrix.md) is

$$
\boxed{I(\theta)=\frac{n}{\theta(1-\theta)}.}
$$

This follows either from the expected negative second derivative or the [variance](../../../../../variance-split.md) of $(X-n\theta)/(\theta(1-\theta))$. At $0,1$ the usual regular score formula does not apply; the interior information diverges as an endpoint is approached.

For a symmetric [Beta distribution](../../../../../beta-distribution.md) prior $\operatorname{Beta}(s,s)$, conjugacy gives $\theta\mid X\sim\operatorname{Beta}(X+s,n-X+s)$, with [posterior mean](../../../../../posterior-mean.md) $(X+s)/(n+2s)$. All three priors below are instances of this calculation.

## ↑ Ancestors (10)

1. [25J](../25j.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
