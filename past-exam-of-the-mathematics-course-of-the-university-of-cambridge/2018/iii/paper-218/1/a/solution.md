<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The violated assumption is [independence of random variables](../../../../../../independent-random-variables.md) across observations: repeated measurements on the same rat form [clustered data](../../../../../../clustered-data.md). A persistent rat-specific weight difference induces positive within-rat [covariance](../../../../../../covariance.md), even after adjustment for time and diet. Treating all 176 measurements as independent is [pseudoreplication](../../../../../../pseudoreplication.md).

For the claimed lack of [identifiability](../../../../../../identifiability.md) in the second fit, Rat must be a [categorical variable](../../../../../../categorical-variable.md), as intended by the rat-effect interpretation. Each rat receives only one diet, so this is [confounding of nested fixed factors](../../../../../../confounding-of-nested-fixed-factors.md). If $z_r$ is the rat-indicator column, the diet-$d$ indicator is $\sum_{r:\,D_r=d}z_r$. Thus a diet effect can be increased by $c_d$ and every corresponding rat effect decreased by $c_d$, leaving all [fitted values](../../../../../../fitted-values.md) unchanged. With an intercept, two diet columns, fifteen rat contrasts and time, there are 19 columns but only 17 independent columns: the intercept and rat contrasts already span the diet columns, while time varies within rats. This gives [rank-deficient ordinary least squares](../../../../../../rank-deficient-ordinary-least-squares.md).

**The first model ignores within-rat dependence; the second cannot separate unrestricted fixed diet and rat effects.** If Rat were instead encoded as a single numeric predictor, the asserted rank deficiency would not follow merely from nesting.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
