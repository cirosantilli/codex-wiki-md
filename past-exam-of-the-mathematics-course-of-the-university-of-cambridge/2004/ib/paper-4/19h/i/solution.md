<h1 id="19h/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Under [squared-error loss](../../../../../../squared-error-loss.md), the [posterior expected loss](../../../../../../posterior-expected-loss.md) decomposes as

$$
\mathbb E[(\theta-a)^2\mid x]=\operatorname{Var}(\theta\mid x)+(a-\mathbb E[\theta\mid x])^2.
$$

It is uniquely minimized by the posterior mean. Integrating the Gamma posterior gives $\mathbb E[\theta\mid x]=b^2\int_0^\infty\theta^2e^{-b\theta}d\theta=2/b$. Hence the [Bayes estimator](../../../../../../bayes-estimator.md) is

$$
\boxed{\widehat\theta_B(X)=\frac{2}{\mu+X}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [19H](../../19h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
