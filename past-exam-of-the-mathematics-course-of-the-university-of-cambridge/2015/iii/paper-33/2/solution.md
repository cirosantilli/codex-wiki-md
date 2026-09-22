<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $W_{aj\ell}$ be recall for age level $a$, processing level $j$, and replicate $\ell=1,\ldots,10$. Write $u_a=1$ for Younger and $0$ for Older. With Older and A as the [reference levels in a regression factor](../../../../../reference-level-in-a-regression-factor.md), the additive [two-factor normal linear model](../../../../../two-factor-normal-linear-model.md) under [treatment coding](../../../../../treatment-coding.md) is

$$
W_{aj\ell}=\mu+\alpha u_a+\gamma_j+\varepsilon_{aj\ell},\qquad\gamma_A=0,
$$

where the errors are independent $N(0,\sigma^2)$, with common positive variance. The [design matrix](../../../../../design-matrix.md) is fixed; subjects supply independent observations; the specified conditional mean is correct; and the absence of an [interaction term](../../../../../interaction-term.md) means the age difference is constant across processing levels. These are model assumptions, not consequences of random assignment. The treatment allocation supports independence between processing assignment and background characteristics, but age itself was not randomized.

An older subject in A has $u_a=0$ and $\gamma_A=0$, so the estimated mean is **$11.35$ words**. Its [standard error](../../../../../standard-error.md) is the intercept's $0.7632$. There are $100-6=94$ [residual degrees of freedom](../../../../../residual-degrees-of-freedom.md), giving the 95% [confidence interval](../../../../../confidence-interval.md) for this mean:

$$
\boxed{11.35\pm t_{94,0.975}\,0.7632\simeq(9.835,12.865).}
$$

This is a mean-response [confidence interval](../../../../../confidence-interval.md), not a prediction interval for a new individual's recall; the latter also includes the new observation's error variance.

The second [two-factor normal linear model](../../../../../two-factor-normal-linear-model.md) adds age-by-processing [interaction terms](../../../../../interaction-term.md):

$$
W_{aj\ell}=\mu+\alpha u_a+\gamma_j+\delta_ju_a+\varepsilon_{aj\ell},\qquad\gamma_A=\delta_A=0.
$$

Its ten free mean parameters are equivalent to one mean for each of the ten cells. To compare the fits, the [null hypothesis](../../../../../null-hypothesis.md) is $\delta_B=\delta_C=\delta_D=\delta_E=0$. The full [residual sum of squares](../../../../../residual-sum-of-squares.md) is $722.30$ on $90$ degrees of freedom. Adding interaction reduces the additive model's [residual sum of squares](../../../../../residual-sum-of-squares.md) by $190.30$, so the reduced value is $912.60$. The [nested-model F-test](../../../../../nested-model-f-test.md) statistic is

$$
\boxed{F=\frac{(912.60-722.30)/4}{722.30/90}=5.9279,\qquad F\sim F_{4,90}\text{ under }H_0.}
$$

Its [p-value](../../../../../p-value.md) is $0.0002793$. **Reject additivity and retain the interaction model.** The significant interaction means that a single age effect averaged over all processing methods does not adequately summarize the data.

The [regression intercept](../../../../../regression-intercept.md) $11.0$ is the older-A mean. The age coefficient $3.8$ is the younger-minus-older contrast specifically in A. The processing coefficients $(-4.0,2.4,1.0,-4.1)$ compare B, C, D and E with A specifically among older subjects. The interaction coefficients $(-4.3,0.4,3.5,-3.1)$ are differences between the age contrast in each of those methods and its value in A. Adding the relevant coefficients gives

$$
\begin{array}{c|rrrrr}
 &A&B&C&D&E\\\hline
\text{Older}&11.0&7.0&13.4&12.0&6.9\\
\text{Younger}&14.8&6.5&17.6&19.3&7.6\\
\text{Younger minus Older}&3.8&-0.5&4.2&7.3&0.7
\end{array}
$$

Thus A, C and especially D favour younger subjects in their estimated means, whereas B and E have little estimated age difference. In the younger group, D has the largest estimated recall, followed by C and A; B and E are much lower. Among older subjects C is largest, D and A are intermediate, and B and E are lowest. Comparing these orders is a description of estimates, not a claim that every pairwise difference is significant.

Each coefficient's printed [standard error](../../../../../standard-error.md) estimates its uncertainty; its $t$ statistic divides the estimate by that error, and its two-sided [p-value](../../../../../p-value.md) uses $t_{90}$ under the relevant zero-contrast [null hypothesis](../../../../../null-hypothesis.md). For example, the older B-versus-A and E-versus-A contrasts have $p=0.00217$ and $0.00170$. The C-versus-A and D-versus-A older contrasts have $p=0.06139$ and $0.43201$. The B interaction has $p=0.01846$, while the D interaction is borderline at $0.05387$ and the other two individual interaction tests are not significant at $5\%$. These individual tests do not override the joint interaction [F-test](../../../../../f-test.md), and multiple comparisons require care. A simple younger-versus-older contrast outside A combines coefficients and must use their estimated [covariance](../../../../../covariance.md), rather than adding their marginal errors.

The residual standard error $2.833$ estimates $\sigma$. The [coefficient of determination](../../../../../coefficient-of-determination.md) $0.7293$ is the fraction of centered sample recall variation explained by the ten-cell model. The overall $F=26.93$ with null law $F_{9,90}$ tests all nine non-intercept coefficients jointly against zero, giving extremely strong evidence that the cell means are not all equal. The sequential [analysis of variance](../../../../../analysis-of-variance.md) separates age, process, and their interaction; the balanced design makes the main-effect sums orthogonal, whereas the coefficient table uses the specified reference-level contrasts.

To assess pooling into three processing types, retain age-by-type interaction because the previous test rejects additivity. The reduced model $W\sim\mathrm{Age}*\mathrm{Type}$ has six cell means. Its [null hypothesis](../../../../../null-hypothesis.md) says A and C have equal means within each age, and B and E have equal means within each age: four restrictions. Compare it with the ten-cell model using

$$
F_{\mathrm{pool}}=\frac{(\operatorname{RSS}_{\mathrm{pool}}-722.30)/4}{722.30/90},\qquad F_{\mathrm{pool}}\sim F_{4,90}.
$$

In fact the supplied fitted cell means and equal cell sizes determine the increase without raw observations. Pooling two ten-person cells with means $m_1,m_2$ adds $5(m_1-m_2)^2$ to the [residual sum of squares](../../../../../residual-sum-of-squares.md). Here the four differences are $2.4,2.8,-0.1,1.1$, so

$$
\operatorname{RSS}_{\mathrm{pool}}-722.30=5(2.4^2+2.8^2+0.1^2+1.1^2)=74.10.
$$

Therefore $F_{\mathrm{pool}}=2.3083$ and $p\simeq0.0640$. **At $5\%$, the data do not reject the three-type reduction**, though the result is borderline and is not proof that the pooled means are identical. This [factor-level pooling test](../../../../../factor-level-pooling-test.md) keeps the previously supported interaction structure; reducing the categories and removing all interaction simultaneously would test a different set of restrictions.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
