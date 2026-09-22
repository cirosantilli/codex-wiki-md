<h1 id="27j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $f=\mathbf1_{[-1,1]}$, part (b) gives $\widehat f(u)=2\sin u/u$. The [Plancherel theorem](../../../../../../plancherel-theorem.md) in the stated Fourier convention gives

$$
\int_{\mathbb R}|f(x)|^2\,dx
=\frac1{2\pi}\int_{\mathbb R}|\widehat f(u)|^2\,du.
$$

Since the left side is two,

$$
2=\frac1{2\pi}\int_{\mathbb R}4\left(\frac{\sin u}{u}\right)^2du.
$$

The integrand is even, so the [sinc-squared integral](../../../../../../sinc-squared-integral.md) is

$$
\boxed{\ \int_0^\infty\left(\frac{\sin x}{x}\right)^2dx=\frac\pi2.\ }
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [27J](../../27j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
