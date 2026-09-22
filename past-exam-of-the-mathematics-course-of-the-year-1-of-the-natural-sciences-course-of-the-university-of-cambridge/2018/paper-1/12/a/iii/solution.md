<h1 id="12/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Reverse the order in the nonnegative [double integral](../../../../../../double-integral.md), using $0\le y<\infty$ and $y\le x\le2y$. For $y>0$, an [antiderivative](../../../../../../antiderivative.md) in $x$ is $-(x/y+1/y^2)e^{-xy}$. Thus

$$
I=\int_0^\infty\left[\left(1+\frac1{y^2}\right)e^{-y^2}
-\left(2+\frac1{y^2}\right)e^{-2y^2}\right]dy.
$$

Let $J$ denote the requested [improper integral](../../../../../../improper-integral.md). Its numerator is $y^2+O(y^4)$ near zero, so its apparent singularity is removable; it also decays at infinity. We may therefore separate the preceding expression into the convergent integrals

$$
I=\int_0^\infty(e^{-y^2}-2e^{-2y^2})\,dy+J
=\frac{\sqrt\pi}{2}(1-\sqrt2)+J=-I+J.
$$

It follows that

$$
\boxed{J=\int_0^\infty\frac{e^{-x^2}-e^{-2x^2}}{x^2}\,dx=\sqrt\pi(\sqrt2-1).}
$$

The two terms divided separately by $x^2$ would each have a divergent [integral](../../../../../../integral-split.md) at zero; the cancellation in their difference is essential.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [12](../../../12.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
