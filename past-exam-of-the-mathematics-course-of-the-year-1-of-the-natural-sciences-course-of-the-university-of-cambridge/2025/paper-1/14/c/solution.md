<h1 id="14/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here $a=0$, so the [probability density function](../../../../../probability-density-function.md) is the [even function](../../../../../even-function.md) $\cos x$ on $[-h,h]$, where $h=\pi/6$. Hence $\mathbb E[X]=0$ by [oddness](../../../../../odd-function.md), and the [variance](../../../../../variance-split.md) is just $\mathbb E[X^2]$. Two applications of [integration by parts](../../../../../integration-by-parts.md) give

$$
\int x^2\cos x\,dx=x^2\sin x+2x\cos x-2\sin x+C.
$$

Thus

$$
\operatorname{Var}(X)=2\left[h^2\sin h+2h\cos h-2\sin h\right]=\boxed{\frac{\pi^2}{36}+\frac{\pi\sqrt3}{3}-2}.
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [14](../../14.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
