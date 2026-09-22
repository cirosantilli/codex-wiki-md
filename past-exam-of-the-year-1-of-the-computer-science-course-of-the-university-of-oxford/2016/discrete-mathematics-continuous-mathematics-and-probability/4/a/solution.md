<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [partial fraction decomposition](../../../../../partial-fraction-decomposition.md):

$$
\frac1{x^2(x^2-4)}=-\frac1{4x^2}+\frac1{4(x^2-4)}
=-\frac1{4x^2}+\frac1{16}\left(\frac1{x-2}-\frac1{x+2}\right).
$$

Integrating each term gives the [antiderivative](../../../../../antiderivative.md)

$$
\boxed{\int\frac{dx}{x^2(x^2-4)}=\frac1{4x}+\frac1{16}\log\left|\frac{x-2}{x+2}\right|+C.}
$$

This holds on any interval avoiding $-2,0,2$; the constant may differ between these intervals. [Differentiation](../../../../../differentiation.md) of the logarithm recovers $1/[4(x^2-4)]$, providing a direct check.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
