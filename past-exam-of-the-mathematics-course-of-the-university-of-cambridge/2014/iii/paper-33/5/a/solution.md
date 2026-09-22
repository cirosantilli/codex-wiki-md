<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Consider a competing interpolant $f$ and set $h=f-g$. At each [spline knot](../../../../../../spline-knot.md), $h(x_i)=0$. If its [second derivative roughness penalty](../../../../../../second-derivative-roughness-penalty.md) is infinite there is nothing to prove, so assume $f''\in L^2$. Its absolutely continuous first derivative makes $h'$ absolutely continuous as well, with $h''$ defined almost everywhere.

On each knot interval the [natural cubic spline](../../../../../../natural-cubic-spline.md) has constant third derivative. Integrating by parts once gives

$$
\int_{x_i}^{x_{i+1}}g''h''
=[g''h']_{x_i}^{x_{i+1}}-g^{(3)}|_{(x_i,x_{i+1})}\,[h]_{x_i}^{x_{i+1}}.
$$

The last term vanishes because $h$ is zero at both endpoints. Summing over intervals cancels the interior boundary terms, since $g''$ and $h'$ are continuous at the knots. The exterior terms vanish because $g''(x_1)=g''(x_n)=0$. Hence $\int g''h''=0$. Expanding the square now gives

$$
\boxed{\alpha\int_{x_1}^{x_n}(f'')^2
=\alpha\int_{x_1}^{x_n}(g'')^2
+\alpha\int_{x_1}^{x_n}(h'')^2
\ \geq\alpha\int_{x_1}^{x_n}(g'')^2.}
$$

Since $\alpha>0$, equality requires $h''=0$ almost everywhere. Absolute continuity then makes $h$ affine. It has at least two distinct zeros because $n\geq2$, so $h=0$. **The natural cubic spline is the unique minimizer.** This proves the [minimum roughness property with absolutely continuous first derivatives](../../../../../../minimum-roughness-property-with-absolutely-continuous-first-derivatives.md), covering the weaker regularity in the question rather than assuming competitors are twice continuously differentiable. The case of two knots is included: the minimizing spline is their straight-line interpolant.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
