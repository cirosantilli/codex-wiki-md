<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The nonnegative series in part (b) has independent squared-standard-normal terms. If $G$ is standard normal, direct Gaussian integration gives $\mathbb E e^{-aG^2}=(1+2a)^{-1/2}$ for $a\geq0$. Consequently, by independence and [dominated convergence](../../../../../../dominated-convergence-theorem.md) applied to the exponentials of increasing partial sums,

$$
\mathbb E\exp\left(-\lambda\int_0^1W_t^2\,dt\right)
=\prod_{n=1}^\infty\left(1+\frac{2\lambda}{(n-\tfrac12)^2\pi^2}\right)^{-1/2}.
$$

Use the permitted product identity with $x=\sqrt{2\lambda}$. The answer is

$$
\boxed{\mathbb E\exp\left(-\lambda\int_0^1W_t^2\,dt\right)=\frac1{\sqrt{\cosh\sqrt{2\lambda}}}\qquad(\lambda\geq0).}
$$

This [Laplace transform of the integrated square of Brownian motion](../../../../../../laplace-transform-of-the-integrated-square-of-brownian-motion.md) equals $1$ at zero. Its first derivative there gives mean $1/2$, in agreement with $\int_0^1\mathbb EW_t^2\,dt$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
