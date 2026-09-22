<h1 id="2/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Under [Neyman allocation](../../../../../../neyman-allocation.md), sample sizes are proportional to the arm standard deviations. Here

$$
\frac{n_1}{n_0}
=\frac{\sqrt{p_1(1-p_1)}}{\sqrt{p_0(1-p_0)}}
=\frac{0.5}{0.3}=\frac53.
$$

For total size $n_{\max}$, the minimized [asymptotic variance](../../../../../../asymptotic-variance.md) is

$$
\operatorname{Var}(\widehat p_1-\widehat p_0)
=\frac{\bigl(\sqrt{0.25}+\sqrt{0.09}\bigr)^2}{n_{\max}}
=\frac{0.64}{n_{\max}}.
$$

Equal allocation gives

$$
\frac{0.25}{n_{\max}/2}+\frac{0.09}{n_{\max}/2}
=\frac{0.68}{n_{\max}}.
$$

The Neyman allocation therefore reduces the large-sample variance by $0.04/n_{\max}$, about $5.9\%$ of the equal-allocation variance.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [2](../../2.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
