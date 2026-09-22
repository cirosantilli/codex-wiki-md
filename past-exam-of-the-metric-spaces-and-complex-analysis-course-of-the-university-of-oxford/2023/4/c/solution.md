<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [c](../c.md)

Use the local factorization for a [pole](../../../../pole.md) of order $n$:

$$
f(z)=(z-a)^{-n}h(z),\qquad h(a)\ne0.
$$

Shrink the disc so that the [holomorphic function](../../../../holomorphic-function-split.md) $h$ has no zeros there. Differentiating and dividing gives the [logarithmic derivative](../../../../logarithmic-derivative.md)

$$
\boxed{\frac{f'(z)}{f(z)}=-\frac n{z-a}+\frac{h'(z)}{h(z)}}.
$$

The second term is [holomorphic](../../../../holomorphic-function-split.md) across $a$. Since $n\geq1$, the first term cannot cancel. Hence $f'/f$ has a [simple pole](../../../../simple-pole.md), and the coefficient of $(z-a)^{-1}$ in its [Laurent series](../../../../laurent-series.md) is

$$
\boxed{\operatorname{Res}_a(f'/f)=-n}.
$$

This is the pole case of the [integer residue of a logarithmic derivative](../../../../integer-residue-of-a-logarithmic-derivative.md).

## ↑ Ancestors (12)

1. [c](../c.md)
2. [4](../../4.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
