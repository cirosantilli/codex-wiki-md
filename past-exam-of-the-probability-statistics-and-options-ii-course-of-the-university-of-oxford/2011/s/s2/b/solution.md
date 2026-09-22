<h1 id="s/s2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the independent standard normals stipulated in this part, simulate $n$ values and average the exceedance indicators:

$$
\boxed{\widehat z_0=\frac1n\sum_{k=1}^n\mathbf1_{\{X_k>c\}}.}
$$

Each indicator is Bernoulli with [probability](../../../../../probability.md) $z_c$, so [expectation](../../../../../expected-value-split.md) and independence give

$$
\boxed{\mathbb E\widehat z_0=z_c,\qquad v_0=\operatorname{Var}(\widehat z_0)=\frac{z_c(1-z_c)}n.}
$$

Thus the Monte Carlo estimator is unbiased.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [S2](../../s2.md)
3. [S](../../../s.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
