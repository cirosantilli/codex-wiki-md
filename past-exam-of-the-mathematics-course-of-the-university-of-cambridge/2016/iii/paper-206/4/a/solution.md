<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $0<p<1$, the [Bernoulli distribution](../../../../../../bernoulli-distribution.md) has mass

$$
\Pr(Y=y)=p^y(1-p)^{1-y}
=\exp\left[y\log\frac p{1-p}+\log(1-p)\right],\qquad y\in\{0,1\}.
$$

In [exponential dispersion family](../../../../../../exponential-dispersion-model.md) notation $\exp\{[y\theta-b(\theta)]/\phi+c(y,\phi)\}$, take

$$
\boxed{\theta=\log\frac p{1-p},\qquad b(\theta)=\log(1+e^\theta),\qquad\phi=1,\qquad c(y,1)=0.}
$$

The support is $\{0,1\}$; outside it the probability is zero. The [natural parameter of an exponential family](../../../../../../natural-parameter-of-an-exponential-family.md) is the [log odds](../../../../../../log-odds.md), and the [dispersion parameter](../../../../../../dispersion-parameter.md) is fixed rather than freely estimated. Differentiating the cumulant gives

$$
\boxed{\mathbb EY=b'(\theta)=\frac{e^\theta}{1+e^\theta}=p,\qquad
\operatorname{Var}(Y)=\phi b''(\theta)=\frac{e^\theta}{(1+e^\theta)^2}=p(1-p).}
$$

At $p=0$ or $1$ the degenerate distributions are limiting boundary cases with natural parameter $-\infty$ or $+\infty$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
