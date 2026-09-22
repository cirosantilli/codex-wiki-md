<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For an observed [random sample](../../../../../../../independent-and-identically-distributed-random-variables.md) with all $x_i>0$, which happens [almost surely](../../../../../../../almost-sure-convergence.md), [independence](../../../../../../../independent-random-variables.md) gives the [likelihood function](../../../../../../../likelihood-function.md)

$$
L(\theta)=\prod_{i=1}^n\frac{2x_i}{\theta}e^{-x_i^2/\theta}=2^n\left(\prod_{i=1}^nx_i\right)\theta^{-n}\exp\left(-\frac{S}{\theta}\right),\qquad S=\sum_{i=1}^nx_i^2>0.
$$

Ignoring a term independent of $\theta$, the [log-likelihood](../../../../../../../log-likelihood.md) and its [derivative](../../../../../../../derivative.md) are

$$
\ell(\theta)=-n\log\theta-\frac S\theta+C,\qquad \ell'(\theta)=\frac{S-n\theta}{\theta^2}.
$$

This [derivative](../../../../../../../derivative.md) is positive for $0<\theta<S/n$ and negative for $\theta>S/n$. Thus there is a unique [global maximum](../../../../../../../global-maximum.md), and the [maximum-likelihood estimator](../../../../../../../maximum-likelihood-estimator.md) is

$$
\boxed{\widehat\theta(\mathbf X)=\frac1n\sum_{i=1}^nX_i^2.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
