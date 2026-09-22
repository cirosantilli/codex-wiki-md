<h1 id="10h/solution">Solution</h1>

↑ **Parent:** [10H](../10h.md)

Assume independent samples $X_1,\ldots,X_n$ and $Y_1,\ldots,Y_m$, each consisting of independent [normal random variables](../../../../../gaussian-random-variable.md), with respective means $\mu_1,\mu_2$ and a common unknown [variance](../../../../../variance-split.md) $\sigma^2>0$. Take $n,m\geq2$. Normality, independence and equal variances are the assumptions giving the exact pooled [Student's t-test](../../../../../student-s-t-test.md); unequal variances would require a different test. We test $H_0:\mu_1=\mu_2$ against an unrestricted difference.

Put $N=n+m$ and

$$
W=\sum_i(X_i-\bar X)^2+\sum_j(Y_j-\bar Y)^2,\qquad
B=\frac{nm}{N}(\bar X-\bar Y)^2.
$$

The normal likelihood is proportional to $(\sigma^2)^{-N/2}\exp[-S/(2\sigma^2)]$, where $S$ is the residual sum of squares. Under the unrestricted model, the maximizing means are $\bar X,\bar Y$ and $S=W$. Under $H_0$, the maximizing common mean is $(n\bar X+m\bar Y)/N$ and decomposition about the [sample means](../../../../../sample-mean.md) gives $S=W+B$. For either model, maximizing over [variance](../../../../../variance-split.md) gives $\widehat\sigma^2=S/N$. Thus the [generalized likelihood-ratio test](../../../../../generalized-likelihood-ratio-test.md) statistic is

$$
\Lambda=\left(\frac{W}{W+B}\right)^{N/2}
=\left(1+\frac{T^2}{N-2}\right)^{-N/2},\qquad
T=\frac{\bar X-\bar Y}{s_p\sqrt{1/n+1/m}},\quad s_p^2=\frac{W}{N-2}.
$$

Small $\Lambda$ is therefore equivalent to large $|T|$.

Under the null, $Z=(\bar X-\bar Y)/[\sigma\sqrt{1/n+1/m}]$ is standard normal. In each sample an orthogonal change of Gaussian coordinates separates the sample-mean coordinate from the centered residual coordinates; those coordinates are independent. Consequently $V=W/\sigma^2$ has a [chi-squared distribution](../../../../../chi-squared-distribution.md) with $N-2$ degrees of freedom and is independent of $Z$. Therefore $T=Z/\sqrt{V/(N-2)}$ has the [Student's t-distribution](../../../../../student-s-t-distribution.md) with $N-2$ degrees of freedom. **At significance level $\alpha$, reject exactly when $\boxed{|T|>t_{N-2,1-\alpha/2}}$**, the two-sample pooled t-test.

## ↑ Ancestors (10)

1. [10H](../10h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
