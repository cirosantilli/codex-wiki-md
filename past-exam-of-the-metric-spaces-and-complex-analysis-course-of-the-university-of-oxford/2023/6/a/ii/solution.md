<h1 id="6/a/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

At $z_0$, [complex differentiability](../../../../../complex-differentiability.md) gives

$$
f(z_0+h)=f(z_0)+f'(z_0)h+o(|h|).
$$

Writing $f'(z_0)=\lambda e^{i\alpha}$, the assumption $f'(z_0)\ne0$ gives $\lambda>0$. Its real derivative is therefore the similarity $h\mapsto\lambda e^{i\alpha}h$, a rotation through $\alpha$ followed by scaling by $\lambda$.

More explicitly, for two differentiable curves $\gamma_1,\gamma_2$ with $\gamma_j(0)=z_0$ and nonzero tangent vectors, the [chain rule](../../../../../chain-rule.md) gives

$$
(f\circ\gamma_j)'(0)=f'(z_0)\gamma_j'(0),\qquad
\frac{(f\circ\gamma_2)'(0)}{(f\circ\gamma_1)'(0)}=\frac{\gamma_2'(0)}{\gamma_1'(0)}.
$$

Taking the [complex argument](../../../../../argument-complex-analysis.md) of this ratio shows that the oriented angle is preserved, while nonvanishing ensures both image tangents remain regular. Thus

$$
\boxed{f\text{ holomorphic and }f'\ne0\text{ on }U\ \Longrightarrow\ f\text{ conformal on }U}.
$$

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [a](../../a.md)
3. [6](../../../6.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
