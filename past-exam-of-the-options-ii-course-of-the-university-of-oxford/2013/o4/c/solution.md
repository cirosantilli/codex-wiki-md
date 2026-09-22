<h1 id="o4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $S=\sum_i x_i^2$, the [likelihood ratio](../../../../likelihood-ratio.md) in favor of the larger [variance](../../../../variance-split.md) is

$$
\frac{f_{\sigma_1^2}(x)}{f_{\sigma_0^2}(x)}
=\left(\frac{\sigma_0}{\sigma_1}\right)^n
\exp\left[\frac S2\left(\frac1{\sigma_0^2}-\frac1{\sigma_1^2}\right)\right].
$$

Because $\sigma_1>\sigma_0$, this is strictly increasing in $S$. The [Neyman-Pearson lemma](../../../../neyman-pearson-lemma.md) therefore selects an upper-tail rejection region. Under the null, $S/\sigma_0^2\sim\chi_n^2$, so size $\alpha$ is obtained with

$$
\boxed{C=\{S\geq k_\alpha\},\qquad k_\alpha=\sigma_0^2F_n^{-1}(1-\alpha).}
$$

Continuity of the chi-squared distribution makes the boundary have [probability](../../../../probability.md) zero. This is a [fixed-mean normal variance test](../../../../fixed-mean-normal-variance-test.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [O4](../../o4.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
