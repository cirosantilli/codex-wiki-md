<h1 id="28j/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The assumed [maximum-likelihood estimator](../../../../../../../maximum-likelihood-estimator.md) is the sample mean of $h(X_i)$. Its [central limit theorem](../../../../../../../central-limit-theorem.md) is

$$
\sqrt n(\widehat\theta_{\mathrm{MLE}}-\theta_0)
\xrightarrow d N\left(0,\operatorname{Var}_{\theta_0}(h(X))\right).
$$

For a regular model, the regular maximum-likelihood limit is

$$
\sqrt n(\widehat\theta_{\mathrm{MLE}}-\theta_0)
\xrightarrow d N(0,I(\theta_0)^{-1}).
$$

The two asymptotic variances must agree, so

$$
\boxed{I(\theta_0)=\frac1{\operatorname{Var}_{\theta_0}(h(X))}.}
$$

Consequently

$$
\operatorname{Var}(\widehat\theta_{\mathrm{MLE}})
=\frac{\operatorname{Var}(h(X))}{n}
=\frac1{nI(\theta_0)}
$$

to first asymptotic order. The estimator therefore attains the [Cramér-Rao bound](../../../../../../../cramer-rao-bound.md) asymptotically: its precision, the reciprocal variance, exhausts the information in the sample.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [28J](../../../28j.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
