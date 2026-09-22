<h1 id="20/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $d=b-a$ and $h=d/n$. The required [Riemann sum](../../../../../riemann-sum.md) is

$$
S_n=h\sum_{k=1}^n(a+kh)^2
=h\left[na^2+2ah\sum_{k=1}^nk+h^2\sum_{k=1}^nk^2\right].
$$

Using $\sum k=n(n+1)/2$ and the given sum of squares,

$$
\boxed{S_n=a^2d+ad^2\frac{n+1}{n}+d^3\frac{(n+1)(2n+1)}{6n^2}.}
$$

An equivalent expression separates its [limit](../../../../../limit-of-a-function.md) and finite-$n$ corrections:

$$
S_n=\frac{b^3-a^3}{3}+\frac{(b-a)(b^2-a^2)}{2n}+\frac{(b-a)^3}{6n^2}.
$$

Consequently

$$
\boxed{\lim_{n\to\infty}S_n=\frac{b^3-a^3}{3}=\int_a^bx^2\,dx.}
$$

The function is continuous, so the [Riemann sums](../../../../../riemann-sum.md) converge to its [definite integral](../../../../../definite-integral.md), the desired [area](../../../../../surface-area.md) under the [parabola](../../../../../parabola.md). Both corrections are positive when $0<a<b$, agreeing with the geometric fact that these right-endpoint rectangles overestimate an increasing curve.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [20](../../20.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
