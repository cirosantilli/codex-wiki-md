<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

A [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) maximizes the [likelihood](../../../../../likelihood-function.md) as a function of the parameter for the observed data. Under the usual regularity conditions, a scalar [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) satisfies $\sqrt n(\hat\theta-\theta)\Rightarrow N(0,I_1(\theta)^{-1})$, where $I_1$ is the [Fisher information](../../../../../fisher-information-matrix.md) in one observation.

For a [Poisson distribution](../../../../../poisson-distribution.md) with $\theta>0$, the [log-likelihood](../../../../../log-likelihood.md) is $\ell(\theta)=\sum_jY_j\log\theta-n\theta-\sum_j\log(Y_j!)$. Solving $\ell'(\theta)=0$ gives **$\boxed{\hat\theta=\bar Y}$.** Its [expectation](../../../../../expected-value.md) is $\theta$ and its [variance](../../../../../variance-split.md) is $\theta/n$. If all observations are zero, the maximum over $\theta\geq0$ occurs at zero; over $\theta>0$ this is a boundary supremum. The one-observation [score function](../../../../../informant-function.md) is $Y/\theta-1$, so $I_1(\theta)=\operatorname{Var}(Y)/\theta^2=1/\theta$ and the asymptotic variance of $\sqrt n(\bar Y-\theta)$ is $\theta$.

For $n\geq2$, let $S=(n-1)^{-1}\sum_j(Y_j-\bar Y)^2$. The identity

$$
\sum_j(Y_j-\bar Y)^2=\sum_j(Y_j-\theta)^2-n(\bar Y-\theta)^2
$$

gives $\mathbb E S=(n\theta-\theta)/(n-1)=\theta$, so $S$ is another [unbiased estimator](../../../../../unbiased-estimator.md). However, the total [score function](../../../../../informant-function.md) has [variance](../../../../../variance-split.md) $n/\theta$. For any regular [unbiased estimator](../../../../../unbiased-estimator.md) $T$, differentiating $\mathbb E_\theta T=\theta$ gives $\operatorname{Cov}(T,\ell')=1$, so the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) yields $\operatorname{Var}(T)\geq\theta/n$. The [sample mean](../../../../../sample-mean.md) attains this [Cramér-Rao bound](../../../../../cramer-rao-bound.md) exactly. **There is no variance advantage in preferring $S$ to $\bar Y$.**

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
