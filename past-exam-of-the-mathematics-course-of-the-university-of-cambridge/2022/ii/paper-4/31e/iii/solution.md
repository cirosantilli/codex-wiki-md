<h1 id="31e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write the normal-form equation as

$$
u''=Q(x)u,
\qquad
Q(x)=\frac1{x^4}-\frac1{4x^2}.
$$

For sufficiently small positive $x$, $Q(x)>0$. Moreover,

$$
\frac{|Q'(x)|}{Q(x)^{3/2}}=O(x)\longrightarrow0,
$$

and the corresponding higher derivative condition also tends to zero, so the amplitude varies slowly relative to the exponential phase and the [Liouville-Green approximation](../../../../../../wkb-approximation.md) applies.

The phase and amplitude have expansions

$$
\begin{aligned}
\sqrt{Q(x)}
&=x^{-2}\left(1-\frac{x^2}{8}
-\frac{x^4}{128}+O(x^6)\right),\\
Q(x)^{-1/4}
&=x\left(1+\frac{x^2}{16}+O(x^4)\right),\\
\int^x\sqrt{Q(s)}\,ds
&=-\frac1x-\frac x8-\frac{x^3}{384}+O(x^5).
\end{aligned}
$$

Hence two independent Liouville-Green solutions satisfy

$$
\boxed{
u_\pm(x)\sim Q(x)^{-1/4}
\exp\left(\pm\int^x\sqrt{Q(s)}\,ds\right)}.
$$

In particular, after choosing the signs according to growth and decay,

$$
u_{\rm grow}(x)\sim xe^{1/x}\left(1+\frac x8+\frac{9x^2}{128}+\cdots\right),
\qquad
u_{\rm decay}(x)\sim xe^{-1/x}\left(1-\frac x8+\frac{9x^2}{128}+\cdots\right).
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [31E](../../31e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
