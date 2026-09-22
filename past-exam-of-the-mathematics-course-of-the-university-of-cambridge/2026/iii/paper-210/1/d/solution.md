<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A centered [random variable](../../../../../../random-variable-split.md) $Y$ is [sub-Gaussian](../../../../../../sub-gaussian-distribution.md) with variance parameter $\sigma^2$ when

$$
\log\mathbb E e^{\lambda Y}\leq\frac{\sigma^2\lambda^2}{2}
\qquad(\lambda\in\mathbb R).
$$

The [Chernoff bound](../../../../../../chernoff-bound.md), applied to $Y$ and $-Y$, yields

$$
\mathbb P(|Y|\geq t)\leq2e^{-t^2/(2\sigma^2)}.
$$

The [tail integral formula for moments](../../../../../../tail-integral-formula-for-moments.md) and the substitution $u=t^2/(2\sigma^2)$ now give

$$
\begin{aligned}
\mathbb E|Y|^q
&=q\int_0^\infty t^{q-1}\mathbb P(|Y|\geq t)\,dt\\
&\leq2q\int_0^\infty t^{q-1}e^{-t^2/(2\sigma^2)}\,dt
=2\Gamma\left(\frac q2+1\right)(2\sigma^2)^{q/2}.
\end{aligned}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 210](../../../paper-210-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
