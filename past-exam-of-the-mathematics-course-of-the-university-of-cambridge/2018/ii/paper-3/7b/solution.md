<h1 id="7b/solution">Solution</h1>

↑ **Parent:** [7B](../7b.md)

On the slit plane $\mathbb C\setminus[-a,a]$, choose

$$
F(z)=\sqrt{z-a}\sqrt{z+a}
$$

so that $F(z)\sim z$ as $z\to\infty$. This [branch cut](../../../../../branch-cut.md) gives, for $-a<x<a$, the boundary values

$$
F_+(x)=i\sqrt{a^2-x^2},
\qquad
F_-(x)=-i\sqrt{a^2-x^2}.
$$

Integrate $F$ over the boundary of a large disk with a thin slit removed. The upper bank is traversed from $-a$ to $a$ and the lower bank from $a$ to $-a$, so together they contribute

$$
2i\int_{-a}^{a}\sqrt{a^2-x^2}\,dx.
$$

At infinity the [Laurent series](../../../../../laurent-series.md) is

$$
F(z)=z\left(1-\frac{a^2}{z^2}\right)^{1/2}
=z-\frac{a^2}{2z}+O(z^{-3}),
$$

and hence the counterclockwise large-circle integral tends to $-\pi i a^2$. By the [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md), the large-circle and slit-boundary contributions sum to zero. Therefore

$$
-\pi i a^2+2i\int_{-a}^{a}\sqrt{a^2-x^2}\,dx=0,
$$

which yields

$$
\boxed{\int_{-a}^{a}\sqrt{a^2-x^2}\,dx=\frac{\pi a^2}{2}.}
$$

## ↑ Ancestors (10)

1. [7B](../7b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
