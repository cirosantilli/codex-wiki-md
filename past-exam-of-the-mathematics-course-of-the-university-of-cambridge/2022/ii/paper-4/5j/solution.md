<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

Writing $Y_i=\operatorname{medv}_i$, $L_i=\operatorname{lstat}_i$, and $A_i=\operatorname{age}_i$, the fitted [normal linear model](../../../../../normal-linear-model.md) is

$$
Y_i
=\beta_0+\beta_1L_i+\beta_2A_i+\beta_3L_iA_i+\varepsilon_i,
\qquad
\varepsilon_i\stackrel{\rm iid}{\sim}N(0,\sigma^2).
$$

The R formula `lstat * age` includes both main effects and their [interaction term](../../../../../interaction-term.md).

Three notable features are:

- The fitted model is highly significant overall: its $F$ statistic is $209.3$ on $(3,502)$ degrees of freedom with $p<2.2\times10^{-16}$. Its $R^2=0.5557$, however, means that about $44\%$ of the observed response variation remains unexplained, and the residual standard deviation is about $6.15$ house-value units.

- At fixed age, the fitted slope with respect to lstat is$$
  -1.3921+0.004156\,A.
  $$

  The large negative main coefficient is strongly significant. The positive interaction is significant at the $5\%$ level ($p=0.0252$), indicating that this negative association becomes slightly weaker for older housing tracts.

- The age main-effect estimate is essentially zero with $p=0.9711$, but it is the age effect specifically at $L=0$ and should not be interpreted separately from the significant interaction. The diagnostic plots also show curved residual structure, increasing spread, a heavy upper tail with observations 215, 372, and 373, and substantial influence from observation 215. These features cast doubt on linearity, constant variance, and Gaussian residual assumptions.

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
