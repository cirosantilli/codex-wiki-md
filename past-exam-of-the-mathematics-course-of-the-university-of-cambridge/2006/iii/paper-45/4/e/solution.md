<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The acceptance [probability](../../../../../../probability.md) is the prior average of the Poisson [likelihood](../../../../../../likelihood-function.md):

$$
\boxed{A_k=E_{\theta,T}\left[e^{-\theta L/2}\frac{(\theta L/2)^k}{k!}\right]=Z_k=P_{\rm prior}(S=k).}
$$

Thus the expected number of proposals per accepted draw is $1/Z_k$. A numerical rate depends on the specified prior, sample size and observed count; it is not determined by $k$ alone.

For a more explicit one-dimensional expression, condition on $\theta$. The [probability generating function](../../../../../../probability-generating-function.md), integrating each independent exponential epoch, is

$$
E[z^S\mid\theta]
=E[e^{-\theta(1-z)L/2}]
=\prod_{j=2}^n\frac{\lambda_j}{\lambda_j+\theta j(1-z)/2}
=\prod_{i=1}^{n-1}\frac{i}{i+\theta(1-z)}.
$$

Let $p_k(\theta)$ be its coefficient of $z^k$. Then $Z_k=\int\pi(\theta)p_k(\theta)\,d\theta$. This identifies the acceptance rate with a fully specified marginal [likelihood](../../../../../../likelihood-function.md) average.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
