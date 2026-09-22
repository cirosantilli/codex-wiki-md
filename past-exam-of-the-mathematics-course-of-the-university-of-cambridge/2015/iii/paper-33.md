# Paper 33

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_33.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_33.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
- [5](#5)
  - [a](#5/a)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
    - [iii](#5/a/iii)
      - [Solution](#5/a/iii/solution)
  - [b](#5/b)
    - [i](#5/b/i)
      - [Solution](#5/b/i/solution)
    - [ii](#5/b/ii)
      - [Solution](#5/b/ii/solution)
    - [iii](#5/b/iii)
      - [Solution](#5/b/iii/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares) objective has [gradient](../../../calculus.md#gradient) $2X^TX\beta-2X^TY$. The [normal equation](../../../statistical-modelling.md#normal-equation) therefore gives

$$
\boxed{\widehat\beta=(X^TX)^{-1}X^TY.}
$$

The [Gram matrix](../../../linear-algebra.md#gram-matrix) $X^TX$ is a [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix) because $X$ has full column rank. More explicitly, for any $b$,

$$
R(b)=R(\widehat\beta)+(b-\widehat\beta)^TX^TX(b-\widehat\beta),
$$

since $X^T(Y-X\widehat\beta)=0$. This proves that the displayed solution is the unique global minimum.

The [fitted values](../../../linear-regression.md#fitted-values) are $\widehat Y=X\widehat\beta=HY$, where the [hat matrix](../../../statistical-modelling.md#hat-matrix) is

$$
H=X(X^TX)^{-1}X^T.
$$

The inverse of the symmetric matrix $X^TX$ is symmetric, so $H^T=H$. Multiplication gives $H^2=X(X^TX)^{-1}(X^TX)(X^TX)^{-1}X^T=H$. Thus $H$ is the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto the [column space](../../../vector-space.md#column-space) of the [design matrix](../../../linear-regression.md#design-matrix).

The [regression residual](../../../probability-and-statistics.md#regression-residual) vector is $e=Y-\widehat Y=GY$ with $G=I_n-H$. Consequently $G^T=G$, $G^2=I_n-2H+H^2=G$, and the [residual sum of squares](../../../linear-regression.md#residual-sum-of-squares) is

$$
\boxed{e^Te=Y^TG^TGY=Y^TGY.}
$$

By [fitted-residual orthogonality](../../../statistical-modelling.md#fitted-residual-orthogonality), $GH=0$. Using $\operatorname{Cov}(Y)=\sigma^2I_n$, the cross-[covariance matrix](../../../variance.md#covariance-matrix) is

$$
\boxed{\operatorname{Cov}(e,\widehat Y)=G\sigma^2I_nH^T=0.}
$$

Both vectors are jointly normal, so they are also independent by [independence of uncorrelated jointly normal variables](../../../probability-and-statistics.md#independence-of-uncorrelated-jointly-normal-variables). The zero covariance calculation itself only needs the common error variance and lack of error correlations.

For the first wind fit, let $v_i$ be wind velocity and $Y_i$ electrical output. The [simple linear regression](../../../linear-regression.md#simple-linear-regression) is $Y_i=\alpha+\beta v_i+\varepsilon_i$, with independent $\varepsilon_i\sim N(0,\sigma^2)$. It has two fitted mean parameters and $25-2=23$ [residual degrees of freedom](../../../statistical-modelling.md#residual-degrees-of-freedom). The missing [analysis of variance](../../../linear-regression.md#analysis-of-variance) entries are therefore **velocity degrees of freedom $1$, velocity mean square $8.9296$, and residual degrees of freedom $23$**. The residual mean square is $1.2816/23\simeq0.05572$, and $8.9296/(1.2816/23)\simeq160.25$, consistent with the printed value after rounding.

Because the model includes a [regression intercept](../../../linear-regression.md#regression-intercept), the [coefficient of determination](../../../linear-regression.md#coefficient-of-determination) is the explained sum of squares divided by the total centered sum of squares:

$$
R^2=\frac{8.9296}{8.9296+1.2816}=1-\frac{1.2816}{10.2112}\simeq\boxed{0.8745}.
$$

A large [coefficient of determination](../../../linear-regression.md#coefficient-of-determination) does not rule out a wrong mean function. In the PDF's first [residual-versus-fitted plot](../../../linear-regression.md#residual-versus-fitted-plot), residuals are negative at both ends and positive in the middle. This curved pattern agrees with the visibly flattening output-versus-velocity relationship and motivates a [polynomial regression](../../../linear-regression.md#polynomial-regression) with a quadratic term.

The second wind model is $Y_i=\alpha+\beta_1v_i+\beta_2v_i^2+\varepsilon_i$, again with independent common-variance normal errors. Its fitted mean is $-1.155898+0.722936v_i-0.038121v_i^2$. The line marked (A) is a two-sided [Student t-test](../../../statistical-modelling.md#student-s-t-test) of $H_0:\beta_2=0$ against $H_1:\beta_2\ne0$, conditional on retaining the intercept and linear term. Under the [null hypothesis](../../../statistical-modelling.md#null-hypothesis),

$$
t=\frac{-0.038121}{0.004797}\simeq-7.947\sim t_{22}.
$$

Its two-sided [p-value](../../../statistical-modelling.md#p-value) is $6.59\times10^{-8}$. This is far below $0.05$, so **reject a purely linear mean in favour of the quadratic fit**. Equivalently, the extra-term [nested-model F-test](../../../probability-and-statistics.md#nested-model-f-test) has $F=t^2\simeq63.15$ and null law $F_{1,22}$.

The third fit is a [reciprocal-predictor regression](../../../linear-regression.md#reciprocal-predictor-regression), $Y_i=a+b/v_i+\varepsilon_i$, with estimated mean $2.9789-6.9345/v_i$. It has two mean parameters rather than the quadratic model's three. Its residual standard error is smaller, $0.09417$ versus $0.1227$, and its [coefficient of determination](../../../linear-regression.md#coefficient-of-determination) is larger, $0.9800$ versus $0.9676$. The corresponding [residual sums of squares](../../../linear-regression.md#residual-sum-of-squares) are approximately $23(0.09417)^2=0.20396$ and $22(0.1227)^2=0.33122$. **The reciprocal fit is preferable on both these fit measures and parsimony.** The two models are not nested, so an ordinary extra-term [F-test](../../../probability-and-statistics.md#f-test) between them is inappropriate. On the common normal-error likelihood, the difference $\operatorname{AIC}_3-\operatorname{AIC}_2=25\log(0.20396/0.33122)-2\simeq-14.12$ also favours the third model.

Neither lower [residual sum of squares](../../../linear-regression.md#residual-sum-of-squares) nor a higher [coefficient of determination](../../../linear-regression.md#coefficient-of-determination) establishes adequate assumptions. The quadratic [residual-versus-fitted plot](../../../linear-regression.md#residual-versus-fitted-plot) removes the original pronounced curvature; the reciprocal plot also has no comparably obvious mean trend. The low-output residuals appear somewhat more spread out, so check [scale-location plots](../../../linear-regression.md#scale-location-plot) and residuals against velocity for [heteroscedasticity](../../../statistical-modelling.md#heteroscedastic). [Q-Q plots](../../../probability-and-statistics.md#q-q-plot) assess normality; residuals against observation order assess serial dependence; [regression leverage](../../../statistical-modelling.md#regression-leverage) and [Cook's distance](../../../statistical-modelling.md#cook-s-distance) identify influential observations. Further [cross-validation](../../../statistical-learning.md#cross-validation), replicate observations at comparable velocities, and prediction errors would help choose between their extrapolation behaviours. Both fitted shapes should be judged principally over the observed positive-velocity range.

## 2

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let $W_{aj\ell}$ be recall for age level $a$, processing level $j$, and replicate $\ell=1,\ldots,10$. Write $u_a=1$ for Younger and $0$ for Older. With Older and A as the [reference levels in a regression factor](../../../statistical-modelling.md#reference-level-in-a-regression-factor), the additive [two-factor normal linear model](../../../statistical-modelling.md#two-factor-normal-linear-model) under [treatment coding](../../../statistical-modelling.md#treatment-coding) is

$$
W_{aj\ell}=\mu+\alpha u_a+\gamma_j+\varepsilon_{aj\ell},\qquad\gamma_A=0,
$$

where the errors are independent $N(0,\sigma^2)$, with common positive variance. The [design matrix](../../../linear-regression.md#design-matrix) is fixed; subjects supply independent observations; the specified conditional mean is correct; and the absence of an [interaction term](../../../statistical-model.md#interaction-term) means the age difference is constant across processing levels. These are model assumptions, not consequences of random assignment. The treatment allocation supports independence between processing assignment and background characteristics, but age itself was not randomized.

An older subject in A has $u_a=0$ and $\gamma_A=0$, so the estimated mean is **$11.35$ words**. Its [standard error](../../../statistical-inference.md#standard-error) is the intercept's $0.7632$. There are $100-6=94$ [residual degrees of freedom](../../../statistical-modelling.md#residual-degrees-of-freedom), giving the 95% [confidence interval](../../../statistical-inference.md#confidence-interval) for this mean:

$$
\boxed{11.35\pm t_{94,0.975}\,0.7632\simeq(9.835,12.865).}
$$

This is a mean-response [confidence interval](../../../statistical-inference.md#confidence-interval), not a prediction interval for a new individual's recall; the latter also includes the new observation's error variance.

The second [two-factor normal linear model](../../../statistical-modelling.md#two-factor-normal-linear-model) adds age-by-processing [interaction terms](../../../statistical-model.md#interaction-term):

$$
W_{aj\ell}=\mu+\alpha u_a+\gamma_j+\delta_ju_a+\varepsilon_{aj\ell},\qquad\gamma_A=\delta_A=0.
$$

Its ten free mean parameters are equivalent to one mean for each of the ten cells. To compare the fits, the [null hypothesis](../../../statistical-modelling.md#null-hypothesis) is $\delta_B=\delta_C=\delta_D=\delta_E=0$. The full [residual sum of squares](../../../linear-regression.md#residual-sum-of-squares) is $722.30$ on $90$ degrees of freedom. Adding interaction reduces the additive model's [residual sum of squares](../../../linear-regression.md#residual-sum-of-squares) by $190.30$, so the reduced value is $912.60$. The [nested-model F-test](../../../probability-and-statistics.md#nested-model-f-test) statistic is

$$
\boxed{F=\frac{(912.60-722.30)/4}{722.30/90}=5.9279,\qquad F\sim F_{4,90}\text{ under }H_0.}
$$

Its [p-value](../../../statistical-modelling.md#p-value) is $0.0002793$. **Reject additivity and retain the interaction model.** The significant interaction means that a single age effect averaged over all processing methods does not adequately summarize the data.

The [regression intercept](../../../linear-regression.md#regression-intercept) $11.0$ is the older-A mean. The age coefficient $3.8$ is the younger-minus-older contrast specifically in A. The processing coefficients $(-4.0,2.4,1.0,-4.1)$ compare B, C, D and E with A specifically among older subjects. The interaction coefficients $(-4.3,0.4,3.5,-3.1)$ are differences between the age contrast in each of those methods and its value in A. Adding the relevant coefficients gives

$$
\begin{array}{c|rrrrr}
 &A&B&C&D&E\\\hline
\text{Older}&11.0&7.0&13.4&12.0&6.9\\
\text{Younger}&14.8&6.5&17.6&19.3&7.6\\
\text{Younger minus Older}&3.8&-0.5&4.2&7.3&0.7
\end{array}
$$

Thus A, C and especially D favour younger subjects in their estimated means, whereas B and E have little estimated age difference. In the younger group, D has the largest estimated recall, followed by C and A; B and E are much lower. Among older subjects C is largest, D and A are intermediate, and B and E are lowest. Comparing these orders is a description of estimates, not a claim that every pairwise difference is significant.

Each coefficient's printed [standard error](../../../statistical-inference.md#standard-error) estimates its uncertainty; its $t$ statistic divides the estimate by that error, and its two-sided [p-value](../../../statistical-modelling.md#p-value) uses $t_{90}$ under the relevant zero-contrast [null hypothesis](../../../statistical-modelling.md#null-hypothesis). For example, the older B-versus-A and E-versus-A contrasts have $p=0.00217$ and $0.00170$. The C-versus-A and D-versus-A older contrasts have $p=0.06139$ and $0.43201$. The B interaction has $p=0.01846$, while the D interaction is borderline at $0.05387$ and the other two individual interaction tests are not significant at $5\%$. These individual tests do not override the joint interaction [F-test](../../../probability-and-statistics.md#f-test), and multiple comparisons require care. A simple younger-versus-older contrast outside A combines coefficients and must use their estimated [covariance](../../../variance.md#covariance), rather than adding their marginal errors.

The residual standard error $2.833$ estimates $\sigma$. The [coefficient of determination](../../../linear-regression.md#coefficient-of-determination) $0.7293$ is the fraction of centered sample recall variation explained by the ten-cell model. The overall $F=26.93$ with null law $F_{9,90}$ tests all nine non-intercept coefficients jointly against zero, giving extremely strong evidence that the cell means are not all equal. The sequential [analysis of variance](../../../linear-regression.md#analysis-of-variance) separates age, process, and their interaction; the balanced design makes the main-effect sums orthogonal, whereas the coefficient table uses the specified reference-level contrasts.

To assess pooling into three processing types, retain age-by-type interaction because the previous test rejects additivity. The reduced model $W\sim\mathrm{Age}*\mathrm{Type}$ has six cell means. Its [null hypothesis](../../../statistical-modelling.md#null-hypothesis) says A and C have equal means within each age, and B and E have equal means within each age: four restrictions. Compare it with the ten-cell model using

$$
F_{\mathrm{pool}}=\frac{(\operatorname{RSS}_{\mathrm{pool}}-722.30)/4}{722.30/90},\qquad F_{\mathrm{pool}}\sim F_{4,90}.
$$

In fact the supplied fitted cell means and equal cell sizes determine the increase without raw observations. Pooling two ten-person cells with means $m_1,m_2$ adds $5(m_1-m_2)^2$ to the [residual sum of squares](../../../linear-regression.md#residual-sum-of-squares). Here the four differences are $2.4,2.8,-0.1,1.1$, so

$$
\operatorname{RSS}_{\mathrm{pool}}-722.30=5(2.4^2+2.8^2+0.1^2+1.1^2)=74.10.
$$

Therefore $F_{\mathrm{pool}}=2.3083$ and $p\simeq0.0640$. **At $5\%$, the data do not reject the three-type reduction**, though the result is borderline and is not proof that the pooled means are identical. This [factor-level pooling test](../../../statistical-modelling.md#factor-level-pooling-test) keeps the previously supported interaction structure; reducing the categories and removing all interaction simultaneously would test a different set of restrictions.

## 3

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For $\lambda>0$, write the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) mass function in [exponential dispersion family](../../../exponential-family.md#exponential-dispersion-model) form:

$$
f(y;\lambda)=\exp\left\{\frac{y\theta-b(\theta)}{a(\phi)}+c(y,\phi)\right\},\quad
\theta=\log\lambda,\quad b(\theta)=e^\theta,\quad a(\phi)=\phi=1,\quad c(y,1)=-\log(y!).
$$

Thus the [natural parameter of an exponential family](../../../exponential-family.md#natural-parameter-of-an-exponential-family) is **$\theta=\log\lambda$** and the [dispersion parameter](../../../exponential-family.md#dispersion-parameter) is **fixed at $1$**. The counting-measure support is $0,1,\ldots$; there is no independent free dispersion parameter in an ordinary Poisson model. The degenerate boundary $\lambda=0$ is obtained as a limit, rather than a finite natural parameter.

The [exponential dispersion family](../../../exponential-family.md#exponential-dispersion-model) identities give $\mathbb EY=b'(\theta)$ and $\operatorname{Var}(Y)=a(\phi)b''(\theta)$. Since both derivatives of $e^\theta$ equal $e^\theta$,

$$
\boxed{\mathbb EY=\lambda,\qquad\operatorname{Var}(Y)=\lambda.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $Y_i$ be the number of maintenance jobs, $t_i$ average temperature and $p_i$ average precipitation. The fitted [Poisson regression](../../../statistical-modelling.md#poisson-regression) assumes independent conditional responses with

$$
Y_i\mid t_i,p_i\sim\operatorname{Poisson}(\mu_i),\qquad
\log\mu_i=\beta_0+\beta_Tt_i+\beta_Pp_i.
$$

The logarithm is the [Poisson canonical link](../../../statistical-modelling.md#poisson-canonical-link), so fitted means are always positive. The estimated [regression coefficients](../../../linear-regression.md#regression-coefficient) are

$$
\boxed{(\widehat\beta_0,\widehat\beta_T,\widehat\beta_P)=(4.079374,-0.006162,-0.002922).}
$$

At fixed precipitation, one unit of temperature multiplies the fitted mean by $e^{-0.006162}\simeq0.99386$, a decrease of about $0.614\%$. The fitted precipitation multiplier is $e^{-0.002922}\simeq0.99708$ per unit, but its large [p-value](../../../statistical-modelling.md#p-value) gives little evidence for that effect. These are conditional associations, not established causal effects.

The intercept-only model has $n-1=23$ residual degrees of freedom, and the full model has $n-3=21$. Both imply **$n=24$ months**.

For an approximate [deviance goodness-of-fit test](../../../statistical-modelling.md#deviance-goodness-of-fit-test) of the full [Poisson regression](../../../statistical-modelling.md#poisson-regression), compare residual deviance $23.527$ with $\chi^2_{21}$. Its upper-tail [p-value](../../../statistical-modelling.md#p-value) $0.3165361$ supplies **no evidence of lack of fit**. The ratio $23.527/21\simeq1.120$ also gives no striking indication of [overdispersion](../../../exponential-family.md#overdispersion), though deviance per degree of freedom is only a rough dispersion check. Fitted count means around fifty make the usual chi-squared approximation plausible. Independence between months, the conditional variance-equals-mean assumption and the absence of residual structure still need diagnostics. Failure to reject is not proof that the model is correct.

The null deviance $37.969$ on $23$ degrees of freedom has $p=0.02566753$, suggesting the constant-mean model is inadequate. In the sequential [analysis of deviance for nested generalized linear models](../../../statistical-modelling.md#analysis-of-deviance-for-nested-generalized-linear-models), adding temperature to that model reduces deviance by $14.204$ on one degree of freedom, giving $p=0.000164$. Adding precipitation after temperature reduces it by only $0.238$, with $p=0.625677$. Therefore **retain temperature; these data give no reason to retain precipitation after temperature**. The temperature-only residual deviance is $23.765$ on $22$ degrees of freedom. This prediction-oriented reduced model should be refitted before reporting its coefficients: the printed temperature coefficient belongs to the full model. The [Wald test](../../../statistical-modelling.md#wald-test) results, $p=0.000833$ and $0.625582$, broadly support the same conclusion, while the sequential deviance tests answer the stated nested-model questions.

## 4

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Use an [unpenalized intercept in ridge regression](../../../linear-regression.md#unpenalized-intercept-in-ridge-regression). For centered predictor columns, the [ridge regression](../../../linear-regression.md#ridge-regression) optimization is

$$
\min_{\alpha,\beta}\ \|Y-\alpha\mathbf1-X\beta\|_2^2+\lambda\|\beta\|_2^2,\qquad\lambda\geq0.
$$

Differentiating with respect to $\alpha$ gives $\widehat\alpha=\overline Y$. Put $Y_c=Y-\overline Y\mathbf1$. Differentiation with respect to $\beta$ gives the ridge [normal equation](../../../statistical-modelling.md#normal-equation)

$$
(X^TX+\lambda I_6)\widehat\beta_\lambda=X^TY_c.
$$

Consequently the [closed-form ridge regression estimator](../../../linear-regression.md#closed-form-ridge-regression-estimator) is

$$
\boxed{\widehat\beta_\lambda=(X^TX+\lambda I_6)^{-1}X^TY_c,\qquad\widehat\alpha=\overline Y.}
$$

Because $X^T\mathbf1=0$, the numerator may also be written $X^TY$. For $\lambda>0$ the inverse exists even with [multicollinearity](../../../statistical-modelling.md#multicollinearity) or deficient column rank; at $\lambda=0$ a unique [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares) coefficient vector requires full rank. The quadratic penalty stabilizes nearly singular directions but generally does not set individual coefficients exactly to zero.

For uncentered original predictors, use $X_c=X-\mathbf1\overline x^T$, apply the displayed estimator to $X_c,Y_c$, and recover $\widehat\alpha=\overline Y-\overline x^T\widehat\beta$. Any internal scaling used by `lm.ridge` must be undone to report coefficients on the original predictor scale. Multiplying the objective by a constant changes the numerical penalty convention unless $\lambda$ is rescaled as well.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [generalized cross-validation](../../../statistical-learning.md#generalized-cross-validation) curve reaches its minimum at **$\lambda=5$** among the supplied grid values. This balances improved conditioning against shrinkage bias using an estimate of prediction error, rather than choosing the penalty with the smallest training [residual sum of squares](../../../linear-regression.md#residual-sum-of-squares). Nearby values have similar errors, so the plot does not establish a highly precise optimal penalty.

Reading the PDF table at $\lambda=5$ gives the fitted [regression intercept](../../../linear-regression.md#regression-intercept) and slopes:

$$
\boxed{\widehat\alpha=0.8695819,\quad
\widehat\beta=(0.5363716,\ 0.4143406,\ -0.01248621,\ 0.10434493,\ 0.7284822,\ -0.002794344)^T.}
$$

These table entries are necessary because the TeX stores the table only inside a figure. The [ridge regression](../../../linear-regression.md#ridge-regression) slopes are shrunk relative to the zero-penalty fit; their small nonzero values do not represent variable exclusion.

There is a minor source inconsistency: the prose says the predictors are centered, but the table's intercept varies with $\lambda$. With exactly centered predictor columns and an unpenalized intercept it would remain $\overline Y$. The numbers above faithfully report the printed table, while part (a) gives the centered formula and the general uncentered conversion. The table therefore reflects a different or incompletely described preprocessing convention.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

An intercept-unpenalized [Lasso](../../../probability-and-statistics.md#lasso) estimator solves the constrained optimization

$$
\boxed{\min_{\alpha,\beta}\ \|Y-\alpha\mathbf1-X\beta\|_2^2
\quad\text{subject to}\quad\sum_{j=1}^6|\beta_j|\leq t.}
$$

For centered predictors, eliminate the intercept as in [ridge regression](../../../linear-regression.md#ridge-regression) and minimize $\|Y_c-X\beta\|_2^2$ under the same constraint. Equivalently, with a suitable tuning parameter $\lambda\geq0$, use $\|Y-\alpha\mathbf1-X\beta\|_2^2+\lambda\sum_j|\beta_j|$. The constraint radius and penalty parameter are different parametrizations; larger radius permits less shrinkage.

The [Lasso](../../../probability-and-statistics.md#lasso) plot parametrizes the [Lasso regularization path](../../../probability-and-statistics.md#lasso-regularization-path) by the fraction of the maximum $l_1$ norm of the standardized slopes. Unlike the ridge quadratic penalty, the corners of the $l_1$ constraint can place some slopes exactly at zero, providing [variable selection](../../../statistical-modelling.md#variable-selection). The maximum norm refers to the path's unpenalized endpoint; centering and scaling conventions must match those used to construct that path.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

At fraction $0.8$, the [Lasso regularization path](../../../probability-and-statistics.md#lasso-regularization-path) lies between the vertical lines marked steps 4 and 5. In that interval the first five predictors have nonzero slopes: $X_1,X_2,X_4,X_5$ are positive and $X_3$ is negative. The sixth predictor remains at zero until the later part of the path, beyond this fraction. Therefore the chosen [Lasso](../../../probability-and-statistics.md#lasso) model includes

$$
\boxed{X_1,X_2,X_3,X_4,X_5\text{, with }X_6\text{ excluded}.}
$$

The [regression intercept](../../../linear-regression.md#regression-intercept) is retained. In particular the negative $X_3$ trace has already left zero at fraction $0.8$; a small slope is not the same as a zero slope. The selected fraction came from ten-fold [K-fold cross-validation](../../../statistical-learning.md#k-fold-cross-validation), and is not a numerical value of the ridge penalty in the preceding parts.

## 5

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

For a nonnegative [random variable](../../../random-variable.md), $T=\int_0^\infty\mathbf1\{T>t\}\,dt$. [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) permits interchanging expectation and this nonnegative integral, giving the [tail integral formula for moments](../../../probability-theory.md#tail-integral-formula-for-moments):

$$
\boxed{\mathbb ET=\int_0^\infty\mathbb P(T>t)\,dt=\int_0^\infty S(t)\,dt.}
$$

The equality also holds when the mean is infinite. Thus mean completion time is the total area under the [survival function](../../../survival-analysis.md#survival-function), while a [restricted mean survival time](../../../survival-analysis.md#restricted-mean-survival-time) integrates only to a specified follow-up horizon.

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

For a continuous positive [survival time](../../../survival-analysis.md#survival-time), $S'(t)=-f(t)$ and the [hazard function](../../../survival-analysis.md#hazard-function) is $h(t)=f(t)/S(t)$ wherever $S(t)>0$. Therefore

$$
\frac{d}{dt}\log S(t)=-h(t).
$$

Since $S(0)=1$, integrating gives the [cumulative hazard function](../../../survival-analysis.md#cumulative-hazard-function) identity

$$
\boxed{S(t)=\exp\{-H(t)\},\qquad H(t)=\int_0^t h(u)\,du.}
$$

At an endpoint where survival reaches zero, the corresponding cumulative hazard is interpreted as $+\infty$ and the exponential as zero.

<h4 id="5/a/iii">iii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/a/iii)

Continuity of the [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function) gives the [probability integral transform](../../../probability-theory.md#probability-integral-transform): $F(T)$ is uniform on $(0,1)$. Hence $S(T)=1-F(T)$ is also uniform, and the [cumulative hazard probability transformation](../../../survival-analysis.md#cumulative-hazard-probability-transformation) gives

$$
H(T)=-\log S(T),\qquad
\mathbb P\{H(T)>x\}=\mathbb P\{S(T)<e^{-x}\}=e^{-x},\quad x\geq0.
$$

Thus

$$
\boxed{H(T)\sim\operatorname{Exp}(1).}
$$

The [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) has rate and mean one here. This proof does not require a strictly increasing cumulative hazard: intervals with zero density carry no probability mass. It assumes a proper continuous finite survival time, without an atom at infinity.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

The [Kaplan–Meier estimator](../../../survival-analysis.md#kaplan-meier-estimator) is $\widehat S(t)=\prod_{t_j\leq t}(1-d_j/r_j)$, with event count $d_j$ and [risk set](../../../survival-analysis.md#risk-set) size $r_j$. Its median is the first event time with estimated survival at most $1/2$. Since $\widehat S(2)=0.5749$ and $\widehat S(3)=0.4286$, **the estimated median completion time is $3$ minutes**.

The original last event exhausts the final [risk set](../../../survival-analysis.md#risk-set), so the fitted [survival function](../../../survival-analysis.md#survival-function) drops to zero at $18$ and its conventional full area is finite. Integrate the right-continuous step function: its height is one before time one, and after each event the height is the newly computed survival value. There are three-minute gaps from $12$ to $15$ and from $15$ to $18$. Thus

$$
\widehat\mu=1+\sum_{j=1}^{11}\widehat S(j)+3\widehat S(12)+3\widehat S(15)
\simeq\boxed{4.188\text{ minutes}.}
$$

Using the exact risk-set products rather than rounded printed survival values gives $4.187856$. This is not the sample mean of the observed event-or-censoring times; [right censoring](../../../survival-analysis.md#right-censoring) changes the estimated survival weights.

If the final observation at $18$ is instead censored, every earlier [Kaplan–Meier estimator](../../../survival-analysis.md#kaplan-meier-estimator) value is unchanged and no event factor is inserted at $18$. The median remains **$3$ minutes**, but the curve stays at $\widehat S(15)\simeq0.0107$ at the end of follow-up. By [terminal censoring and survival-mean identifiability](../../../survival-analysis.md#terminal-censoring-and-survival-mean-identifiability), **a full unrestricted mean is no longer determined nonparametrically by these observations**. Extending the final positive step forever would give an infinite integral, but that plotting convention does not establish an infinite population mean. Extra assumptions about the unobserved tail would be needed for a finite full-mean estimate.

The [restricted mean survival time](../../../survival-analysis.md#restricted-mean-survival-time) through $18$ is still **$4.187856$ minutes** in either version: the two curves differ only at or after the endpoint, which does not affect the area up to it. All these interpretations require [independent censoring](../../../survival-analysis.md#independent-censoring). Giving up may be related to how long a person would have taken to finish, so that assumption needs scientific justification in this study.

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

Let $a_i$ be age in years, $g_i$ the male indicator and $m_i$ the indicator for the Messiah group. The fitted [Cox proportional-hazards model](../../../survival-analysis.md#cox-proportional-hazards-model) is

$$
h_i(t)=h_0(t)\exp\{0.006536a_i-0.603547g_i+0.755308m_i\},
$$

with an unspecified common [baseline hazard](../../../survival-analysis.md#baseline-hazard). Its coefficients were estimated by [Cox partial likelihood](../../../survival-analysis.md#cox-partial-likelihood), using the [Breslow approximation for tied event times](../../../survival-analysis.md#breslow-approximation-for-tied-event-times). There are $100$ participants, $96$ recorded completions and four censored observations.

A higher [hazard function](../../../survival-analysis.md#hazard-function) means a greater instantaneous chance of completion among those not yet completing, so it describes faster completion rather than greater mortality. Holding gender and group fixed, an extra year of age multiplies the completion hazard by **$1.0066$**, about a $0.66\%$ increase. The 95% [confidence interval](../../../statistical-inference.md#confidence-interval) is $(0.9865,1.0270)$ and the [Wald test](../../../statistical-modelling.md#wald-test) has $p=0.5241$, so there is little evidence of an age association.

Holding age and group fixed, male participants have a [hazard ratio](../../../survival-analysis.md#hazard-ratio) **$0.5469$** relative to female participants, about a $45.3\%$ lower completion hazard. Its 95% [confidence interval](../../../statistical-inference.md#confidence-interval) is $(0.3560,0.8401)$ and $p=0.00586$. Under the fitted model this corresponds to slower completion for males. It is not a ratio of mean or median completion times.

Holding age and gender fixed, participants assigned to Messiah have a [hazard ratio](../../../survival-analysis.md#hazard-ratio) **$2.1283$** relative to The Kingdom, with 95% [confidence interval](../../../statistical-inference.md#confidence-interval) $(1.3653,3.3176)$ and $p=0.000854$. This is strong evidence of a group difference, with faster completion in the Messiah group under the fitted model. Random assignment supports interpreting a group contrast as an effect of the assigned condition, subject to the assumptions about follow-up and censoring; age and gender contrasts remain observational associations.

Each printed $z$ statistic is the coefficient divided by its [standard error](../../../statistical-inference.md#standard-error), using an asymptotic standard normal [sampling distribution](../../../statistical-modelling.md#sampling-distribution) under a zero-coefficient [null hypothesis](../../../statistical-modelling.md#null-hypothesis). The [hazard ratio](../../../survival-analysis.md#hazard-ratio) is $e^\beta$, and its confidence limits exponentiate the coefficient limits. Proportional hazards assumes these covariate-specific hazard multipliers stay constant over follow-up, together with the specified linear age effect and [independent censoring](../../../survival-analysis.md#independent-censoring) conditional on covariates.

<h4 id="5/b/iii">iii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/b/iii)

The command `cox.zph` checks the [proportional hazards assumption test](../../../survival-analysis.md#proportional-hazards-assumption-test) through time dependence of [scaled Schoenfeld residuals](../../../survival-analysis.md#scaled-schoenfeld-residual). Under constant coefficients, their expected trend against transformed event time should be flat. A significant covariate-specific test would suggest that its coefficient varies with time; the global test checks the coefficients jointly.

The [p-values](../../../statistical-modelling.md#p-value) are $0.461$ for age, $0.538$ for gender and $0.882$ for group, with global $p=0.846$. Thus **these tests find no evidence against proportional hazards**. They do not prove the assumption, establish the correct age functional form, or test the censoring mechanism.

The separate diagnostic plot targets the broader fitted survival distribution. The code evaluates a fitted [cumulative hazard function](../../../survival-analysis.md#cumulative-hazard-function) at each observed time and multiplies by the subject's fitted hazard multiplier, forming [Cox–Snell residuals](../../../survival-analysis.md#cox-snell-residual):

$$
r_i=\widehat H_i(T_i)=\widehat H_{\mathrm{ref}}(T_i)\exp\{\widehat\eta_i\}.
$$

The curve returned without `newdata` by `survfit` is a reference-profile curve, not necessarily the all-zero-covariate baseline. The multiplier must use the same centering as that reference curve; the fitted linear predictors use the model's reference convention. With this consistency, $-\log\widehat S_{\mathrm{ref}}$ times the multiplier is the fitted subject-specific cumulative hazard.

Part (a) shows why complete transformed event times should be approximately unit exponential if the [Cox proportional-hazards model](../../../survival-analysis.md#cox-proportional-hazards-model) is correct. The Q–Q plot compares ordered fitted residuals with an independent random exponential sample. Most points are near the diagonal, with some upper-tail departures, so it gives **no obvious indication of a gross distributional failure**. A random reference sample adds simulation noise, and estimated parameters and tied recorded times prevent this from being an exact distribution-free test.

Importantly, four observed times are censored. Their transformed times retain the censoring indicators and are not complete exponential observations. Simply plotting all $100$ residuals as uncensored therefore gives only a rough visual check. A more appropriate [Cox–Snell residual survival diagnostic](../../../survival-analysis.md#cox-snell-residual-survival-diagnostic) fits a [Kaplan–Meier estimator](../../../survival-analysis.md#kaplan-meier-estimator) or [Nelson–Aalen estimator](../../../survival-analysis.md#nelson-aalen-estimator) to $(r_i,D_i)$, retains the censoring flags, and checks whether the estimated cumulative hazard is close to $r$, equivalently whether estimated survival is close to $e^{-r}$. Taken together, the supplied checks are broadly compatible with the fitted model, while none resolves potentially [informative censoring](../../../survival-analysis.md#informative-censoring) from giving up.

## 6

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

For a [finite Gaussian mixture with a common variance](../../../statistical-modelling.md#finite-gaussian-mixture-with-a-common-variance), introduce independent latent labels $Z_i\in\{1,\ldots,k\}$ with probabilities $\pi_j>0$, $\sum_j\pi_j=1$, and conditional responses $Y_i\mid Z_i=j\sim N(\mu_j,\sigma^2)$, with common $\sigma^2>0$. The observed density and [log-likelihood](../../../statistical-modelling.md#log-likelihood) are

$$
f(y)=\sum_{j=1}^k\pi_j\phi(y;\mu_j,\sigma^2),\qquad
\ell=\sum_{i=1}^n\log\left\{\sum_j\pi_j\phi(y_i;\mu_j,\sigma^2)\right\}.
$$

The [expectation-maximization algorithm](../../../statistical-modelling.md#expectation-maximization-algorithm) replaces the difficult log of sums by an expected complete-data objective. Choose positive initial weights and variance and separated initial means. At iteration $r$, the E-step computes the [mixture responsibilities](../../../statistical-modelling.md#mixture-responsibility)

$$
\tau_{ij}^{(r)}=\mathbb P_{\theta^{(r)}}(Z_i=j\mid y_i)
=\frac{\pi_j^{(r)}\exp\{-(y_i-\mu_j^{(r)})^2/(2\sigma^{2(r)})\}}
{\sum_{l=1}^k\pi_l^{(r)}\exp\{-(y_i-\mu_l^{(r)})^2/(2\sigma^{2(r)})\}}.
$$

The common normalizing factor cancels. For numerical stability the probabilities can be evaluated by subtracting the largest log weight before exponentiating.

With the old responsibilities held fixed, the expected complete-data [log-likelihood](../../../statistical-modelling.md#log-likelihood), up to irrelevant constants, is

$$
Q=\sum_{i,j}\tau_{ij}^{(r)}\log\pi_j-\frac n2\log\sigma^2
-\frac1{2\sigma^2}\sum_{i,j}\tau_{ij}^{(r)}(y_i-\mu_j)^2.
$$

Let $N_j=\sum_i\tau_{ij}^{(r)}$. A Lagrange multiplier for $\sum_j\pi_j=1$, weighted least squares for the means, and differentiation in the common variance give the M-step:

$$
\boxed{\pi_j^{(r+1)}=\frac{N_j}{n},\qquad
\mu_j^{(r+1)}=\frac{\sum_i\tau_{ij}^{(r)}y_i}{N_j},\qquad
\sigma^{2(r+1)}=\frac1n\sum_{i,j}\tau_{ij}^{(r)}(y_i-\mu_j^{(r+1)})^2.}
$$

The variance update uses the **new means and old responsibilities**, with denominator $n$, not a residual degrees-of-freedom adjustment: this is [maximum likelihood estimation](../../../statistical-modelling.md#maximum-likelihood-estimation). Repeat the E- and M-steps until the observed [log-likelihood](../../../statistical-modelling.md#log-likelihood) and parameters stabilize.

By [EM likelihood monotonicity](../../../statistical-modelling.md#em-likelihood-monotonicity), exact updates do not decrease the observed likelihood. They need not reach its global maximum, so use several starting configurations and keep the best converged fit, checking for empty or nearly empty components and vanishing variance. The labels are interchangeable; sorting means after fitting supplies an interpretable labeling. Distinct starting means do not guarantee that all fitted components remain distinct. With a common variance and the usual fixed small $k$ relative to distinct observations the model avoids the individual-component variance-collapse pathology of unrestricted Gaussian mixtures, but degenerate data or too many components still require attention.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

The statistician first models the age- and gender-dependent mean by [linear regression](../../../linear-regression.md). Its fitted value is $27.01675-0.10483\,\mathrm{age}+1.47031\,\mathrm{gender}$. At fixed gender, a year of age is associated with a decrease of $0.10483$ BMI units; the group coded gender $1$ has a fitted mean $1.47031$ units above the group coded $0$ at the same age. This question does not state which gender receives which code. The intercept refers to age zero in the reference group, outside a typical adult-patient range, so its substantive interpretation is limited. Both slope [Student t-tests](../../../statistical-modelling.md#student-s-t-test) have small [p-values](../../../statistical-modelling.md#p-value), and the overall [F-test](../../../probability-and-statistics.md#f-test) supports an age/gender-dependent mean. The [coefficient of determination](../../../linear-regression.md#coefficient-of-determination) is only $0.18$, leaving considerable individual variation to investigate.

The residual diagnostics check whether mean adjustment is plausible and whether a single normal error law is adequate. The [residual-versus-fitted plot](../../../linear-regression.md#residual-versus-fitted-plot) has no strong curved mean trend, although its smooth curve is not perfectly flat. The [scale-location plot](../../../linear-regression.md#scale-location-plot) suggests some decline in spread as fitted BMI increases, so common residual variance is a working approximation rather than an established fact. The normal [Q-Q plot](../../../probability-and-statistics.md#q-q-plot) has systematic departures, notably shorter tails than the normal reference, suggesting the residual law is not exactly normal. The [regression leverage](../../../statistical-modelling.md#regression-leverage) plot does not display an obviously extreme leverage point, but the marked observations and [Cook's distance](../../../statistical-modelling.md#cook-s-distance) should still be checked for influence. Independence between patients cannot be diagnosed from these four plots alone.

Next the statistician extracts the [regression residuals](../../../probability-and-statistics.md#regression-residual) and fits an intercept-only normal model as a baseline residual distribution. With an intercept in the original [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares) model, the residuals sum to zero by the [normal equation](../../../statistical-modelling.md#normal-equation); the near-zero fitted residual mean and its $p=1$ are therefore automatic, not new evidence of good fit. The $2.698$ standard error in this refit uses $499$ degrees of freedom, whereas the original $2.704$ uses $497$ after estimating three regression coefficients. The reported [log-likelihood](../../../statistical-modelling.md#log-likelihood) for the single-normal residual model is $-1205.25$.

The histogram suggests a shape worth exploring beyond one normal density, with broad shoulders and some asymmetry, without showing unambiguous separated clusters. The statistician fits two- and three-component [finite Gaussian mixtures with a common variance](../../../statistical-modelling.md#finite-gaussian-mixture-with-a-common-variance) by the [expectation-maximization algorithm](../../../statistical-modelling.md#expectation-maximization-algorithm), starting from separated means and positive weights. Successive likelihoods increase and the displayed final iterations stabilize, as expected from [EM likelihood monotonicity](../../../statistical-modelling.md#em-likelihood-monotonicity). This is evidence of numerical convergence from those starts, not proof of a global maximum.

The two-component fit assigns weights $(0.3317,0.6683)$, residual means $(-2.7844,1.3819)$ and common variance $3.4175$. The three-component fit assigns weights $(0.2051,0.3926,0.4023)$, residual means $(-3.7306,-0.4417,2.3329)$ and common variance $2.1448$. The code correctly passes the square roots of those variances to `dnorm` and overlays the resulting weighted densities. Both curves broadly follow the histogram and are very similar. In particular, a two-component mixture need not have two distinct visible modes.

These fits explore [residual mixture clustering](../../../statistical-modelling.md#residual-mixture-clustering): groups differ in BMI relative to the same age/gender-adjusted mean, rather than simply in raw BMI. Membership can be summarized by the fitted [mixture responsibilities](../../../statistical-modelling.md#mixture-responsibility), retaining uncertainty instead of asserting a certain label for each patient. The common-variance assumption is economical, but should be checked; the common regression slope assumption and constancy of mixture proportions across age and gender are also substantive. A residual mixture alone does not establish genuine biological subpopulations; a flexible continuous distribution, missing predictors, nonlinear mean effects or [heteroscedasticity](../../../statistical-modelling.md#heteroscedastic) could explain a similar marginal shape.

There is also a [two-stage residual mixture fitting](../../../statistical-modelling.md#two-stage-residual-mixture-fitting) limitation. Fitted [regression residuals](../../../probability-and-statistics.md#regression-residual) are not exactly independent identically distributed observations: even under a normal regression, their [covariance matrix](../../../variance.md#covariance-matrix) is $\sigma^2(I-H)$, and estimating the mean adjustment introduces uncertainty. With $500$ subjects and three initial regression coefficients, treating them as independent is a useful approximation for exploring shape, but ordinary mixture likelihoods omit the first-stage uncertainty. A joint [mixture regression with shared slopes](../../../statistical-modelling.md#mixture-regression-with-shared-slopes), or a suitable bootstrap of the whole analysis, would give a firmer basis for parameter uncertainty and cluster selection. Examine component membership versus age/gender and repeat the algorithm from multiple starts before making substantive clustering claims.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

The three-component [finite Gaussian mixture with a common variance](../../../statistical-modelling.md#finite-gaussian-mixture-with-a-common-variance) has the largest displayed maximized [log-likelihood](../../../statistical-modelling.md#log-likelihood), but it also has more fitted parameters. For $k$ components there are $k-1$ free weights, $k$ means and one common variance, making **$d=2k$** residual-distribution parameters. Applying the nominal [Akaike information criterion](../../../statistical-modelling.md#akaike-information-criterion) and [Bayesian information criterion](../../../statistical-modelling.md#bayesian-information-criterion) to the three residual fits gives

$$
\begin{array}{c|r|r|r|r}
 k&\ell&d&\mathrm{AIC}=-2\ell+2d&\mathrm{BIC}=-2\ell+d\log500\\\hline
1&-1205.2500&2&2414.500&2422.929\\
2&-1193.8265&4&2395.653&2412.511\\
3&-1192.2715&6&2396.543&2421.831
\end{array}
$$

Both criteria favour **the two-component model**. It improves the likelihood substantially over one normal component; the third component gains only $1.5550$ in log-likelihood at a cost of two further parameters. The [Akaike information criterion](../../../statistical-modelling.md#akaike-information-criterion) difference between two and three components is small, about $0.89$, so that criterion alone gives only a slight preference; the [Bayesian information criterion](../../../statistical-modelling.md#bayesian-information-criterion) preference for two is stronger. Their nearly indistinguishable overlaid curves also support retaining the simpler two-component fit.

These calculations are model-selection aids, not an exact test. Ordinary chi-squared calibration of a [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test) for the number of mixture components is invalid in general: under a smaller-component null, some weights lie on the boundary and extra-component parameters are unidentified. This is [nonregular mixture model selection](../../../statistical-modelling.md#nonregular-mixture-model-selection). A parametric bootstrap or predictive [cross-validation](../../../statistical-learning.md#cross-validation) is preferable for a formal comparison, and should account for the mean-adjustment stage. The table uses the provided residual likelihoods and their nominal parameter counts; first-stage regression uncertainty and possible local EM maxima remain qualifications. **On the supplied evidence, select two components without claiming that two distinct biological groups have been established.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
