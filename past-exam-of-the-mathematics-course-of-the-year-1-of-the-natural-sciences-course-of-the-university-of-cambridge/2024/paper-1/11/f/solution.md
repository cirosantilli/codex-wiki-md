<h1 id="11/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For $\theta\notin2\pi\mathbb Z$, use the [finite geometric series](../../../../../finite-geometric-series.md) with ratio $e^{i\theta}$:

$$
\sum_{n=0}^{N-1}e^{in\theta}=\frac{1-e^{iN\theta}}{1-e^{i\theta}}=e^{i(N-1)\theta/2}\frac{\sin(N\theta/2)}{\sin(\theta/2)}.
$$

The second equality follows by factoring $1-e^{it}=-2ie^{it/2}\sin(t/2)$ in numerator and denominator. Taking [real parts](../../../../../real-part.md) proves the [finite trigonometric sum](../../../../../finite-trigonometric-sum.md) identity

$$
\boxed{\sum_{n=0}^{N-1}\cos(n\theta)=\frac{\cos((N-1)\theta/2)\sin(N\theta/2)}{\sin(\theta/2)}.}
$$

When $\theta=2p\pi$, every [cosine](../../../../../cosine.md) is $1$, so the [sum](../../../../../sum.md) is $\boxed{N}$. This also gives the continuous limiting value at the excluded arguments.

## ↑ Ancestors (13)

1. [F](../f.md)
2. [11](../../11.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
