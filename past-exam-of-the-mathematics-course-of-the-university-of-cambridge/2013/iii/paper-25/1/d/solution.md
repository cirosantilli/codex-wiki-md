<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The density $Z=\exp(X(k)-\|k\|^2/2)$ is strictly positive. The [Gaussian moment-generating function](../../../../../../moment-generating-function-of-a-normal-distribution.md) gives $\mathbb E Z=1$, so it defines an [equivalent probability measure](../../../../../../equivalent-probability-measure.md).

The joint [normal distribution](../../../../../../normal-distribution.md) of $(X(h),X(k))$, with [covariance](../../../../../../covariance.md) $\langle h,k\rangle$, gives the mixed exponential formula

$$
\mathbb E_{\mathbb P}e^{X(k)+i\theta X(h)}=\exp\left(\frac12\|k\|^2+i\theta\langle h,k\rangle-\frac12\theta^2\|h\|^2\right).
$$

Multiplying by the normalizing and centring factors therefore yields

$$
\mathbb E_{\mathbb Q}e^{i\theta(X(h)-\langle h,k\rangle)}=\exp\left(-\frac12\theta^2\|h\|^2\right).
$$

The [characteristic function](../../../../../../characteristic-function.md) identifies the answer:

$$
\boxed{X(h)-\langle h,k\rangle\sim N(0,\|h\|^2)\quad\text{under }\mathbb Q.}
$$

This is [exponential tilting of an isonormal Gaussian process](../../../../../../exponential-tilting-of-an-isonormal-gaussian-process.md): the mean shifts by the inner product while its [covariance](../../../../../../covariance.md) remains unchanged.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
