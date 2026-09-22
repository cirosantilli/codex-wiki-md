<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A second opportunity to reject raises the trial's overall [Type I error](../../../../../../type-i-and-type-ii-errors.md) above the nominal 10% in general. If $A$ and $B$ denote rejection at the first and second analyses, the overall error is

$$
\mathbb P_0(A)+\mathbb P_0(A^c\cap B).
$$

The cumulative-data [test statistics](../../../../../../test-statistic.md) are correlated, so neither 20% nor $1-0.9^2=19\%$ is the general answer. The latter requires independent tests, which is not the situation here.

**The rejection thresholds and the stopping/continuation rule must be calibrated jointly.** A prespecified [group sequential design](../../../../../../group-sequential-design.md) or [alpha-spending function](../../../../../../alpha-spending-function.md) can allocate a total error budget of 10% across the analyses, using their joint null distribution. A conservative alternative planned in advance is two tests each at 5%, controlled by the [Bonferroni inequality](../../../../../../bonferroni-inequalities.md). An unplanned change to a design with a remaining error budget can be justified by the [conditional error principle](../../../../../../conditional-error-principle.md). Here, however, an original single-look test at 10% has no remaining conditional rejection probability after its final nonrejection. Keeping its entire original rejection region and adding a new positive-probability rejection opportunity cannot in general retain a 10% overall error rate. The two-look rule therefore needs prospective joint calibration; an already observed result cannot retrospectively create an unused error budget.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
