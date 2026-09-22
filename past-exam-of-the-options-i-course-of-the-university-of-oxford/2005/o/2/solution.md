<h1 id="o/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A $100(1-\alpha)\%$ [confidence interval](../../../../confidence-interval.md) procedure produces random endpoints $L,U$ such that $\mathbb P_\mu(L\leq\mu\leq U)=1-\alpha$, under the model. In everyday terms, repeating the same sampling and interval construction many times would give intervals containing the true mean in about $100(1-\alpha)\%$ of repetitions.

For $n\geq2$, define the [sample mean](../../../../sample-mean.md) $\bar X=n^{-1}\sum_iX_i$ and the [sample variance](../../../../sample-variance.md) $S^2=(n-1)^{-1}\sum_i(X_i-\bar X)^2$. For [independent](../../../../independent-random-variables.md) observations from a [normal distribution](../../../../normal-distribution.md) with $\sigma^2>0$, the standard sampling results are

$$
\frac{\sqrt n(\bar X-\mu)}S\sim t_{n-1},\qquad\frac{(n-1)S^2}{\sigma^2}\sim\chi^2_{n-1}.
$$

The first follows from the [independent](../../../../independent-random-variables.md) [normal sample](../../../../normal-sample.md) mean and [sample variance](../../../../sample-variance.md). Let $q=t_{n-1,1-\alpha/2}$ be the positive Student [quantile](../../../../quantile-function.md). Symmetry gives the central [confidence interval](../../../../confidence-interval.md)

$$
\boxed{\left[\bar X-q\frac S{\sqrt n},\ \bar X+q\frac S{\sqrt n}\right].}
$$

Its width is $W=2qS/\sqrt n$, so

$$
\boxed{c=\frac{n(n-1)}{4t_{n-1,1-\alpha/2}^{\,2}},\qquad \frac{cW^2}{\sigma^2}=\frac{(n-1)S^2}{\sigma^2}\sim\chi^2_{n-1}.}
$$

## ↑ Ancestors (12)

1. [2](../2.md)
2. [O](../../o.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
