<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Covariance-based [PCA](../../../../../../../principal-component-analysis.md) uses centered protein measurements in their original gram units. Its total [variance](../../../../../../../variance-split.md) is $218.4$. Correlation-based [PCA](../../../../../../../principal-component-analysis.md) first divides each centered food measurement by its sample [standard deviation](../../../../../../../standard-deviation.md), giving nine unit-variance variables and total [variance](../../../../../../../variance-split.md) nine. Thus it is [principal component analysis on a correlation matrix](../../../../../../../principal-component-analysis-on-a-correlation-matrix.md), not an equivalent rotation of the original unscaled measurements.

The [variances](../../../../../../../variance-split.md) of cereals and milk together account for $170.9/218.4\approx78.3\%$ of the original total. Consequently those variables have considerable influence on covariance-based [PCA](../../../../../../../principal-component-analysis.md). Its first component is dominated by a cereal coefficient $-0.86$ opposed to milk $0.42$, broadly a cereal-versus-milk contrast. Its second is dominated by milk $0.83$, with cereals $0.40$ and fish $-0.29$. Its third is chiefly white meat $0.80$ versus fish $-0.52$, with a smaller negative milk term. Component signs may all be reversed without changing the analysis; the important features are relative signs and magnitudes.

After standardization, eggs and starch can contribute as strongly as large-variance foods. The first correlation-based component gives positive weight to meat, eggs, milk and starch, opposed principally to cereals and pulses/nuts; eggs now has coefficient $0.43$ despite its small raw [variance](../../../../../../../variance-split.md). The second emphasizes fish and fruit/vegetables negatively, opposed especially to starch and white meat. The third contrasts white meat and fruit/vegetables with milk, fish and red meat. Thus standardization changes both the emphasis and the directions, rather than just the displayed units of the same components.

The [explained variance of a principal component](../../../../../../../explained-variance-of-a-principal-component.md) must use the appropriate total:

$$
\begin{array}{c|ccc|c}
\text{analysis}&\text{PC1}&\text{PC2}&\text{PC3}&\text{first three}\\\hline
\text{covariance}&71.1\%&14.1\%&7.1\%&92.3\%\\
\text{correlation}&44.6\%&18.2\%&12.6\%&75.3\%.
\end{array}
$$

Raw and standardized percentages describe different [variance](../../../../../../../variance-split.md) objectives and must not be compared as if one method were always superior.

**Standardize when relative patterns across variables, rather than their absolute gram-scale variation, should have equal marginal weight.** Correlation-based [PCA](../../../../../../../principal-component-analysis.md) is also insensitive to changing a variable's measurement unit, which covariance-based [PCA](../../../../../../../principal-component-analysis.md) is not. Here every food group already has the same units, so differing units do not force standardization. If large fluctuations in actual protein amounts are scientifically important, covariance-based [PCA](../../../../../../../principal-component-analysis.md) is appropriate. If dietary composition across all food groups is the focus, correlation-based [PCA](../../../../../../../principal-component-analysis.md) can be more informative. Standardization can nevertheless amplify noise in nearly constant variables; the decision should follow the scientific purpose and measurement reliability.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
