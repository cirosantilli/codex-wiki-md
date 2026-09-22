<h1 id="4/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The reported [deviance information criterion](../../../../../../deviance-information-criterion.md) differs by

$$
\boxed{\operatorname{DIC}_2-\operatorname{DIC}_3=1.9.}
$$

Model 3 has a mean [Bayesian deviance](../../../../../../bayesian-deviance.md) worse by only $0.2$, but its [effective parameter count in DIC](../../../../../../effective-parameter-count-in-dic.md) is lower by $2.1$. The small fit cost is more than offset by the reduced complexity penalty, so the criterion gives a mild preference to Model 3. A difference this small should not be presented as decisive evidence, especially without the [Monte Carlo error](../../../../../../monte-carlo-error.md) of the criterion difference.

The counts $143.6$ and $141.5$ are effective rather than literal parameter numbers. The likelihood includes child-specific intercepts and uncertain true baselines as well as global coefficients. With 106 of each local quantity and seven global parameters, Model 2 has 219 stochastic unknowns in a natural full representation, but [partial pooling](../../../../../../partial-pooling.md) and other prior information reduce their effective contribution. Fixing two slopes lowers the effective count by about two, with a further small change from the fitted posterior. There is no reason for $p_D$ to be an integer, or to equal just the number of population-level regression coefficients.

For illustration, the deviances evaluated at posterior means implied by the table are $\overline D-p_D=984.5$ for Model 2 and $986.8$ for Model 3. These differ from the average deviances because averaging a nonlinear deviance is not the same as evaluating it at an averaged parameter. This interpretation presumes the same observed-data likelihood convention in both fits; integrating local variables out before forming the deviance would define a different comparison. The [DIC](../../../../../../deviance-information-criterion.md) difference is not a [Bayes factor](../../../../../../bayes-factor.md).

## ↑ Ancestors (11)

1. [G](../g.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
