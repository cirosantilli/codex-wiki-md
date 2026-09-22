<h1 id="3d/solution">Solution</h1>

↑ **Parent:** [3D](../3d.md)

For an observed $x\ge0$, the [continuous uniform distribution](../../../../../continuous-uniform-distribution.md) likelihood is $p(x\mid\theta)=\theta^{-1}1_{\{\theta\ge x\}}$, with $\theta>0$. Multiplying by the stated prior cancels the factor $\theta$, giving $e^{-\theta}1_{\{\theta\ge x\}}$. Its integral over the permitted parameter values is $e^{-x}$. Hence the [posterior distribution](../../../../../bayesian-posterior.md) is

$$
\boxed{p(\theta\mid x)=e^{-(\theta-x)}1_{\{\theta\ge x\}},\qquad \theta\mid x\sim x+\operatorname{Exp}(1).}
$$

This is the [exponential posterior for a uniform endpoint](../../../../../exponential-posterior-for-a-uniform-endpoint.md). Its posterior mean is $x+1$ and its variance is one. The posterior expected [squared-error loss](../../../../../squared-error-loss.md) decomposes as

$$
E[c(\theta-a)^2\mid x]=c\operatorname{Var}(\theta\mid x)+c(a-E[\theta\mid x])^2=c+c(a-x-1)^2.
$$

Since $c>0$, its unique minimum occurs at **the Bayes estimate** $\boxed{\widehat\theta_B=x+1}$. The positive loss multiplier changes the risk, not the optimizing action.

## ↑ Ancestors (10)

1. [3D](../3d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
