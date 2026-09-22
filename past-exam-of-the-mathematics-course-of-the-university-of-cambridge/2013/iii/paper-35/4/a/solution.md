<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Both factors are assigned at orchard level. Therefore the [experimental units](../../../../../../experimental-unit.md) are the twelve orchards; the trees are [observational units](../../../../../../observational-unit.md) within them. The six combinations form a balanced [factorial design](../../../../../../factorial-design.md), replicated twice. The orchard [ANOVA stratum](../../../../../../anova-stratum.md) has $12-1=11$ [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md). Spray uses $2-1=1$, pruning uses $3-1=2$, and their [interaction term](../../../../../../interaction-term.md) uses $(2-1)(3-1)=2$, leaving six for error.

Dividing each treatment [sum of squares in ANOVA](../../../../../../sum-of-squares-in-anova.md) by its [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md) and using $1440/6=240$ as the denominator gives **all missing entries**:

| Orchard source | Degrees of freedom | Mean square | Variance ratio, one significant figure |
| --- | --- | --- | --- |
| Spray | 1 | 998 | 4 |
| Pruning | 2 | 560 | 2 |
| Spray by pruning | 2 | 202 | 0.8 |
| Residual | 6 | 240 | Not applicable |

The unrounded [F-test](../../../../../../f-test.md) statistics are $998/240=4.15833\ldots$, $560/240=2.33333\ldots$ and $202/240=0.841667\ldots$. The within-orchard tree [mean square in ANOVA](../../../../../../mean-square-in-anova.md), 180, is not the treatment error denominator: using it would confuse subsampling with independent [replication](../../../../../../replication-in-experimental-design.md). The tree [ANOVA stratum](../../../../../../anova-stratum.md) has $12(30-1)=348$ [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md); $1+11+348=360$ is the uncorrected total, and the corrected total is 359.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
