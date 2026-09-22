<h1 id="14a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Because $e^{-\lambda|k|}$ is an [even function](../../../../../../even-function.md), [Fourier inversion](../../../../../../fourier-inversion-theorem.md) reduces to a cosine integral:

$$
\begin{aligned}
g(x)
&=\frac1{2\pi}\int_{-\infty}^{\infty}e^{-\lambda|k|}e^{ikx}\,dk\\
&=\frac1\pi\int_0^\infty e^{-\lambda k}\cos(kx)\,dk
=\frac1\pi\operatorname{Re}\frac1{\lambda-ix}.
\end{aligned}
$$

Therefore

$$
\boxed{g(x)=\frac{\lambda}{\pi(x^2+\lambda^2)}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14A](../../14a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
