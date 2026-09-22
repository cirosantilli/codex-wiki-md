<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [log-likelihood function](../../../../../../log-likelihood.md) for the [Laplace distribution](../../../../../../laplace-distribution.md) is

$$
\ell(\kappa)=-n\log2-\sum_{i=1}^n|Y_i-\kappa|.
$$

Thus [maximum likelihood estimation](../../../../../../maximum-likelihood-estimation-split.md) is equivalent to minimizing the sum of [absolute values](../../../../../../absolute-value.md). Write $n=2m+1$ and sort the data as $Y_{(1)}\le\cdots\le Y_{(n)}$. Between observations, if $r$ values lie to the left of $\kappa$, the [derivative](../../../../../../derivative.md) of $\sum_i|Y_i-\kappa|$ is $r-(n-r)=2r-n$. It is negative before the middle observation and positive after it. The minimum occurs at the [sample median](../../../../../../sample-median.md):

$$
\boxed{\widehat\kappa=Y_{(m+1)}=Y_{((n+1)/2)}.}
$$

This minimizer remains unique for odd $n$ even when some observations coincide, since fewer than half the observations can lie strictly on either side of the middle value.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Mathematics III](../../../mathematics-iii-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
