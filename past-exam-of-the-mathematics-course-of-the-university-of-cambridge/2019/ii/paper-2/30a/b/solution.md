<h1 id="30a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let

$$
I(x)=\int_x^\infty e^{-t^2}\,dt.
$$

Since $d(e^{-t^2})=-2te^{-t^2}dt$, repeated [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\begin{aligned}
I(x)
&=\frac{e^{-x^2}}{2x}
-\frac12\int_x^\infty t^{-2}e^{-t^2}\,dt\\
&=\frac{e^{-x^2}}{2x}
-\frac{e^{-x^2}}{4x^3}
+\frac34\int_x^\infty t^{-4}e^{-t^2}\,dt\\
&=\frac{e^{-x^2}}{2x}
\left(1-\frac1{2x^2}+\frac3{4x^4}
+O(x^{-6})\right).
\end{aligned}
$$

The final remainder estimate follows by one further integration by parts, or by bounding the remaining positive integral by its leading boundary term. Therefore the requested first three terms are

$$
\boxed{\operatorname{erfc}(x)
\sim\frac{e^{-x^2}}{2\sqrt{2\pi}\,x}
\left(1-\frac1{2x^2}+\frac3{4x^4}\right).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30A](../../30a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
