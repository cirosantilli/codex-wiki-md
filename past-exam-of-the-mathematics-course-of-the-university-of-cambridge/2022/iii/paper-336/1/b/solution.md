<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $e^x=1+xg(x)$, where $g=(e^x-1)/x$ is smooth at zero. Then

$$
\int_0^1\frac{dx}{\sqrt{x+\epsilon}}
=2-2\sqrt\epsilon+\epsilon+O(\epsilon^2),
$$

and a uniformly integrable expansion gives

$$
\int_0^1\frac{xg(x)}{\sqrt{x+\epsilon}}dx
=\int_0^1\sqrt x,g(x)dx
-\frac\epsilon2\int_0^1\frac{g(x)}{\sqrt x}dx
+O(\epsilon^{3/2}).
$$

By [integration by parts](../../../../../../integration-by-parts.md),

$$
\int_0^1\frac{e^x-1}{x^{3/2}}dx=-2(e-1)+2I(0).
$$

Therefore

$$
\boxed{I(\epsilon)=I(0)-2\sqrt\epsilon+[e-I(0)]\epsilon+O(\epsilon^{3/2}).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
