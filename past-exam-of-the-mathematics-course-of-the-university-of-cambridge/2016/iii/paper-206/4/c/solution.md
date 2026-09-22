<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

This is a sequential [analysis of deviance for nested generalized linear models](../../../../../../analysis-of-deviance-for-nested-generalized-linear-models.md). Adding age to the intercept-only [logistic regression](../../../../../../logistic-regression.md) reduces deviance by $6.5187$, with approximate $\chi^2_1$ [p-value](../../../../../../p-value.md) $0.01067$. Adding frailty to the age model reduces it by another $16.6474$, with [p-value](../../../../../../p-value.md) $4.501\times10^{-5}$. Thus **both variables have evidence of association with surgical success**, under the model assumptions, and neither should be dropped solely on these results.

The second test assesses frailty adjusted for age, whereas the first assesses age before frailty is included. Sequential tests depend on term order. Evidence for age adjusted for frailty is additionally provided by its full-model [Wald test](../../../../../../wald-test.md), $p=0.01390$. Both fitted coefficients are negative: age and frailty are associated with lower fitted success probabilities. On the odds scale, one extra year at fixed frailty multiplies the odds by $e^{-0.08942}\approx0.9145$, and frailty at fixed age multiplies them by $e^{-3.15336}\approx0.04271$. These are [odds ratios](../../../../../../odds-ratio.md), not [risk ratios](../../../../../../risk-ratio.md), and an observational [statistical association](../../../../../../statistical-association.md) does not by itself establish a [causal effect](../../../../../../causal-effect.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 206](../../../paper-206-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
