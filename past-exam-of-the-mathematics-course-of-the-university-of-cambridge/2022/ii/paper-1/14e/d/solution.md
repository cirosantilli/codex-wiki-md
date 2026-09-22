<h1 id="14e/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For real $s>0$, collapse the Hankel contour onto the negative axis and use the jump in the argument of $t^{s-1}$. The reflection formula for the [gamma function](../../../../../../gamma-function.md) yields

$$
\boxed{
I(z,s)=\frac z{\Gamma(s)}
\int_0^\infty\frac{t^{s-1}}{e^t-z},dt},
$$

so $K(z,s,t)=z t^{s-1}/[\Gamma(s)(e^t-z)]$. At positive integer $s$, the original Hankel expression is interpreted by analytic continuation: the pole of $\Gamma(1-s)$ cancels the corresponding zero of the contour integral.

When $z$ crosses the slit at $x>1$, the pole of the real-integral kernel at $t=\log x$ crosses the integration path. The two boundary values differ by $2\pi i$ times its residue. Since $d(e^t-z)/dt=x$ there, that residue is $(\log x)^{s-1}/\Gamma(s)$, giving the jump

$$
\boxed{\frac{2\pi i(\log x)^{s-1}}{\Gamma(s)}}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [14E](../../14e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
