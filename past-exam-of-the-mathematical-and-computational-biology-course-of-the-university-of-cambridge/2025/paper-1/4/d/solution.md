<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Yes. The [bootstrap confidence interval](../../../../../bootstrap-confidence-interval.md) for the age coefficient, $(0.057060,0.193584)$, excludes zero and supports the same positive association. A well-implemented [parametric bootstrap](../../../../../parametric-bootstrap.md) can give better finite-sample calibration than the asymptotic [likelihood-ratio test](../../../../../likelihood-ratio-test.md), especially with only eleven year groups and estimated [variance components](../../../../../variance-component.md). Its advantage depends on simulating the full fitted [Gaussian linear mixed model](../../../../../gaussian-linear-mixed-model.md) and refitting correctly; resampling individual records as if they were independent would discard the grouping. A [bootstrap confidence interval](../../../../../bootstrap-confidence-interval.md) is also not literally the same procedure as a bootstrap-calibrated test.

The bird-level [standard deviation](../../../../../standard-deviation.md) is appreciable, with interval $(0.436,0.720)$ hatchlings, whereas the year-level estimate is much less precise, with interval $(0.0195,0.333)$. The residual [standard deviation](../../../../../standard-deviation.md) is approximately $0.381$–$0.493$. Boundary fits in 23 of the 1000 replicates indicate that at least one fitted [variance component](../../../../../variance-component.md) sometimes reaches zero; the convergence warning should also be investigated before trusting the reported intervals. Neither the asymptotic test nor a model-based [bootstrap](../../../../../bootstrapping-statistics.md) repairs incorrect response-distribution or mean-structure assumptions.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
