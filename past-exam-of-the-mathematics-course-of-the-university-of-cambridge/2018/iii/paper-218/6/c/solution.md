<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The command performs a [nested-model F-test](../../../../../../nested-model-f-test.md) for $H_0:\beta_1=0$ against $H_1:\beta_1\ne0$, retaining the intercept and $x_2$ coefficient in both models. Write $RSS_2$ and $RSS_3$ for the [residual sum of squares](../../../../../../residual-sum-of-squares.md) in the reduced and full fits. Under $H_0$ and the independent normal-error assumptions,

$$
\boxed{F=\frac{(RSS_2-RSS_3)/1}{RSS_3/(n-3)}\sim F_{1,n-3},\qquad p=\Pr(F_{1,n-3}\geq F_{obs}).}
$$

By [Cochran's theorem](../../../../../../cochran-s-theorem.md), the numerator and denominator are independent scaled chi-squares with one and $n-3$ degrees of freedom. Equivalently, for this single-coefficient restriction, $F=t_{\beta_1}^2$, so its p-value equals that of the two-sided coefficient [Student's t-test](../../../../../../student-s-t-test.md) in model3.

Using the printed $t$ value gives $F=0.800^2=0.640$ and $p\approx0.43$. The printed estimate and standard error instead give

$$
\boxed{F=(1.8663/2.3538)^2\approx0.62867,\qquad p\approx0.43.}
$$

This discrepancy is present in the PDF and is too large to be explained by rounding at the shown precision; the underlying ANOVA output is omitted, so an exact unique statistic cannot be recovered. The univariate correlation and $t$ value imply $n\approx2+2.575^2(1-0.2517297^2)/0.2517297^2\approx100.006$, consistent with $n=100$ after rounding. With denominator degrees of freedom 97, the two versions give p-values approximately $0.4257$ and $0.4298$, respectively. Either way the partial effect is not significant at 5%.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
