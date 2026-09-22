<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For an [exponential dispersion family](../../../../../exponential-dispersion-model.md), differentiating the normalization integral with respect to $\theta$ gives an expected score of zero. The score is $(Y-b'(\theta))/\phi$, hence $E(Y)=b'(\theta)$. Differentiating again, the expected squared score is $b''(\theta)/\phi$; it is also $\operatorname{Var}(Y)/\phi^2$. Thus

$$
\boxed{\mu_i=b'(\theta_i),\qquad\operatorname{Var}(Y_i)=\phi b''(\theta_i).}
$$

The [canonical link function](../../../../../canonical-link-function.md) sets the [linear predictor](../../../../../linear-predictor.md) equal to the natural parameter: $g(\mu)=\theta=(b')^{-1}(\mu)$. The [variance function](../../../../../variance-function.md) is $V(\mu)=b''((b')^{-1}(\mu))$, so $\operatorname{Var}(Y_i)=\phi V(\mu_i)$; the [dispersion parameter](../../../../../dispersion-parameter.md) $\phi$ is separated from the mean-dependent factor.

The [saturated statistical model](../../../../../saturated-statistical-model.md) has a separate mean for each response and fits $\widetilde\mu_i=y_i$, with boundary parameters interpreted by limits. At the same fixed dispersion, its log [likelihood](../../../../../likelihood-function.md) and the fitted model's [log-likelihood](../../../../../log-likelihood.md) define the [scaled deviance](../../../../../scaled-deviance.md)

$$
D^*=2\{\ell(\widetilde\theta;\phi)-\ell(\widehat\theta;\phi)\}.
$$

The unscaled [deviance](../../../../../exponential-family-deviance.md) is

$$
D=\phi D^*=2\sum_i\{y_i(\widetilde\theta_i-\widehat\theta_i)-b(\widetilde\theta_i)+b(\widehat\theta_i)\}.
$$

Keeping dispersion fixed in this definition is essential; it is not a comparison with a separately estimated zero [variance](../../../../../variance-split.md) in a Gaussian saturated fit.

For the [normal distribution](../../../../../normal-distribution.md), expanding its density exponent gives

$$
-\frac{(y-\mu)^2}{2\sigma^2}-\frac12\log(2\pi\sigma^2)
=\frac{y\mu-\mu^2/2}{\sigma^2}-\frac{y^2}{2\sigma^2}-\frac12\log(2\pi\sigma^2).
$$

Consequently

$$
\boxed{\theta_i=\mu_i,\quad b(\theta)=\theta^2/2,\quad\phi=\sigma^2,\quad c(y,\phi)=-y^2/(2\phi)-\tfrac12\log(2\pi\phi).}
$$

Here $V(\mu)=1$ and the canonical link is the identity, so $\mu_i=\beta^Tx_i$. The saturated natural parameter is $\widetilde\theta_i=y_i$. Substitution into the [deviance](../../../../../exponential-family-deviance.md) formula yields

$$
D=\sum_i(y_i-\widehat\mu_i)^2,\qquad
\boxed{D=\operatorname{RSS},\qquad D^*=\operatorname{RSS}/\sigma^2.}
$$

For the cholesterol fits, all formulae include an intercept. Model 1 has age and BMI with three coefficients; models 2 and 3 have one of these [covariates](../../../../../covariate.md) with two coefficients; model 4 has only the intercept. Their residual [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md) are respectively $27,28,28,29$. Their reported deviances are [residual sums of squares](../../../../../residual-sum-of-squares.md), because these are Gaussian linear models.

The relevant hypothesis is $H_0:\beta_{\mathrm{BMI}}=0$ in the full model, against $H_1:\beta_{\mathrm{BMI}}\ne0$, with age already present. Thus compare model 2 with model 1 using the [partial F-test](../../../../../partial-f-test-for-nested-linear-models.md). Its extra sum of squares is $31.64-27.10=4.54$, and the common [variance](../../../../../variance-split.md) is estimated from model 1 by $\widehat\sigma^2=27.10/27$. Therefore

$$
F=\frac{31.64-27.10}{27.10/27}=4.52325\sim F_{1,27}\quad\text{under }H_0.
$$

Since $4.52325>4.210$, reject at $5\%$; the two-sided coefficient-test equivalent has $p\simeq0.0427$. **BMI is associated with cholesterol after adjustment for age**, under the linear Gaussian model. The [RSS](../../../../../residual-sum-of-squares.md) values alone do not identify the sign of its coefficient or the size of the association.

For comparison, the marginal BMI test would compare model 4 with model 3, giving $F=13.88/(35.82/28)=10.8498$ on $(1,28)$ [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md), with $p\simeq0.00268$. This does not answer the adjusted question and makes the BMI evidence appear stronger than the conditional test. Age also contributes after BMI: comparing model 3 with model 1 gives $F=8.72/(27.10/27)=8.6878$ on $(1,27)$ [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md), with $p\simeq0.00653$. Thus retaining both predictors is supported at the stated level.

A raw [deviance](../../../../../exponential-family-deviance.md) difference must not simply be compared with the supplied $\chi_1^2$ cutoff: Gaussian dispersion is unknown and the differences here are unscaled. If $\sigma^2$ were known, the scaled difference $4.54/\sigma^2$ would have a $\chi_1^2$ law. Estimating it from the full fit gives the exact finite-sample $F$ comparison above, with the appropriate denominator [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
