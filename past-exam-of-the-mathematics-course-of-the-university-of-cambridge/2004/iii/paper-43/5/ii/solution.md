<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For equal prior probabilities, $b=\tfrac12a^T(\mu_1+\mu_2)$. The projected score is [normal](../../../../../../normal-distribution.md) under either class because it is a [linear image of a multivariate normal vector](../../../../../../linear-image-of-a-multivariate-normal-vector.md), and its [variance](../../../../../../variance-split.md) is

$$
a^TVa=(\mu_1-\mu_2)^TV^{-1}(\mu_1-\mu_2)=\delta^2.
$$

Moreover $a^T\mu_1-a^T\mu_2=\delta^2$, so the midpoint threshold lies $\delta^2/2$ from either projected [mean](../../../../../../expected-value.md). Hence

$$
a^TX-b\mid C_1\sim N(\delta^2/2,\delta^2),\qquad a^TX-b\mid C_2\sim N(-\delta^2/2,\delta^2).
$$

Standardizing the two [normal distributions](../../../../../../normal-distribution.md), with $\Phi$ the [standard normal distribution function](../../../../../../standard-normal-distribution-function.md), gives

$$
\boxed{P(\text{assign }C_2\mid C_1)=\Phi(-\delta/2)=P(\text{assign }C_1\mid C_2).}
$$

Thus the [equal-covariance Gaussian classification error](../../../../../../equal-covariance-gaussian-classification-error.md) is $p(\delta)=\Phi(-\delta/2)$. The [Mahalanobis distance](../../../../../../mahalanobis-distance.md) $\delta$ between the class [means](../../../../../../expected-value.md) is their separation in units of within-class noise. It yields $p\to1/2$ as $\delta\downarrow0$ and $p\to0$ as $\delta\to\infty$. The stipulated $\delta>0$ means the two class [means](../../../../../../expected-value.md) are distinct.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
