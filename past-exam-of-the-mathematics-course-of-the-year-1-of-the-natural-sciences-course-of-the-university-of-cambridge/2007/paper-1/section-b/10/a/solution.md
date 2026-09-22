<h1 id="section-b/10/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $x>0$ write $f(x)=x^{-a}I(x)$, where $I(x)=\int_0^xe^{-t}t^{a-1}\,dt$. Because $a>0$, the lower endpoint is [integrable](../../../../../../integrability.md). At each positive upper endpoint the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) gives $I'(x)=e^{-x}x^{a-1}$. The [product rule](../../../../../../product-rule.md) therefore yields

$$
\boxed{f'(x)=\frac{e^{-x}}x-\frac{a}{x}f(x).}
$$

Differentiating once more and substituting this expression for $f'$ gives

$$
\boxed{f''(x)=-\frac{e^{-x}}x-\frac{(a+1)e^{-x}}{x^2}+\frac{a(a+1)}{x^2}f(x).}
$$

Substitution now cancels the $e^{-x}$ terms and the terms proportional to $f$, proving $xf''+(1+a+x)f'+af=0$.

The [change of variables](../../../../../../change-of-variables-formula.md) $t=xu$ identifies $f$ as the [scaled lower incomplete gamma integral](../../../../../../scaled-lower-incomplete-gamma-integral.md) $\int_0^1e^{-xu}u^{a-1}du$. It has a smooth extension at zero, with $f(0)=1/a$, $f'(0)=-1/(a+1)$ and $f''(0)=1/(a+2)$. Thus the apparent singularities in the derivative formulas cancel there; those formulas with denominators $x$ were derived for $x>0$.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [10](../../10.md)
3. [Section B](../../../section-b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
