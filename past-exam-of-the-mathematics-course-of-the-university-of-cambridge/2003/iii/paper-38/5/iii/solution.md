<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [population-averaged logistic regression](../../../../../../population-averaged-logistic-model-for-repeated-binary-outcomes.md) describes $P(Y_{ij}=1\mid z_i,x_i)$ after averaging over unmeasured individual heterogeneity. Its intercept is a marginal [log odds](../../../../../../log-odds.md) at reference baseline values and time zero, its treatment coefficient is a population conditional-on-baseline [log odds ratio](../../../../../../log-odds-ratio.md), and its time coefficient is the change in that marginal [log odds](../../../../../../log-odds.md) per month. Time zero is an extrapolation here because the recorded visits begin later; centring time at the first visit would give a more interpretable intercept.

In the [random-intercept logistic model](../../../../../../logistic-random-intercept-model-for-repeated-binary-outcomes.md), the intercept is instead the conditional [log odds](../../../../../../log-odds.md) for a subject with $B_i=0$. The treatment and time coefficients apply at fixed $B_i$; the subject's actual intercept is $\alpha_C+B_i$. Even with a treatment-independent [random intercept](../../../../../../random-intercept.md), the conditional and marginal coefficients generally differ through [noncollapsibility of the odds ratio](../../../../../../noncollapsibility-of-the-odds-ratio.md). Indeed, if $\eta=\alpha_C+\phi_Cz+\beta_C^Tx+\delta_Ct$, marginalization gives

$$
M(\eta)=\mathbb E_B[\operatorname{logit}^{-1}(\eta+B)],
$$

which is not generally a logistic curve with the same linear coefficients. To quantify [random-intercept attenuation of marginal logistic slopes](../../../../../../random-intercept-attenuation-of-marginal-logistic-slopes.md), let $p_B=\operatorname{logit}^{-1}(\eta+B)$. Then

$$
M'=\mathbb E[p_B(1-p_B)]=M(1-M)-\operatorname{Var}(p_B),\qquad \frac{d\operatorname{logit}M}{d\eta}=1-\frac{\operatorname{Var}(p_B)}{M(1-M)}.
$$

For a nondegenerate finite [random intercept](../../../../../../random-intercept.md) this derivative lies strictly between zero and one and usually varies with $\eta$. Thus the marginal treatment contrast is an integrated, attenuated version of the conditional contrast, and the marginal time slope need not be constant. One should not equate the two sets of coefficients, even in a [randomized controlled trial](../../../../../../randomized-controlled-trial.md) without treatment confounding.

For [missing completely at random](../../../../../../missing-completely-at-random.md), an unweighted observed-response [GEE](../../../../../../generalized-estimating-equation.md) with cluster-robust [standard errors](../../../../../../standard-error.md) can consistently fit the marginal mean, and a correctly specified integrated [GLMM](../../../../../../generalized-linear-mixed-model.md) likelihood is valid as well. Under [missing at random](../../../../../../missing-at-random.md) depending on previous observed outcomes, ordinary unweighted [GEE](../../../../../../generalized-estimating-equation.md) is generally biased because the remaining responses are selected by informative observed history. Correct [inverse-observation-weighted estimating equations for longitudinal dropout](../../../../../../inverse-observation-weighted-estimating-equations-for-longitudinal-dropout.md) recover the marginal target under the sequential MAR and positivity assumptions already stated. Covariate-only observation mechanisms are a simpler special case in which correctly conditioned unweighted mean equations can remain valid.

A correctly specified joint response [GLMM](../../../../../../generalized-linear-mixed-model.md), fitted by [observed-data likelihood](../../../../../../observed-data-likelihood.md), is valid under ignorable [missing at random](../../../../../../missing-at-random.md) with [distinct parameters](../../../../../../distinct-parameters.md), including dependence of missingness on observed response history. This is a likelihood property, not a claim that every mixed model automatically fixes missingness. Under [missing not at random](../../../../../../missing-not-at-random.md), neither ordinary [GEE](../../../../../../generalized-estimating-equation.md), MAR-based weights nor a response-only [GLMM](../../../../../../generalized-linear-mixed-model.md) is generally valid; the unseen-outcome dependence requires further modelling and sensitivity assumptions.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
