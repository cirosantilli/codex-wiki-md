<h1 id="13l/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $X$ be the $173\times3$ design [matrix](../../../../../../matrix.md) and write $p=3$. The displayed estimate in row $j$ is

$$
\widehat\beta_j,\qquad
\widehat\beta=(X^TX)^{-1}X^TY.
$$

With

$$
s^2=\frac{\operatorname{RSS}}{n-p}
=\frac{\|Y-X\widehat\beta\|^2}{170},
$$

its standard error is

$$
\operatorname{se}(\widehat\beta_j)
=s\sqrt{[(X^TX)^{-1}]_{jj}}.
$$

The $t$-value and two-sided $p$-value are

$$
t_j=\frac{\widehat\beta_j}{\operatorname{se}(\widehat\beta_j)},
\qquad
2\mathbb P\{|T_{170}|\geq|t_j|\},
$$

respectively.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [13L](../../13l.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
