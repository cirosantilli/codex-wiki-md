<h1 id="5a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

On the active interval the excess temperature satisfies $\theta_2'+a\theta_2=-1$. Multiplication by the [integrating factor](../../../../../../integrating-factor.md) $e^{at}$ and integration from time one gives

$$
e^{at}\theta_2(t)-e^a\theta_2(1)=-\int_1^t e^{as}\,ds
=-\frac{e^{at}-e^a}{a}.
$$

There is no impulse in this equation, so [continuity](../../../../../../continuous-function.md) supplies $\theta_2(1)=(T_0-T_\infty)e^{-a}$. Therefore

$$
\boxed{T_2(t)=T_\infty-\frac1a+
 e^{-at}\left(T_0-T_\infty+\frac{e^a}{a}\right),\qquad1<t<2.}
$$

The equivalent correction to the common unforced temperature is $-(1-e^{-a(t-1)})/a$, which vanishes continuously at the beginning of the interval.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5A](../../5a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
