<h1 id="28k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take the proposal density $h(x)=e^{-x}\mathbf1_{x\geq0}$. For the target [half-normal distribution](../../../../../../half-normal-distribution.md),

$$
\frac{f(x)}{h(x)}
=\sqrt{\frac2\pi}\exp\left(-\frac{x^2}{2}+x\right)
=\sqrt{\frac{2e}{\pi}}\exp\left(-\frac{(x-1)^2}{2}\right).
$$

The ratio is maximized at $x=1$, so the sharp envelope constant is

$$
\boxed{M=\sqrt{\frac{2e}{\pi}}}.
$$

Generate $X=-\log U_1$ and an independent uniform $U_2$, and accept $X$ when

$$
U_2\leq\frac{f(X)}{Mh(X)}
=e^{-(X-1)^2/2}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28K](../../28k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
