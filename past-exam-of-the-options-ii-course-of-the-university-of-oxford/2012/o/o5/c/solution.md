<h1 id="o/o5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [likelihood ratio](../../../../../likelihood-ratio.md) between the two normal means is

$$
\frac{L(\mu_1;x)}{L(\mu_0;x)}
=\exp\left((\mu_1-\mu_0)\sum_{i=1}^nx_i-\frac n2(\mu_1^2-\mu_0^2)\right).
$$

Since $\mu_1>\mu_0$, it is strictly increasing in $\overline x$. The Neyman–Pearson test therefore rejects for large sample means. Under the null, $\sqrt n(\overline X-\mu_0)\sim N(0,1)$, so choosing a right-tail [probability](../../../../../probability.md) $\alpha$ gives

$$
\boxed{c_\alpha=\mu_0+\frac{z_\alpha}{\sqrt n},\qquad C=\{x:\overline x\geq c_\alpha\}.}
$$

This has size exactly $\alpha$ because the [sampling distribution](../../../../../sampling-distribution.md) is [continuous](../../../../../continuous-function.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [O5](../../o5.md)
3. [O](../../../o.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
