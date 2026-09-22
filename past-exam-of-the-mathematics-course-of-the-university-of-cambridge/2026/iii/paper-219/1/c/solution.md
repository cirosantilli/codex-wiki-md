<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [inverse-square law](../../../../../../inverse-square-law.md) gives $f_s=L_0/(4\pi r_s^2)$, so a star is observed exactly when

$$
r_s\leq R=\sqrt{\frac{L_0}{4\pi f_{\min}}}.
$$

Writing $a=R/r_0$, integration of the shape-three gamma density gives

$$
\mathbb P(r_s\leq R)=1-e^{-a}\left(1+a+\frac{a^2}{2}\right).
$$

Therefore the fully normalized [truncated distribution](../../../../../../truncated-distribution.md) is

$$
\boxed{p(r_s\mid I_s=1)=
\frac{r_s^2e^{-r_s/r_0}}
{2r_0^3\left[1-e^{-a}(1+a+a^2/2)\right]}
\mathbf1_{(0,R]}(r_s).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
