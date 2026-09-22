<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix any [estimator](../../../../../../estimator.md) $\widehat\eta$ and put $A(x)=d(\widehat\eta(x),f)$, $B(x)=d(\widehat\eta(x),g)$ and $D=d(f,g)$. The [triangle inequality](../../../../../../triangle-inequality.md) for the [metric](../../../../../../metric.md) gives $A+B\geq D$. Hence

$$
A^2+B^2\geq\frac{(A+B)^2}{2}\geq\frac{D^2}{2}.
$$

The larger of the two [risk functions](../../../../../../risk-function.md) dominates their average. Using nonnegativity to replace both [probability density functions](../../../../../../probability-density-function.md) by their minimum,

$$
\begin{aligned}
\sup_{\eta\in\mathcal F}P_\eta d(\widehat\eta,\eta)^2
&\geq\frac12\{P_fA^2+P_gB^2\}\\
&\geq\frac12\int\min(p_f,p_g)(A^2+B^2)\,d\mu\\
&\geq\frac{D^2}{4}\int\min(p_f,p_g)\,d\mu.
\end{aligned}
$$

The right side is independent of the [estimator](../../../../../../estimator.md), so taking the infimum proves

$$
\boxed{\inf_{\widehat\eta}\sup_{\eta\in\mathcal F}P_\eta d(\widehat\eta,\eta)^2\geq\frac{d(f,g)^2}{4}\int\min(p_f,p_g)\,d\mu.}
$$

This [metric squared-loss two-point bound](../../../../../../metric-squared-loss-two-point-bound.md) uses overlap of the observation laws to quantify how hard it is to distinguish the two separated parameters.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
