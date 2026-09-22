<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $X$ have the [Pareto distribution](../../../../../pareto-distribution.md) with [probability density function](../../../../../probability-density-function.md) $f_X(x)=3x^{-4}$ for $x\geq1$, and zero otherwise. Its [normalization of a probability distribution](../../../../../normalization-of-a-probability-distribution.md) and first two [moments](../../../../../moment.md) follow from

$$
\int_1^\infty3x^{-4}\,dx=1,\qquad
\mathbb EX=3\int_1^\infty x^{-3}\,dx=\frac32,\qquad
\mathbb EX^2=3\int_1^\infty x^{-2}\,dx=3.
$$

Set $Y=X-3/2$. Then

$$
\boxed{\mathbb EY=0,\qquad\operatorname{Var}(Y)=3-\frac94=\frac34.}
$$

The [probability distribution](../../../../../probability-distribution-split.md) of $Y$ is not a [symmetric distribution](../../../../../symmetric-distribution.md): $Y\geq-1/2$ [almost surely](../../../../../almost-sure-convergence.md), whereas $\mathbb P(Y>1/2)=\mathbb P(X>2)=1/8>0$ and $\mathbb P(Y<-1/2)=0$. For $X\geq3$ we have $|Y|\geq X/2$, so

$$
\mathbb E|Y|^3\geq\frac18\mathbb E\bigl[X^3\mathbf1_{\{X\geq3\}}\bigr]
=\frac38\int_3^\infty\frac{dx}{x}=\infty.
$$

Thus $\boxed{Y=X-3/2}$ has every property required.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
