<h1 id="12h/solution">Solution</h1>

↑ **Parent:** [12H](../12h.md)

Assume the two normal samples are independent. Write $n_X=6$, $n_Y=21$, and let $S_X,S_Y$ denote their residual sums of squares about the respective sample means. The joint [likelihood function](../../../../../likelihood-function.md), apart from its constant factor, is

$$
L=(v_X)^{-n_X/2}(v_Y)^{-n_Y/2}\exp\left[-\frac{\sum(X_i-\mu_X)^2}{2v_X}-\frac{\sum(Y_j-\mu_Y)^2}{2v_Y}\right],
$$

where $v_X=\sigma_X^2$, $v_Y=\sigma_Y^2$. For every fixed variance pair the means maximize this likelihood at $\bar X,\bar Y$, because $\sum(X_i-\mu_X)^2=S_X+n_X(\bar X-\mu_X)^2$, and likewise for $Y$.

Under equal variances, differentiate the profiled log-likelihood to obtain $\widehat v_0=(S_X+S_Y)/(n_X+n_Y)$. Without the order constraint, the separate variance maxima are $\widehat v_X=S_X/n_X$, $\widehat v_Y=S_Y/n_Y$. If $\widehat v_X>\widehat v_Y$ they lie in the alternative. If their order is reversed, maximizing over $v_X\geq v_Y$ puts the optimum on the equal-variance boundary. These assertions also follow by strict concavity in the precisions $1/v_X,1/v_Y$.

Thus the [one-sided likelihood-ratio test for two normal variances](../../../../../one-sided-likelihood-ratio-test-for-two-normal-variances.md) uses the quotient of the null maximum to the maximum over null and ordered alternative:

$$
\Lambda=\begin{cases}\displaystyle\frac{(S_X/n_X)^{n_X/2}(S_Y/n_Y)^{n_Y/2}}{[(S_X+S_Y)/(n_X+n_Y)]^{(n_X+n_Y)/2}},&R>1,\\1,&R\leq1,\end{cases}\qquad R=\frac{S_X/n_X}{S_Y/n_Y}.
$$

To identify the rejection direction, put $q=S_X/(S_X+S_Y)$. Up to constants, $\log\Lambda=(n_X/2)\log q+(n_Y/2)\log(1-q)$. Its derivative is $[n_X-(n_X+n_Y)q]/[2q(1-q)]$, negative on the ordered branch $q>n_X/(n_X+n_Y)$. Hence small likelihood ratios mean a large sample variance ratio.

The null law must account for estimating both means. By [Cochran's theorem](../../../../../cochran-s-theorem.md), $S_X/\sigma^2$ and $S_Y/\sigma^2$ are independent random variables with [chi-squared distributions](../../../../../chi-squared-distribution.md) of 5 and 20 degrees of freedom. Consequently the exact null statistic is

$$
F=\frac{S_X/5}{S_Y/20}\sim F_{5,20}.
$$

It is an increasing multiple of $R$, so an upper-tail critical region is the likelihood-ratio rejection region. The observed statistic is $F=(30/5)/(40/20)=3$. The supplied 95th percentile is 2.71, so

$$
\boxed{3>2.71:\quad\text{reject equal variances at the 5 percent level in favor of }\sigma_X^2>\sigma_Y^2.}
$$

The [F-distribution](../../../../../f-distribution.md) degrees of freedom are $5,20$, not $6,21$, although the variance maximum-likelihood estimates themselves have denominators $6,21$.

## ↑ Ancestors (10)

1. [12H](../12h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
