<h1 id="7a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the suggested substitution

$$
x=\frac{t}{\sqrt{2-t^2}}.
$$

It maps $[0,1]$ to itself and satisfies

$$
dx=\frac{2\,dt}{(2-t^2)^{3/2}},
\qquad
1-x^4=\frac{4(1-t^2)}{(2-t^2)^2}.
$$

Hence

$$
\int_0^1\frac{dx}{\sqrt{1-x^4}}
=\frac1{\sqrt2}\int_0^1
\frac{dt}{\sqrt{(1-t^2)(1-t^2/2)}}
=\frac1{\sqrt2}K(1/\sqrt2),
$$

where $K$ is the [complete elliptic integral of the first kind](../../../../../../complete-elliptic-integral-of-the-first-kind.md). Part (a) and the [Gamma function recurrence](../../../../../../gamma-function-recurrence.md) $\Gamma(5/4)=\Gamma(1/4)/4$ now give

$$
\boxed{K(1/\sqrt2)
=\frac{\Gamma(1/4)^2}{4\sqrt\pi}
=\frac{4\Gamma(5/4)^2}{\sqrt\pi}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7A](../../7a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
