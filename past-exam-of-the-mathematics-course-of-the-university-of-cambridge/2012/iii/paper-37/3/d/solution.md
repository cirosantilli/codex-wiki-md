<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In the species-only model, the [log odds](../../../../../../log-odds.md) for adult species A is the intercept, so **$\widehat\theta_A=0.91191$ with [standard error](../../../../../../standard-error.md) 0.07824**. This also follows directly by pooling its vials: there are 570 other-species eggs among 799 eggs eaten, giving $\widehat p_A=570/799$ and

$$
\widehat\theta_A=\log\frac{570}{229}\simeq0.91191.
$$

For a regular [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md), [asymptotic normality of a maximum likelihood estimator](../../../../../../asymptotic-normality-of-a-maximum-likelihood-estimator.md) gives $\widehat\theta_A\overset{\rm approx}{\sim}N(\theta_A,I_A^{-1})$, with information $I_A=N_Ap_A(1-p_A)$. Substitution of $\widehat p_A$ gives $\operatorname{se}(\widehat\theta_A)=\sqrt{1/570+1/229}\simeq0.07824$. An approximate 95% [Wald confidence interval](../../../../../../wald-confidence-interval.md) is

$$
\boxed{0.91191\pm1.96(0.07824)=(0.7586,1.0653).}
$$

This interval treats the selected species-only model as fixed; it does not account separately for uncertainty from choosing that model.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
