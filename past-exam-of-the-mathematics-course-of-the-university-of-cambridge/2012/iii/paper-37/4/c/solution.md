<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A Poisson model assumes independent counts between rats conditional on time, a common mean at a given time, and conditional [variance](../../../../../../variance-split.md) equal to that mean. Comparable observation units and consistent counting are needed; unexplained rat-to-rat heterogeneity is excluded by this simple specification. The quadratic [Poisson regression](../../../../../../poisson-regression.md) is

$$
Y_i\overset{\rm independent}{\sim}\operatorname{Pois}(\mu_i),\qquad
\log\mu_i=\beta_0+\beta_1t_i+\beta_2t_i^2.
$$

The printed nested analysis of deviance tests $H_0:\beta_2=0$ against $H_1:\beta_2\ne0$. Its likelihood-ratio statistic is $G^2=3.8548$, approximately $\chi^2_1$ under the [null hypothesis](../../../../../../null-hypothesis.md) and regular Poisson asymptotics. The reported $p=0.0496$ gives **borderline rejection of the log-linear time effect at 5%**, conditional on the Poisson assumptions. This is curvature of the log mean, rather than an ordinary quadratic model for the count itself.

There are only three distinct time values, so the intercept, linear term, and quadratic term span every possible set of three log means. This is [Poisson mean saturation at three distinct times](../../../../../../poisson-mean-saturation-at-three-distinct-times.md): the quadratic fit is saturated for the time-group means, which are $14/7=2$, $17/8=2.125$, and $47/7\simeq6.7143$. A grouped deviance comparison against unrestricted time-group means has zero [statistical degrees of freedom](../../../../../../statistical-degrees-of-freedom.md): **the quadratic functional form cannot be tested at these three times**. The individual-observation deviance 24.515 still describes within-group departure from the [Poisson distribution](../../../../../../poisson-distribution.md), but small means and zeros make the naive $\chi^2_{19}$ goodness-of-fit calibration doubtful. Poisson variation itself can be checked using the replicates, preferably by a [parametric bootstrap](../../../../../../parametric-bootstrap.md); it is not rendered untestable by the saturated mean specification.

[Overdispersion](../../../../../../overdispersion.md) means conditional [variance](../../../../../../variance-split.md) exceeding the [variance](../../../../../../variance-split.md) assumed by the Poisson mean model. For example, rats may have different latent susceptibility, so if $Y\mid\Lambda\sim\operatorname{Pois}(\Lambda)$, the [law of total variance](../../../../../../law-of-total-variance.md) gives $\operatorname{Var}(Y)=\mathbb E\Lambda+\operatorname{Var}(\Lambda)>\mathbb E Y$. A quasi-Poisson model instead uses $\operatorname{Var}(Y_i)=\phi\mu_i$. The Pearson-residual dispersion estimate is $\widehat\phi=1.254068$, using $n-p=22-3=19$.

For the conventional [quasi-likelihood](../../../../../../quasi-likelihood.md) comparison with estimated dispersion, use

$$
\boxed{F=\frac{(D_{\rm reduced}-D_{\rm full})/1}{\widehat\phi}
=\frac{3.8548}{1.254068}\simeq3.0738
\ \overset{\rm approx}{\sim}\ F_{1,19}.}
$$

Its upper-tail probability is about 0.096, so the evidence for curvature no longer reaches 5%. The [F-distribution](../../../../../../f-distribution.md) is an approximate calibration, not an exact small-sample result for arbitrary overdispersed counts; [quasi-likelihood](../../../../../../quasi-likelihood.md) does not supply a full Poisson likelihood. With known dispersion one would instead compare $G^2/\phi$ approximately with $\chi^2_1$. The displayed dispersion code uses the undefined name `acf.glm2`; its fitted values must be those of `aom.glm2` for the stated calculation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
