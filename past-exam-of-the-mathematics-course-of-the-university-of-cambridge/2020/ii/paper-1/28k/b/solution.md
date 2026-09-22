<h1 id="28k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If

$$
\sum_{n=0}^{\infty}\frac1{\lambda_n}<\infty,
$$

then

$$
\mathbb ET_\infty=\sum_{n=0}^{\infty}\mathbb EX_n
=\sum_{n=0}^{\infty}\frac1{\lambda_n}<\infty.
$$

A nonnegative random variable with finite expectation is finite almost surely, so the process explodes.

Conversely, suppose the series diverges. For $s>0$, independence and the [Laplace transform](../../../../../../laplace-transform.md) of an exponential variable give

$$
\mathbb E e^{-sT_\infty}
=\prod_{n=0}^{\infty}\frac{\lambda_n}{\lambda_n+s}
=\exp\left[-\sum_{n=0}^{\infty}
\log\left(1+\frac{s}{\lambda_n}\right)\right].
$$

The sum in the exponent diverges. If infinitely many $\lambda_n\le s$, infinitely many terms are at least $\log2$; otherwise, eventually $s/\lambda_n\le1$ and

$$
\log(1+s/\lambda_n)\ge\frac{s}{2\lambda_n}.
$$

Thus $\mathbb Ee^{-sT_\infty}=0$. Since $e^{-sT_\infty}$ is strictly positive on $\{T_\infty<\infty\}$, this forces $T_\infty=\infty$ almost surely. Hence the [nonexplosion criterion for a pure birth process](../../../../../../nonexplosion-criterion-for-a-pure-birth-process.md) is

$$
\boxed{N\text{ is nonexplosive}
\iff\sum_{n=0}^{\infty}\lambda_n^{-1}=\infty}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28K](../../28k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
