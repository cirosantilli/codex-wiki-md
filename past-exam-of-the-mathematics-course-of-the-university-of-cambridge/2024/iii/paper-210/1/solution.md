<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A centered random variable $X$ is a [Sub-Gamma random variable in the right tail](../../../../../sub-gamma-random-variable-in-the-right-tail.md) with variance factor $\sigma^2$ and scale parameter $c$ when

$$
\log\mathbb Ee^{\lambda X}
\leq\frac{\sigma^2\lambda^2}{2(1-c\lambda)}
\qquad(0\leq\lambda<c^{-1}).
$$

The [Chernoff bound](../../../../../chernoff-bound.md) with $\lambda=x/(\sigma^2+cx)$ gives

$$
\mathbb P(X\geq x)
\leq\exp\left\{-\frac{x^2}{2(\sigma^2+cx)}\right\}.
$$

If $cx\leq\sigma^2$, the exponent is at least $x^2/(4\sigma^2)$; if $cx\geq\sigma^2$, it is at least $x/(4c)$. Hence

$$
\mathbb P(X\geq x)
\leq\max\left\{e^{-x^2/(4\sigma^2)},e^{-x/(4c)}\right\}.
$$

[Bernstein's inequality](../../../../../bernstein-inequalities-probability-theory.md) states that if $Z_1,\ldots,Z_n$ are independent, centered, $Z_i\leq b$ almost surely, and $v=\sum_i\mathbb EZ_i^2$, then

$$
\mathbb P\left(\sum_iZ_i\geq x\right)
\leq\exp\left\{-\frac{x^2}{2(v+bx/3)}\right\}.
$$

For $0\leq\lambda<3/b$, the elementary exponential-series bound gives

$$
e^{\lambda z}
\leq1+\lambda z+
\frac{\lambda^2z^2}{2(1-\lambda b/3)}
\qquad(z\leq b).
$$

For $z\leq0$ this follows from $e^u-1-u\leq u^2/2$, and for $0<z\leq b$ it follows by bounding the higher powers using $k!\geq2\,3^{k-2}$. Taking expectations, using $\log u\leq u-1$, and then independence yields

$$
\log\mathbb E\exp\left(\lambda\sum_iZ_i\right)
\leq\frac{v\lambda^2}{2(1-\lambda b/3)}.
$$

Thus the sum is sub-Gamma with parameters $(v,b/3)$, and the preceding Chernoff calculation proves Bernstein's inequality.

For the [empirical distribution function](../../../../../empirical-distribution-function.md), set $q=1-F(x)$ and

$$
Z_i=\mathbf1_{\{X_i\leq x\}}-F(x).
$$

Then $Z_i\leq q$, $\mathbb EZ_i^2=F(x)q$, and

$$
F_n(x)-F(x)=\frac1n\sum_iZ_i.
$$

The inverted Bernstein bound gives, with probability at least $1-\delta$,

$$
F_n(x)-F(x)
\leq\sqrt{\frac{2F(x)q\log(1/\delta)}n}
+\frac{q\log(1/\delta)}{3n}.
$$

Since $\sqrt2\leq2$ and $1/3\leq4/3$, this implies the stated bound.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
