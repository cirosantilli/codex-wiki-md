<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $\lambda>0$, write the [Poisson distribution](../../../../../../poisson-distribution.md) mass function in [exponential dispersion family](../../../../../../exponential-dispersion-model.md) form:

$$
f(y;\lambda)=\exp\left\{\frac{y\theta-b(\theta)}{a(\phi)}+c(y,\phi)\right\},\quad
\theta=\log\lambda,\quad b(\theta)=e^\theta,\quad a(\phi)=\phi=1,\quad c(y,1)=-\log(y!).
$$

Thus the [natural parameter of an exponential family](../../../../../../natural-parameter-of-an-exponential-family.md) is **$\theta=\log\lambda$** and the [dispersion parameter](../../../../../../dispersion-parameter.md) is **fixed at $1$**. The counting-measure support is $0,1,\ldots$; there is no independent free dispersion parameter in an ordinary Poisson model. The degenerate boundary $\lambda=0$ is obtained as a limit, rather than a finite natural parameter.

The [exponential dispersion family](../../../../../../exponential-dispersion-model.md) identities give $\mathbb EY=b'(\theta)$ and $\operatorname{Var}(Y)=a(\phi)b''(\theta)$. Since both derivatives of $e^\theta$ equal $e^\theta$,

$$
\boxed{\mathbb EY=\lambda,\qquad\operatorname{Var}(Y)=\lambda.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
