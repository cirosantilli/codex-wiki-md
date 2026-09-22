<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $B=\|b\|_\infty$ and define the [scale function of a one-dimensional diffusion](../../../../../../scale-function-stochastic-processes.md)

$$
\boxed{
g(x)=\int_0^x
\exp\left(-2\int_0^u b(v)\,dv\right)\,du.}
$$

Since $b$ is continuous, $g\in C^2$, and

$$
g'(x)=\exp\left(-2\int_0^x b(v)\,dv\right)>0,\qquad
g''(x)=-2b(x)g'(x).
$$

Thus $g$ is strictly increasing. The [Itô formula](../../../../../../ito-s-lemma.md) for the additive-noise equation gives

$$
d\,g(X_t)
=\left(b(X_t)g'(X_t)+\frac12g''(X_t)\right)dt+g'(X_t)dW_t
=g'(X_t)dW_t.
$$

The integrand is locally square-integrable: a continuous path $X$ has compact range on every finite interval, where $g'$ is bounded. Hence

$$
\boxed{Y_t=g(X_t)\text{ is a continuous local martingale}.}
$$

This is the [scale transform for an additive-noise diffusion](../../../../../../scale-transform-for-an-additive-noise-diffusion.md). Its range is the open interval $I=g(\mathbb R)$, which need not be all of $\mathbb R$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
