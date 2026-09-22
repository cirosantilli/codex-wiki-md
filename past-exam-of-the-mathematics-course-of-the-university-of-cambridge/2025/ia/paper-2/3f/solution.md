<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

Since $Y=\int_0^\infty\mathbf1_{\{Y\ge y\}}\,dy$, Tonelli's theorem gives

$$
\mathbb E Y=\int_0^\infty\mathbb P(Y\ge y)\,dy.
$$

For the integer-valued minimum,

$$
\mathbb E M=\sum_{k=1}^n\mathbb P(M\ge k)
=\sum_{j=0}^{n-1}\left(1-\frac jn\right)^n
\le\sum_{j=0}^\infty e^{-j}=\frac e{e-1}<e.
$$

Markov's inequality now gives

$$
\boxed{\mathbb P(M\ge6)\le\frac{\mathbb E M}{6}<\frac e6<\frac12.}
$$

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
