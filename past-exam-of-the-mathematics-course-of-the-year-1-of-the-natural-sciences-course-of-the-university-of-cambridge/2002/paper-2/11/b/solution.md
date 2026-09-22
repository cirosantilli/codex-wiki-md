<h1 id="11/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiate $v_t=yu_x-xu_y$ with respect to $t$, remembering that its coefficients also depend on $t$. The [product rule](../../../../../product-rule.md) and [multivariable chain rule](../../../../../multivariable-chain-rule.md) give

$$
\begin{aligned}
v_{tt}&=y_tu_x+y(u_{xx}x_t+u_{xy}y_t)-x_tu_y-x(u_{yx}x_t+u_{yy}y_t)\\
&=-xu_x+y(yu_{xx}-xu_{xy})-yu_y-x(yu_{yx}-xu_{yy}).
\end{aligned}
$$

For a twice continuously differentiable $u$, equality of [mixed partial derivatives](../../../../../mixed-partial-derivative.md) gives $u_{yx}=u_{xy}$. Hence

$$
\boxed{v_{tt}=y^2u_{xx}-2xyu_{xy}+x^2u_{yy}-xu_x-yu_y.}
$$

The first-order terms come from differentiating $x$ and $y$ themselves; treating $y\partial_x-x\partial_y$ as an operator with constant coefficients would miss them.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [11](../../11.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
