<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $y=0,1,2,\ldots$ and $\lambda>0$, the [Poisson distribution](../../../../../../poisson-distribution.md) has mass

$$
\Pr(Y=y)=\frac{e^{-\lambda}\lambda^y}{y!}
=\exp\{y\log\lambda-\lambda-\log(y!)\}.
$$

Match this to the [exponential dispersion family](../../../../../../exponential-dispersion-model.md) with

$$
\boxed{\theta=\log\lambda,\quad b(\theta)=e^\theta,\quad
\phi=1,\quad c(y,1)=-\log(y!).}
$$

Then $\mu=b'(\theta)=e^\theta=\lambda$ and $V(\mu)=b''(\theta)=\mu$. The [canonical link function](../../../../../../canonical-link-function.md) expresses the [natural parameter](../../../../../../natural-parameter-of-an-exponential-family.md) in terms of the mean, so the [Poisson canonical link](../../../../../../poisson-canonical-link.md) is **$g(\mu)=\log\mu$**. Its conditional [variance](../../../../../../variance-split.md) equals its conditional mean.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
