<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Among the 12 pairs with control time first, the eight in which that first time is an event contribute $(1+\beta)^{-1}$ each. Among the eight pairs with treated time first, the four in which that first time is an event contribute $\beta/(1+\beta)$ each. Later events in one-eye risk sets contribute one. Hence

$$
L(\beta)\propto
\left(\frac1{1+\beta}\right)^8
\left(\frac\beta{1+\beta}\right)^4
=\frac{\beta^4}{(1+\beta)^{12}}.
$$

Differentiating the log likelihood gives $4/\beta-12/(1+\beta)=0$, and therefore

$$
\boxed{\widehat\beta=\frac12.}
$$

Without randomization, treatment side can be associated with prognosis. Always treating the left eye confounds treatment with systematic left-right differences; choosing the worse eye creates severe [confounding by indication](../../../../../../confounding-by-indication.md), baseline imbalance, and possible [regression toward the mean](../../../../../../regression-toward-the-mean.md). The within-patient comparison then no longer identifies a treatment effect without stronger adjustment assumptions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
