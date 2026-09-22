<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

In the [log-linear transition intensity model](../../../../../../log-linear-transition-intensity-model.md), each [hazard ratio](../../../../../../hazard-ratio.md) multiplies a specific off-diagonal [transition intensity](../../../../../../transition-intensity.md), comparing its post-transplant period with the pre-transplant period while holding the modeled origin state fixed. Diagonal entries must then be recalculated from row sums.

For mild-to-severe progression, the early [hazard ratio](../../../../../../hazard-ratio.md) $0.52$ suggests a 48% decrease, but its interval $(0.11,2.4)$ includes no effect. The later [hazard ratio](../../../../../../hazard-ratio.md) $0.02$, with interval wholly below one, suggests a 98% decrease. These findings are compatible with suppression of progression by [hematopoietic stem cell transplantation](../../../../../../hematopoietic-stem-cell-transplantation.md) among those remaining in the mild state.

For mild-to-death, the early [hazard ratio](../../../../../../hazard-ratio.md) $43.92$ indicates a very large relative increase, and the later ratio $3.54$ still indicates an increase; both intervals are above one. For severe-to-death, the early ratio $2.37$ indicates increased mortality, whereas the later ratio $0.57$ indicates a 43% decrease; these intervals also exclude one. Early treatment toxicity and infection are plausible explanations for an immediate mortality increase. Later control of the underlying [myelodysplastic syndrome](../../../../../../myelodysplastic-syndrome.md) is a plausible explanation for reduced advanced-state mortality and progression.

Relative increases must be interpreted alongside baseline rates. The early mild-state death rate is approximately $0.0016\times43.92=0.0703$ per month, whereas the early severe-state death rate is $0.0380\times2.37=0.0901$ per month. Thus the far larger mild-state [hazard ratio](../../../../../../hazard-ratio.md) partly reflects its much smaller starting mortality, rather than greater absolute mortality after transplantation. The later corresponding rates are $0.00566$ and $0.02166$ per month.

Within the question's model, **delaying transplantation while the disease is mild can avoid a large immediate mortality cost, whereas the high baseline mortality in the severe state makes the later survival benefit more valuable.** This provides a qualitative rationale for the stated policy. The estimates do not establish an optimal timing rule: treatment selection, changing health status, selection of survivors into the later period and the use of the previous visit's covariate value can affect the comparison. They are associations from the fitted cohort model, not automatically causal [hazard ratios](../../../../../../hazard-ratio.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
