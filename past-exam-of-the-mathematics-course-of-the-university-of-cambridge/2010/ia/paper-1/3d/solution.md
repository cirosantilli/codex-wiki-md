<h1 id="3d/solution">Solution</h1>

↑ **Parent:** [3D](../3d.md)

A [power series](../../../../../power-series.md) has [radius of convergence](../../../../../radius-of-convergence.md) $R$ when it converges absolutely for every $|z|<R$ and diverges for every $|z|>R$. Its behaviour on $|z|=R$ is not specified by this definition. When $R=0$, it converges at the centre and diverges at every nonzero point; an infinite [radius of convergence](../../../../../radius-of-convergence.md) means [absolute convergence](../../../../../absolute-convergence.md) at every finite $z$.

Suppose, towards a contradiction, that $|a_nz^n|\leq M$ for all $n$ at some $|z|>R$. Choose a [complex number](../../../../../complex-number.md) $w$ with $R<|w|<|z|$. Then

$$
|a_nw^n|=|a_nz^n|\left(\frac{|w|}{|z|}\right)^n
\leq Mq^n,\qquad q=\frac{|w|}{|z|}<1.
$$

The [comparison test for series](../../../../../comparison-test-for-series.md) with the convergent [geometric series](../../../../../geometric-series.md) $\sum Mq^n$ yields [absolute convergence](../../../../../absolute-convergence.md) at $w$, contradicting the definition of $R$. Thus [terms of a power series are unbounded outside its convergence disc](../../../../../terms-of-a-power-series-are-unbounded-outside-its-convergence-disc.md):

$$
\boxed{|z|>R\ \Longrightarrow\ (|a_nz^n|)_{n\geq0}\text{ is unbounded}.}
$$

For the given [power series](../../../../../power-series.md), the [ratio test](../../../../../ratio-test.md) gives, when $z\ne0$,

$$
\frac{|z|^{n+1}/(n+1)^3}{|z|^n/n^3}
=|z|\left(\frac n{n+1}\right)^3\longrightarrow |z|.
$$

Hence it converges absolutely for $|z|<1$ and its terms fail to tend to zero for $|z|>1$ (the ratios are eventually larger than some number greater than $1$). Therefore $\boxed{R=1}$. In fact, on $|z|=1$ it also converges absolutely by comparison with the convergent [p-series](../../../../../p-series.md) $\sum n^{-3}$.

## ↑ Ancestors (10)

1. [3D](../3d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
