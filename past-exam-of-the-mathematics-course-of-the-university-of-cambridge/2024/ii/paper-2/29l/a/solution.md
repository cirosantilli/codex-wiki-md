<h1 id="29l/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\widehat\theta_n$ be the MLE and let $I(\theta)$ be the one-observation Fisher information [matrix](../../../../../../matrix.md). One standard form of the Wald statistic is

$$
\boxed{W_n(\theta)
=n(\widehat\theta_n-\theta)^T
I(\widehat\theta_n)(\widehat\theta_n-\theta)}.
$$

Any consistent information estimator gives the same asymptotics. Under $H_0$,  
$W_n(\theta_0)\Rightarrow\chi_p^2$. If  
$c_{p,\alpha}$ is the $(1-\alpha)$ quantile of $\chi_p^2$, reject when

$$
W_n(\theta_0)>c_{p,\alpha}.
$$

The asymptotic type-I error is $\alpha$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [29L](../../29l.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
