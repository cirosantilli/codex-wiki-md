<h1 id="31d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiation under the integral sign gives

$$
U'(x)=-\int_0^\infty\frac{te^{-xt}}{1+t}\,dt,
\qquad
U''(x)=\int_0^\infty\frac{t^2e^{-xt}}{1+t}\,dt.
$$

Hence

$$
\begin{aligned}
xU''+(1-x)U'-U
&=\int_0^\infty e^{-xt}
\frac{xt^2-(1-x)t-1}{1+t}\,dt\\
&=\int_0^\infty e^{-xt}(xt-1)\,dt\\
&=x\frac1{x^2}-\frac1x=0.
\end{aligned}
$$

Thus

$$
\boxed{xU''(x)+(1-x)U'(x)-U(x)=0}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [31D](../../31d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
