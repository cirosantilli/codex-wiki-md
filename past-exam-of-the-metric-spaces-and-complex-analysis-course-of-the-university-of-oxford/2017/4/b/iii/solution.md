<h1 id="4/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Fix $0<r<1$ and $k\geq1$. On $|z|=1$ and $|z_0|<r$, the [reverse triangle inequality](../../../../../reverse-triangle-inequality.md) gives $|z-z_0|\geq1-r$. Subtract the two [Cauchy integral formula](../../../../../cauchy-integral-formula.md) expressions and apply the [estimation lemma](../../../../../estimation-lemma.md), using circle length $2\pi$:

$$
\sup_{|z_0|<r}|f_n^{(k)}(z_0)-f^{(k)}(z_0)|\leq\frac{k!}{(1-r)^{k+1}}\sup_{|z|=1}|f_n(z)-f(z)|\longrightarrow0.
$$

Thus **every fixed-order derivative converges uniformly on each smaller disc**. The right-hand factor tends to zero by the assumed uniform convergence on $D$. Keeping a positive gap $1-r$ from the integration contour is the essential feature of this [Cauchy derivative convergence bound](../../../../../cauchy-derivative-convergence-bound.md). If $r\leq0$, the specified open disc is empty and the claim is vacuous.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
