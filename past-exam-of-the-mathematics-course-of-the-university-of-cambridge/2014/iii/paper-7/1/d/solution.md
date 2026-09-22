<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose $f_0(x,v)=e^{-(x^2+v^2)}$ and $h(t,x,v)=x^2+v^2$. The initial [Gaussian function](../../../../../../gaussian-function.md) is smooth and belongs to every finite [Lp space](../../../../../../lp-space.md), and is also bounded. The source is smooth and nonzero. The accumulated source along the backward [characteristic curve](../../../../../../characteristic-curve.md) is

$$
 \begin{aligned}
 q_t(x,v)&=\int_0^t|A_{s-t}(x,v)|^2\,ds\\
 &=\frac{\sinh(2t)}2(x^2+v^2)-(\cosh(2t)-1)xv.
 \end{aligned}
$$

Its quadratic-form eigenvalues are $(e^{2t}-1)/2$ and $(1-e^{-2t})/2$. Both are positive for $t>0$, so

$$
 f_t(x,v)=e^{-|A_{-t}(x,v)|^2}+q_t(x,v)
 \geq\frac{1-e^{-2t}}2(x^2+v^2).
$$

Consequently **$\|f_t\|_p=\infty$ for every $t>0$ and every finite $p\geq1$**; it is unbounded, so its $L^\infty$ [norm](../../../../../../norm.md) is infinite as well. This [spatially nonintegrable forcing in transport](../../../../../../spatially-nonintegrable-forcing-in-transport.md) example avoids any ambiguity about whether the last endpoint is included in “all $p$”.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
