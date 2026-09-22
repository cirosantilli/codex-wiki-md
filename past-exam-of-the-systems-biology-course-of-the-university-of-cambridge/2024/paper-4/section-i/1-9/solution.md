<h1 id="section-i/1-9/solution">Solution</h1>

↑ **Parent:** [1.9](../1-9.md)

The two quantities are

$$
\boxed{\mathrm{precision}=\frac{TP}{TP+FP},\qquad\mathrm{recall}=\frac{TP}{TP+FN}.}
$$

[Classification precision](../../../../../precision-classification.md) asks how many retained calls agree with the positive reference; [classification recall](../../../../../recall-classification.md) asks how much of the positive reference set has been recovered. Recall is the [true positive rate](../../../../../recall-classification.md). Increasing recall by accepting more loci can reduce precision through additional false positives.

If positive prevalence is $p$, then

$$
\mathrm{precision}=\frac{p\,\operatorname{TPR}}{p\,\operatorname{TPR}+(1-p)\operatorname{FPR}}.
$$

Thus prevalence matters: good ROC discrimination need not give high precision when true positives are rare. A precision–recall area must be judged against its own prevalence-dependent baseline; it is not numerically interchangeable with ROC area.

## ↑ Ancestors (13)

1. [1.9](../1-9.md)
2. [Section I](../../section-i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [2024](../../../split.md)
5. [Past exam of the systems biology course of the University of Cambridge](../../../../split.md)
6. [Systems Biology course of the University of Cambridge](../../../../../systems-biology-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
