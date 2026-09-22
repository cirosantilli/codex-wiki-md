<h1 id="19d/solution">Solution</h1>

↑ **Parent:** [19D](../19d.md)

For observed data $x$, let $F_x$ be the [posterior](../../../../../bayesian-posterior.md) [cumulative distribution function](../../../../../cumulative-distribution-function.md). Assuming finite [posterior](../../../../../bayesian-posterior.md) first moment, the [posterior](../../../../../bayesian-posterior.md) risk under [asymmetric absolute-error loss](../../../../../asymmetric-absolute-error-loss.md) is

$$
R_x(a)=\gamma\int_a^\infty(\theta-a)\pi(\theta\mid x)d\theta
+\delta\int_{-\infty}^a(a-\theta)\pi(\theta\mid x)d\theta.
$$

At points where the [posterior](../../../../../bayesian-posterior.md) has a density, differentiation gives $R_x'(a)=(\gamma+\delta)F_x(a)-\gamma$. Risk is convex, so a global minimum is a [posterior](../../../../../bayesian-posterior.md) [quantile](../../../../../quantile-function.md):

$$
\boxed{a(x)=F_x^{-1}\left(\frac\gamma{\gamma+\delta}\right).}
$$

More generally any $a$ with $F_x(a^-)\leq\gamma/(\gamma+\delta)\leq F_x(a)$ minimizes risk. This is the [Bayes quantile under asymmetric absolute-error loss](../../../../../bayes-quantile-under-asymmetric-absolute-error-loss.md); a larger cost for underestimation moves the chosen [quantile](../../../../../quantile-function.md) upward.

For the uniform sampling model set $M=\max_iX_i$. For a valid positive sample the [likelihood](../../../../../likelihood-function.md) is $\theta^{-n}\mathbf1_{\{\theta>M\}}$. Multiplying by the [prior](../../../../../prior-probability.md) cancels its power of $\theta$ and gives [posterior](../../../../../bayesian-posterior.md) density proportional to $e^{-\theta}\mathbf1_{\{\theta>M\}}$. Normalization yields

$$
\pi(\theta\mid x)=e^{-(\theta-M)}\mathbf1_{\{\theta>M\}},\qquad
F_x(a)=1-e^{-(a-M)}\quad(a\geq M).
$$

Solving the [quantile](../../../../../quantile-function.md) equation gives the explicit Bayes estimate

$$
\boxed{a(X_1,\ldots,X_n)=M+\log\left(\frac{\gamma+\delta}{\delta}\right).}
$$

The [posterior](../../../../../bayesian-posterior.md) is the sample maximum plus a unit-rate [exponential distribution](../../../../../exponential-distribution.md) displacement; it has finite first moment, so the preceding risk minimization is justified here.

## ↑ Ancestors (10)

1. [19D](../19d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
