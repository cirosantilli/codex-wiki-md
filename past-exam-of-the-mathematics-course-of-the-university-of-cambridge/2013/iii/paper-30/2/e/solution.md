<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [analysis of variance](../../../../../../analysis-of-variance.md) provides evidence of a chocolate effect both with day included ($F_{3,18}=3.9665$, [p-value](../../../../../../p-value.md) $0.02473$) and with day omitted ($F_{3,20}=4.039$, [p-value](../../../../../../p-value.md) $0.02133$). Because every chocolate–day cell has the same replication, [balanced factorial orthogonality](../../../../../../balanced-factorial-orthogonality.md) separates the two main effects; the chocolate row is meaningful despite being entered first.

The chocolate-only fitted group means are approximately $14.17,11.67,9.33,11.33$ boards for A, B, C, D respectively. Thus **A has the largest fitted lecturing speed and C the smallest**. Relative to A, the fitted differences are $-2.50,-4.83,-2.83$ boards. The printed individual [Student t-tests](../../../../../../student-s-t-test.md) give strong evidence for the A–C contrast ([p-value](../../../../../../p-value.md) $0.00245$); B and D versus A have [p-values](../../../../../../p-value.md) $0.08835$ and $0.05582$, respectively. Those latter contrasts are not significant at 5%, and the output does not test all other pairwise comparisons. Simultaneous claims would require accounting for [multiple hypothesis testing](../../../../../../multiple-hypothesis-testing.md).

There is little evidence of a day effect after adjusting for chocolate. A chocolate-only [normal linear model](../../../../../../normal-linear-model.md) is therefore a reasonable simpler summary, with residual [standard deviation](../../../../../../standard-deviation.md) about $2.42$ boards and explained variation $R^2\simeq0.377$. This is an association under the additive [statistical model](../../../../../../statistical-model-split.md); a causal claim would additionally require an appropriate assignment of chocolate and checks of the [regression residuals](../../../../../../regression-residual.md) and possible [interaction terms](../../../../../../interaction-term.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
