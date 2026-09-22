<h1 id="o/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For the continuous distribution in the question, $F$ maps the support monotonically from zero to one. For $0<t<1$, strict monotonicity gives

$$
\mathbb P(F(X)\leq t)=\mathbb P(X\leq F^{-1}(t))=t.
$$

Thus **$F(X)$ is uniform on $(0,1)$**, the [probability integral transform](../../../../probability-integral-transform.md).

The [order statistics](../../../../order-statistic.md) are the sample values sorted increasingly, $X_{(1)}\leq\cdots\leq X_{(n)}$. Monotonicity of $F$ makes $F(X_{(i)})$ the $i$th [order statistic](../../../../order-statistic.md) of independent uniforms. Its density is $n!t^{i-1}(1-t)^{n-i}/[(i-1)!(n-i)!]$, giving

$$
\boxed{\mathbb E F(X_{(i)})=\frac{i}{n+1},\qquad i=1,\ldots,n.}
$$

This follows either by beta integrals or by the equal expected lengths of the $n+1$ uniform spacings.

For the stated log-logistic cumulative distribution,

$$
\log\frac{F(x)}{1-F(x)}=(\beta-1)\log x-(\beta-1)\log\alpha.
$$

Therefore plot $\log[p_i/(1-p_i)]$ vertically against $\log X_{(i)}$ horizontally, with plotting positions $p_i=i/(n+1)$. A plausible model gives an approximately straight line, with **slope $\beta-1$ and intercept $-(\beta-1)\log\alpha$**. This specifies the axes explicitly, since reversing them would invert the slope.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [O](../../o.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
