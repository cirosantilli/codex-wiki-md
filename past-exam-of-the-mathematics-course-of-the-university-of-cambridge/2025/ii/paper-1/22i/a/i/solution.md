<h1 id="22i/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The dual $X^*$ is the [vector space](../../../../../../../vector-space-split.md) of bounded [linear maps](../../../../../../../linear-map.md) $f:X\to\mathbb F$, with norm

$$
\lVert f\rVert=\sup_{\lVert x\rVert\leq1}|f(x)|.
$$

If $(f_n)$ is Cauchy in this norm, then $(f_n(x))$ is Cauchy in the complete [scalar](../../../../../../../scalar.md) field for every $x$. Define $f(x)=\lim_nf_n(x)$. Pointwise passage to the [limit](../../../../../../../limit-of-a-function.md) preserves [linearity](../../../../../../../linearity.md). Given $\varepsilon>0$, choose $N$ such that $\lVert f_n-f_m\rVert<\varepsilon$ for $m,n\geq N$; sending $m\to\infty$ gives

$$
|f_n(x)-f(x)|\leq\varepsilon\lVert x\rVert.
$$

**Thus $f$ is bounded and $\lVert f_n-f\rVert\leq\varepsilon$. Hence $X^*$ is Banach, even if $X$ was only normed.**

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [22I](../../../22i.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
