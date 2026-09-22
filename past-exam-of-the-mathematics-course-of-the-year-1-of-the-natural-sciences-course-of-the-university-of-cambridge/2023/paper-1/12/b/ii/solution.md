<h1 id="12/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The horizontal cross-section is a [triangle](../../../../../../triangle.md), so its [area](../../../../../../surface-area.md) is half its width times its depth:

$$
A(z)=LD\left(1-\frac zH\right)\sqrt{1-\frac z{2H}}.
$$

Thus the [volume integral](../../../../../../volume-integral.md), with $t=z/H$, is

$$
V=LDH\int_0^1(1-t)\sqrt{1-t/2}\,dt.
$$

For the [substitution rule](../../../../../../integration-by-substitution.md), put $u=1-t/2$. The endpoint values are $1$ and $1/2$, and $1-t=2u-1$, giving

$$
\begin{aligned}
\frac V{LDH}&=2\int_{1/2}^1(2u-1)u^{1/2}\,du\\
&=2\left[\frac45u^{5/2}-\frac23u^{3/2}\right]_{1/2}^1\\
&=\frac{4+2\sqrt2}{15}.
\end{aligned}
$$

Therefore $\boxed{V=\dfrac{(4+2\sqrt2)LDH}{15}}$.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [12](../../../12.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
