# Paper 41

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper41.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper41.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [Solution](#3/solution)
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

## 1

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write $q=n-p$. In this [normal linear model](../../../statistical-modelling.md#normal-linear-model), the [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares) criterion is $\|Y-Xb\|^2$. Differentiating with respect to $b$ gives the [normal equations for linear least squares](../../../linear-regression.md#normal-equations-for-linear-least-squares), $X^TXb=X^TY$. Full column rank of the [design matrix](../../../linear-regression.md#design-matrix) makes $X^TX$ invertible, and completing the square proves that the unique minimum is

$$
\boxed{\widehat\beta=(X^TX)^{-1}X^TY.}
$$

Since $\widehat\beta=\beta+(X^TX)^{-1}X^T\epsilon$, its [sampling distribution](../../../statistical-modelling.md#sampling-distribution) is the [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution)

$$
\widehat\beta\sim N_p\bigl(\beta,\sigma^2(X^TX)^{-1}\bigr).
$$

Let $H=X(X^TX)^{-1}X^T$ be the [hat matrix](../../../statistical-modelling.md#hat-matrix). It is symmetric and idempotent with rank $p$, and $HX=X$. The [regression residual](../../../probability-and-statistics.md#regression-residual) vector is $(I-H)Y=(I-H)\epsilon$, so

$$
\operatorname{RSS}=\|Y-X\widehat\beta\|^2=Y^T(I-H)Y,\qquad \boxed{s^2=\frac{\operatorname{RSS}}{n-p}.}
$$

An [orthogonal projection of a Gaussian vector](../../../probability-and-statistics.md#orthogonal-projection-of-a-gaussian-vector) onto the residual space gives $\operatorname{RSS}/\sigma^2\sim\chi^2_q$. The residual projection and fitted projection have zero cross-[covariance](../../../variance.md#covariance), hence are [independent](../../../random-variable.md#independent-random-variables) because they are jointly [normal](../../../probability-theory.md#normal-distribution). In particular, $s^2$ is an [unbiased estimator](../../../statistical-modelling.md#unbiased-estimator) of $\sigma^2$ and is [independent](../../../random-variable.md#independent-random-variables) of $\widehat\beta$. The [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator) of $\sigma^2$ instead divides by $n$ and is not unbiased.

For the [null hypothesis](../../../statistical-modelling.md#null-hypothesis) $\beta_1=0$, put $v_{11}=((X^TX)^{-1})_{11}$. Under that [null hypothesis](../../../statistical-modelling.md#null-hypothesis), $\widehat\beta_1/(\sigma\sqrt{v_{11}})$ is standard [normal](../../../probability-theory.md#normal-distribution) and independent of $qs^2/\sigma^2$. Therefore the [Student t-test](../../../statistical-modelling.md#student-s-t-test) uses

$$
T=\frac{\widehat\beta_1}{s\sqrt{v_{11}}}\sim t_q.
$$

**A two-sided level-$\alpha$ test rejects when $|T|>t_{q,1-\alpha/2}$.** The denominator is the estimated [standard error](../../../statistical-inference.md#standard-error) of the [regression coefficient](../../../linear-regression.md#regression-coefficient).

The fitted [linear regression](../../../linear-regression.md) includes an [intercept](../../../linear-regression.md#regression-intercept) and three [covariates](../../../statistical-model.md#covariate):

$$
\operatorname{NO2}_i=\beta_0+\beta_w\operatorname{wind}_i+\beta_t\operatorname{maxtemp}_i+\beta_s\operatorname{insol}_i+\epsilon_i,\qquad \epsilon_i\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

Thus $n=25$, $p=4$ and the residual [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom) are $21$. The fitted [conditional mean](../../../measure-theory.md#conditional-expectation) is

$$
\widehat{\operatorname{NO2}}=3.784916-0.527410\operatorname{wind}+0.124991\operatorname{maxtemp}-0.005259\operatorname{insol}.
$$

Each slope measures a conditional association with the response while the other two [covariates](../../../statistical-model.md#covariate) are held fixed. Increasing wind speed by one mile per hour corresponds to a fitted decrease of $0.527410$ in the concentration units used. Its [standard error](../../../statistical-inference.md#standard-error) is $0.224904$, giving $t=-2.345$ and a two-sided [p-value](../../../statistical-modelling.md#p-value) of $0.0289$: evidence of a negative conditional association at the 5% level. The temperature slope is $0.124991$ per degree Fahrenheit, with [standard error](../../../statistical-inference.md#standard-error) $0.075173$, $t=1.663$ and [p-value](../../../statistical-modelling.md#p-value) $0.1112$. The insolation slope is $-0.005259$ per langley per day, with [standard error](../../../statistical-inference.md#standard-error) $0.006637$, $t=-0.792$ and [p-value](../../../statistical-modelling.md#p-value) $0.4370$. Neither of these last two conditional effects is significant at 5%; that does not establish that either true slope is zero. These are associations, not a demonstration of causal effects.

The [intercept](../../../linear-regression.md#regression-intercept) estimates the mean at zero values of all three [covariates](../../../statistical-model.md#covariate). Its value $3.784916$ has a large [standard error](../../../statistical-inference.md#standard-error) $7.979647$, giving $t=0.474$ and [p-value](../../../statistical-modelling.md#p-value) $0.6402$. The zero-covariate combination may be outside the observed range, so this test may have little practical relevance. Every coefficient test uses a [Student t-distribution](../../../continuous-probability-distribution.md#student-s-t-distribution) with $21$ [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom).

The reported residual [standard deviation](../../../variance.md#standard-deviation) $s=1.844$ measures unexplained variation in concentration units; the subsequent table gives $\operatorname{RSS}=71.428$, consistent with $s=\sqrt{71.428/21}$ after rounding. The five-number residual summary describes the spread, from $-2.3052$ to $3.4033$, with median $-0.4990$. An [intercept](../../../linear-regression.md#regression-intercept) forces the residual sum to zero, not the residual median. These five numbers alone cannot establish [normal](../../../probability-theory.md#normal-distribution) errors, constant [variance](../../../variance.md) or [independence](../../../random-variable.md#independent-random-variables); residual-versus-fitted and [quantile-quantile plots](../../../probability-and-statistics.md#q-q-plot) would be more informative, and successive days also warrant checking serial dependence. The [coefficient of determination](../../../linear-regression.md#coefficient-of-determination) $R^2=0.6533$ means that 65.33% of the sample response sum of squares about its mean is explained by this fit. Its adjusted version is

$$
\overline R^2=1-\frac{\operatorname{RSS}/21}{\operatorname{TSS}/24}=0.6037,
$$

which accounts for the number of estimated [regression coefficients](../../../linear-regression.md#regression-coefficient).

The [stepwise selection by the Akaike information criterion](../../../statistical-modelling.md#stepwise-selection-by-the-akaike-information-criterion) searches between the intercept-only model and the specified model with all three main effects. For these [Gaussian](../../../probability-theory.md#normal-distribution) fits, the printed [Akaike information criterion](../../../statistical-modelling.md#akaike-information-criterion) is, up to a constant common to the candidates,

$$
\operatorname{AIC}=25\log(\operatorname{RSS}/25)+2p.
$$

The full model has $p=4$ and AIC $34.246$. Removing insolation increases the [residual sum of squares](../../../linear-regression.md#residual-sum-of-squares) by $2.136$ but decreases AIC to $32.982$, so that removal is chosen. Removing temperature or wind instead would give AIC $35.337$ or $38.060$ and is worse. In the next step the candidate models include deletions and restoration of insolation. Keeping wind and temperature has the smallest AIC: removing temperature gives $33.389$, restoring insolation gives $34.246$, and removing wind gives $37.960$. Hence the search stops, giving

$$
\boxed{\widehat{\operatorname{NO2}}=4.4368-0.5734\operatorname{wind}+0.1040\operatorname{maxtemp}.}
$$

The accompanying [F-tests](../../../probability-and-statistics.md#f-test) compare a larger model with a one-parameter reduction: $F=\Delta\operatorname{RSS}/s^2$, where $s^2$ is estimated from the larger model. For example, removing insolation gives $2.136/(71.428/21)=0.628$, equal to the corresponding squared [test statistic](../../../statistical-modelling.md#test-statistic). Deletions from the second-stage model use $73.564/22$ in the denominator, whereas restoring insolation uses the full-model denominator. These tests describe the comparisons; they do not determine the AIC choice. In particular, temperature is retained despite its deletion-test [p-value](../../../statistical-modelling.md#p-value) $0.15016$. AIC balances fit and complexity, and a stepwise optimum need not be a global optimum over a richer model class. Ordinary coefficient inference after choosing a model does not account for the selection itself.

For positive responses, the [Box–Cox transformation](../../../statistical-modelling.md#box-cox-transformation) is $T_\lambda(y)=(y^\lambda-1)/\lambda$ for $\lambda\ne0$, and $T_0(y)=\log y$. Its [profile likelihood](../../../statistical-modelling.md#profile-likelihood) refits the [linear regression](../../../linear-regression.md) and [variance](../../../variance.md) at each $\lambda$ and includes the transformation Jacobian. The graph peaks at roughly $\lambda=0.3$–$0.4$. The approximate 95% [likelihood-ratio confidence interval](../../../statistical-inference.md#likelihood-ratio-confidence-interval) contains values a little below zero through approximately one, using the cutoff $\ell_{\max}-\chi^2_{1,0.95}/2$. Thus a [logarithmic transformation](../../../statistical-modelling.md#logarithmic-transformation) ($\lambda=0$) and a square-root transformation ($\lambda=1/2$) are plausible, while leaving the response on its original scale ($\lambda=1$) is at or very near the upper confidence boundary. **The broad profile supports considering a mild power transformation; it does not determine a sharply estimated power.** The raster does not justify more precise endpoints or a decisive assertion about which side of the boundary $\lambda=1$ lies.

## 2

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let $m=\overline Y_{+++}$, $r_i=\overline Y_{i++}$ and $c_j=\overline Y_{+j+}$. The proposed [least-squares estimators](../../../statistical-modelling.md#ordinary-least-squares-estimators) satisfy the sum-to-zero constraints because $\sum_i r_i=Im$ and $\sum_j c_j=Jm$. Define $e_{ijk}=Y_{ijk}-r_i-c_j+m$. Direct summation gives

$$
\sum_{j,k}e_{ijk}=0\quad\hbox{for every }i,\qquad \sum_{i,k}e_{ijk}=0\quad\hbox{for every }j.
$$

Now write any other admissible parameters as $\mu=m+u$, $\alpha_i=r_i-m+a_i$, $\beta_j=c_j-m+b_j$, where $\sum_i a_i=\sum_j b_j=0$. Expanding the [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares) criterion, the cross-products with $e$ vanish by the preceding identities. The cross-products between $u$, $a_i$ and $b_j$ vanish by their zero sums. Consequently

$$
S=\sum_{i,j,k}e_{ijk}^2+IJK u^2+JK\sum_i a_i^2+IK\sum_j b_j^2.
$$

Every added term is nonnegative and all vanish only at $u=0$, $a_i=b_j=0$. This proves the unique constrained minimum, with

$$
\boxed{\widehat\mu=m,\qquad\widehat\alpha_i=r_i-m,\qquad\widehat\beta_j=c_j-m.}
$$

The additive-model [residual sum of squares](../../../linear-regression.md#residual-sum-of-squares) and intercept-only [residual sum of squares](../../../linear-regression.md#residual-sum-of-squares) are therefore

$$
\operatorname{RSS}_1=\sum_{i,j,k}(Y_{ijk}-r_i-c_j+m)^2,\qquad \operatorname{RSS}_0=\sum_{i,j,k}(Y_{ijk}-m)^2.
$$

The same [orthogonality](../../../linear-algebra.md#orthogonal-vectors) gives the [analysis of variance](../../../linear-regression.md#analysis-of-variance) identity

$$
\operatorname{RSS}_0=\operatorname{RSS}_1+SS_A+SS_B,\qquad SS_A=JK\sum_i(r_i-m)^2,\quad SS_B=IK\sum_j(c_j-m)^2.
$$

Fitting factor B alone yields fitted values $c_j$ and residual sum $\operatorname{RSS}_0-SS_B$. Fitting A alone gives residual sum $\operatorname{RSS}_0-SS_A$. Adding B after A then reduces it to $\operatorname{RSS}_1$, a reduction of $SS_B$ again. **The reduction due to B is $SS_B$ in either order.** This is [balanced factorial orthogonality](../../../linear-regression.md#balanced-factorial-orthogonality); it generally fails for unequal cell replication.

There are $12$ observations. The additive model estimates $1+(3-1)+(2-1)=4$ independent parameters, so the missing [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom) are **A: 2, B: 1, residuals: 8**. The individual requested residual sums are below.

To check for an [interaction](../../../statistical-model.md#interaction-statistics), extend the [normal linear model](../../../statistical-modelling.md#normal-linear-model) to $\mu+\alpha_i+\beta_j+\gamma_{ij}$, with each row and column sum of $\gamma$ zero. Equivalently, fit the six unrestricted cell means. Its [residual sum of squares](../../../linear-regression.md#residual-sum-of-squares) is the within-cell sum

$$
\operatorname{RSS}_{\mathrm{cell}}=\sum_{i,j,k}(Y_{ijk}-\overline Y_{ij+})^2.
$$

The interaction adds $(I-1)(J-1)=2$ parameters; the cell-means residual has $IJ(K-1)=6$ [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom). Under the no-interaction [null hypothesis](../../../statistical-modelling.md#null-hypothesis) and the independent equal-variance [normal](../../../probability-theory.md#normal-distribution) error model,

$$
\boxed{F=\frac{(2.6867-\operatorname{RSS}_{\mathrm{cell}})/2}{\operatorname{RSS}_{\mathrm{cell}}/6}\sim F_{2,6}.}
$$

The numerator and denominator arise from orthogonal [Gaussian](../../../probability-theory.md#normal-distribution) projections, proving the exact [F-test](../../../probability-and-statistics.md#f-test). Reject for a sufficiently large value. The printed additive [analysis of variance](../../../linear-regression.md#analysis-of-variance) table does not supply $\operatorname{RSS}_{\mathrm{cell}}$, so it cannot determine this test statistic numerically; the replicated cell data would do so.

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The intercept-only [residual sum of squares](../../../linear-regression.md#residual-sum-of-squares) contains both main-effect sums and the additive-model residual: **$\operatorname{RSS}_0=12.7400+0.4033+2.6867=15.8300$**. Its residual [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom) are $12-1=11$.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The additive-model [residual sum of squares](../../../linear-regression.md#residual-sum-of-squares) is the reported residual entry: **$\operatorname{RSS}_1=2.6867$**, with $8$ residual [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom).

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

By [balanced factorial orthogonality](../../../linear-regression.md#balanced-factorial-orthogonality), omitting B adds $SS_B$ to the full additive residual: **$\operatorname{RSS}_{A\text{-only}}=2.6867+0.4033=3.0900$**. This model has $3$ parameters and $9$ residual [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom).

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

By [balanced factorial orthogonality](../../../linear-regression.md#balanced-factorial-orthogonality), omitting A adds $SS_A$ to the additive residual: **$\operatorname{RSS}_{B\text{-only}}=2.6867+12.7400=15.4267$**. This model has $2$ parameters and $10$ residual [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom).

## 3

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) has probability mass $e^{-\mu}\mu^y/y!=\exp\{y\theta-e^\theta-\log(y!)\}$, where $\theta=\log\mu$. It is an [exponential family](../../../exponential-family.md) with $b(\theta)=e^\theta$, mean $\mu$ and [variance](../../../variance.md) $\mu$. The responses are independent, their linear predictors are $x_i^T\beta$, and the [log link](../../../statistical-modelling.md#logarithmic-link-function) relates these predictors to their means. These are precisely the components of a [generalized linear model](../../../statistical-modelling.md#generalized-linear-model); the [log link](../../../statistical-modelling.md#logarithmic-link-function) is its [canonical link function](../../../statistical-modelling.md#canonical-link-function) and the dispersion is one.

The [log-likelihood](../../../statistical-modelling.md#log-likelihood) and [score function](../../../statistical-modelling.md#informant-function) are

$$
\ell(\beta)=\sum_i\{y_i x_i^T\beta-e^{x_i^T\beta}-\log(y_i!)\},\qquad U(\beta)=\sum_i x_i\{y_i-e^{x_i^T\beta}\}.
$$

Thus a finite [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator) satisfies

$$
\boxed{\sum_i x_i(y_i-\widehat\mu_i)=0,\qquad\widehat\mu_i=e^{x_i^T\widehat\beta}.}
$$

The Hessian is $-\sum_i\mu_i x_ix_i^T$; with a full-rank [design matrix](../../../linear-regression.md#design-matrix) it is negative definite at finite parameter values, so a finite solution is the unique maximum. A finite maximum need not exist for every possible response/design combination; the displayed equations describe it when it does exist. If the first component of every $x_i$ is one, the first score equation gives **$\sum_i y_i=\sum_i\widehat\mu_i$**.

The saturated model fits each mean as $y_i$, with the limiting mean zero allowed for a zero count. Subtracting the fitted [log-likelihood](../../../statistical-modelling.md#log-likelihood) from the saturated [log-likelihood](../../../statistical-modelling.md#log-likelihood) gives the [Poisson deviance](../../../statistical-modelling.md#poisson-deviance)

$$
\boxed{D=2\sum_i\left[y_i\log\frac{y_i}{\widehat\mu_i}-(y_i-\widehat\mu_i)\right],}
$$

where $0\log(0/\widehat\mu_i)=0$. With an [intercept](../../../linear-regression.md#regression-intercept), the sum of the second terms is zero, but retaining them is necessary without that score equation.

Take low pH as a [reference level](../../../statistical-modelling.md#reference-level-in-a-regression-factor). For group $j$, the model with [interaction](../../../statistical-model.md#interaction-statistics) has

$$
Y_i\sim\operatorname{Poisson}(\mu_i),\qquad \log\mu_i=\alpha+\gamma_j+(\beta+\delta_j)b_i,\qquad \gamma_{\mathrm{low}}=\delta_{\mathrm{low}}=0,
$$

where $b_i$ is biomass. The additive model sets every $\delta_j$ to zero. The [interaction](../../../statistical-model.md#interaction-statistics) model estimates six parameters and the additive model four. In the additive model the log-mean curves are parallel straight lines, while the mean curves are positive exponentials with fixed ratios $e^{\gamma_j-\gamma_k}$. In the [interaction](../../../statistical-model.md#interaction-statistics) model the log-mean slopes differ, and the mean ratio is $e^{\gamma_j-\gamma_k+(\delta_j-\delta_k)b}$. The following sketches illustrate [common versus factor-specific slopes in Poisson regression](../../../statistical-modelling.md#common-versus-factor-specific-slopes-in-poisson-regression); their coefficients are illustrative, not estimates from the data.

<a id="3/image-illustrative-poisson-mean-curves-with-common-and-ph-specific-biomass-slopes"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41-biomass-models.png)

**[Figure 1](#3/image-illustrative-poisson-mean-curves-with-common-and-ph-specific-biomass-slopes). Illustrative Poisson mean curves with common and pH-specific biomass slopes**.

The additive model is nested in the [interaction](../../../statistical-model.md#interaction-statistics) model with two restrictions. The [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test) therefore uses

$$
D_{\mathrm{add}}-D_{\mathrm{int}}=99.2-83.2=16.0\ \stackrel{H_0}{\approx}\ \chi^2_2,
$$

whose [p-value](../../../statistical-modelling.md#p-value) is $e^{-8}=0.0003355$. **There is strong evidence that the biomass slope on the log-mean scale depends on pH.** The interaction-model residual [deviance](../../../exponential-family.md#exponential-family-deviance) $83.2$ is close to its $90-6=84$ residual [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom), giving no obvious indication of [overdispersion](../../../exponential-family.md#overdispersion) from this comparison alone. The supplied deviances contain no slope estimates: they do not establish which pH group has more species, whether each slope is positive or negative, or whether any actual curves cross. Those conclusions require the fitted coefficients and their uncertainty.

## 4

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

**The Fort Worth observation for ages 75–84 is missing.** It is not a zero count and cannot be replaced by one. The missing cell prevents a direct two-city comparison in that age group and leaves an unbalanced age-by-city table. The youngest groups have only one and four cases, so [chi-squared asymptotic approximations](../../../probability-theory.md#chi-squared-asymptotic-approximation) to tests and uncertainty may be poor there. The open-ended oldest group and broad age bands can conceal different within-group age compositions between cities.

The denominators are population counts rather than reported person-time, and the observation period is not specified. Comparable coverage, case definitions and time periods must therefore be established before interpreting the numbers as comparable incidence measures. The data contain no information on potential [confounders](../../../causal-inference.md#confounder) such as individual risk factors or differences in ascertainment. These are aggregated observations on women in the listed ages, and any fitted city association is not automatically causal or generalizable beyond that population.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Index city by $g\in\{0,1\}$ and age group by $j$, with the youngest group the [reference level](../../../statistical-modelling.md#reference-level-in-a-regression-factor). For each of the 15 observed cells, the [grouped-binomial logistic regression](../../../statistical-modelling.md#grouped-binomial-logistic-regression) assumes

$$
C_{gj}\sim\operatorname{Binomial}(N_{gj},\pi_{gj}),\qquad \log\frac{\pi_{gj}}{1-\pi_{gj}}=\alpha+a_j+\gamma g,\qquad a_{15\text{–}24}=0,
$$

with independent cell counts. The response supplied to R is $C_{gj}/N_{gj}$, and the weights specify the binomial numbers of trials $N_{gj}$. They are not 15 arbitrary precision weights: the conditional [variance](../../../variance.md) of the proportion is $\pi_{gj}(1-\pi_{gj})/N_{gj}$. The [logit link](../../../statistical-modelling.md#logit) models log odds, and the two sets of factor coefficients use corner-point constraints.

There are nine parameters: one [intercept](../../../linear-regression.md#regression-intercept), seven age contrasts and one city contrast. Hence the residual [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom) are $15-9=6$, not the total population minus nine. The null model has only an [intercept](../../../linear-regression.md#regression-intercept) and $14$ residual [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom). Adding age uses seven more parameters and reduces the [binomial deviance](../../../statistical-modelling.md#binomial-deviance) from $2330.46$ to $232.28$, a drop of $2098.19$. Adding city then uses one parameter and reduces it by $227.12$ to $5.15$. These are sequential [likelihood-ratio tests](../../../statistical-modelling.md#likelihood-ratio-test), asymptotically compared with [chi-squared distributions](../../../probability-theory.md#chi-squared-distribution) on seven and one [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom). Both provide extremely strong evidence of an effect; the printed age [p-value](../../../statistical-modelling.md#p-value) $0.00$ is rounding, not an exactly zero probability. Because the table is incomplete, sequential main-effect sums need not be invariant to the order of fitting.

The [intercept](../../../linear-regression.md#regression-intercept) estimate $-11.69364$ is the log odds for the youngest Minneapolis–Saint Paul group. It implies baseline odds $e^{-11.69364}$ and a fitted probability about $8.35\times10^{-6}$. Its [standard error](../../../statistical-inference.md#standard-error) is $0.44923$; its reported [Wald test](../../../statistical-modelling.md#wald-test) tests log odds zero, or probability $1/2$, rather than a scientifically interesting comparison of groups.

The age coefficients are log [odds ratios](../../../statistical-modelling.md#odds-ratio) relative to the youngest group within the same city. Their exponentials are approximately $13.86$, $46.82$, $99.03$, $162.23$, $284.38$, $497.07$ and $484.57$ as age increases through the seven other groups. All these comparisons have large positive [Wald statistics](../../../statistical-modelling.md#wald-test) and small [p-values](../../../statistical-modelling.md#p-value). Thus the fitted probabilities are much higher in the older groups than in the youngest group. The slightly smaller coefficient in the oldest group than in the preceding group does not itself prove a real decline: that claim needs a contrast and its [standard error](../../../statistical-inference.md#standard-error), including the [covariance](../../../variance.md#covariance) of the two estimates.

The city coefficient $0.85492$ is the log [odds ratio](../../../statistical-modelling.md#odds-ratio) for Fort Worth relative to Minneapolis–Saint Paul, adjusted for age. Its [standard error](../../../statistical-inference.md#standard-error) $0.05969$ gives $z=14.322$, so the null city effect is strongly rejected by the [Wald test](../../../statistical-modelling.md#wald-test), consistent with the sequential [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test). The fitted constant-over-age city [odds ratio](../../../statistical-modelling.md#odds-ratio) and an approximate 95% [confidence interval](../../../statistical-inference.md#confidence-interval) are

$$
\boxed{\operatorname{OR}=e^{0.85492}=2.351,\qquad \operatorname{CI}_{95\%}=e^{0.85492\pm1.96(0.05969)}\approx(2.09,2.64).}
$$

This is an odds ratio, not generally a probability ratio. The probabilities here are sufficiently small that the two ratios are close. The absence of an age-by-city [interaction](../../../statistical-model.md#interaction-statistics) is an assumption of the fitted additive log-odds model.

The final [binomial deviance](../../../statistical-modelling.md#binomial-deviance) is $5.1509$ on six [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom); its approximate upper-tail [p-value](../../../statistical-modelling.md#p-value) is $0.525$. It gives no indication of substantial lack of fit against the saturated observed-cell model. The [deviance residuals](../../../statistical-modelling.md#deviance-residual) range from $-1.2830$ to $1.0820$, with median zero and no conspicuously large value in the five-number summary. Neither statement proves that every model assumption holds. In particular, the small case counts motivate checking the accuracy of the [chi-squared asymptotic approximation](../../../probability-theory.md#chi-squared-asymptotic-approximation), for example by a fitted-model [parametric bootstrap](../../../statistical-modelling.md#parametric-bootstrap).

The dispersion is fixed at one by the [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution); it was not estimated as a free scale parameter. Four [Fisher scoring](../../../statistical-modelling.md#scoring-algorithm) iterations describe the numerical optimization, not four additional parameters. Residual and cellwise observed-versus-fitted comparisons would help assess adequacy and potential [overdispersion](../../../exponential-family.md#overdispersion).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The second analysis is an exposure-adjusted [Poisson regression](../../../statistical-modelling.md#poisson-regression) for case counts:

$$
\boxed{C_{gj}\sim\operatorname{Poisson}(\lambda_{gj}),\qquad\log\lambda_{gj}=\log N_{gj}+\alpha_P+a_{P,j}+\gamma_Pg,\qquad a_{P,15\text{–}24}=0.}
$$

Cell counts are independent, and their conditional [variance](../../../variance.md) equals their conditional mean. The population term is an [offset](../../../statistical-modelling.md#generalized-linear-model-offset) with coefficient fixed at one. Thus the fitted case rate is $\lambda_{gj}/N_{gj}=\exp(\alpha_P+a_{P,j}+\gamma_Pg)$; treating $\log N_{gj}$ as a free [covariate](../../../statistical-model.md#covariate) would fit a different model. Age multipliers and the adjusted city rate ratio are exponentials of the corresponding [regression coefficients](../../../linear-regression.md#regression-coefficient).

The fitted model again has nine parameters and six residual [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom). Sequential additions of age and city reduce the [Poisson deviance](../../../statistical-modelling.md#poisson-deviance) by $2095.56$ on seven [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom) and $226.52$ on one, respectively. The residual [deviance](../../../exponential-family.md#exponential-family-deviance) is $5.21$, close to the six residual [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom). The city [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test) is overwhelmingly significant, as in the binomial analysis. The table provides no Poisson coefficient estimates, so an exact Poisson city rate ratio cannot be read from it.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

For rare events, $\operatorname{Binomial}(N,\pi)$ is approximately $\operatorname{Poisson}(N\pi)$. The binomial [variance](../../../variance.md) is $N\pi(1-\pi)$, close to the Poisson [variance](../../../variance.md) $N\pi$, and $\log\{\pi/(1-\pi)\}$ is close to $\log\pi$. Even the largest observed proportion here is below $0.009$. Thus the binomial log-odds model and Poisson log-rate model should give similar fitted counts and tests, as their very similar deviances show.

**Both analyses indicate strong age and adjusted city associations, with no apparent large residual lack of fit.** The binomial model is natural when each person can contribute at most one case during a fixed period and the denominator counts people at risk. A Poisson count model is natural for event counts with an appropriate exposure or person-time denominator; population size is an approximation to such exposure if the observation periods are comparable. An [odds ratio](../../../statistical-modelling.md#odds-ratio) and a rate ratio are different parameters despite being close in this rare-event setting.

The models both assume a common city effect across ages. An age-by-city [interaction](../../../statistical-model.md#interaction-statistics) can be checked by comparing with the saturated model for the 15 observed cells, using the six additional [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom); the small final deviances offer no substantial evidence against the additive fits in that comparison. This cannot recover the missing city-by-age cell or eliminate unmeasured [confounding](../../../causal-inference.md#confounding). Nor is choosing the lower of $5.1509$ and $5.21$ a valid model-selection rule: these deviances are measured against saturated models for different response distributions.

## 5

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

[Survival data](../../../survival-analysis.md#survival-data) describe the time $T$ from a specified origin to an event, together with [covariates](../../../statistical-model.md#covariate) and information about how observation begins and ends. Some event times are observed exactly; others are subject to [censoring](../../../survival-analysis.md#censoring-statistics) or excluded by [truncation](../../../survival-analysis.md#truncation-statistics). Here the time origin is the opening of a business and the event is its closure. An observed record contains an entry age, an exit age, an event indicator and the business characteristics. **The time origin and observation mechanism are part of the data specification.**

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

With [right censoring](../../../survival-analysis.md#right-censoring), an event has not occurred by the last observation time $C$, so the data establish only $T>C$. One records $Y=\min(T,C)$ and $\delta=\mathbf1_{\{T\le C\}}$, distinguishing an observed event from a censored exit. A business still operating at the follow-up deadline is administratively right-censored. **Its observed age is a lower bound on its lifetime, not its eventual closure age.** Standard [survival analysis](../../../survival-analysis.md) requires suitable [independent censoring](../../../survival-analysis.md#independent-censoring), possibly conditional on the fitted [covariates](../../../statistical-model.md#covariate).

<h4 id="5/a/iii">iii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/a/iii)

With [left truncation](../../../survival-analysis.md#left-truncation), a subject is observed only if it survives to its entry time $E$: subjects with $T\le E$ are absent from the sample. A business already operating when observation begins has this delayed-entry mechanism. It joins a [risk set](../../../survival-analysis.md#risk-set) only after its recorded entry age. **Left truncation excludes earlier failures entirely; left censoring instead includes subjects whose event is known to have happened before a specified time.** These mechanisms must not be conflated.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

**Statistician B uses the more appropriate analysis.** Its start–stop representation includes [left truncation](../../../survival-analysis.md#left-truncation) as well as [right censoring](../../../survival-analysis.md#right-censoring). Both entry and exit are ages since opening, so a business belongs to the [risk set](../../../survival-analysis.md#risk-set) at age $t$ only when $\operatorname{ageatentry}<t\le\operatorname{obsage}$. The event indicator distinguishes closure from a censored end of observation. The counting-process representation does not mean that multiple closures per business have been observed.

Statistician A records only exit and status and treats every sampled business as at risk from opening. That incorrectly adds already-established businesses to [risk sets](../../../survival-analysis.md#risk-set) at ages before they entered observation, ignoring their necessary survival to entry. Its first risk count is $60$, whereas B's is $25$. The extra non-events dilute early estimated closure hazards and here bias the estimated survival upward. Correcting [left truncation](../../../survival-analysis.md#left-truncation) makes later [risk sets](../../../survival-analysis.md#risk-set) capable of increasing as businesses enter at their respective ages.

For the [Kaplan–Meier estimator with delayed entry](../../../survival-analysis.md#kaplan-meier-estimator-with-delayed-entry), at event ages $t_j$ with $d_j$ closures and $r_j$ businesses at risk,

$$
\widehat S(t)=\prod_{t_j\le t}\left(1-\frac{d_j}{r_j}\right),\qquad \widehat{\operatorname{se}}(\widehat S(t))=\widehat S(t)\left\{\sum_{t_j\le t}\frac{d_j}{r_j(r_j-d_j)}\right\}^{1/2}.
$$

The [standard error](../../../statistical-inference.md#standard-error) follows from the [Greenwood formula](../../../survival-analysis.md#greenwood-formula). Between event times this [survival function](../../../survival-analysis.md#survival-function) estimate is constant. At age five the last preceding event is at $4.52$, and at age ten it is at $9.90$. Thus the requested estimates, including their precision, are

$$
\boxed{\widehat S(5)=0.462,\quad\operatorname{se}=0.0780,\quad95\%\ \operatorname{CI}=(0.332,0.643),}
$$

and

$$
\boxed{\widehat S(10)=0.280,\quad\operatorname{se}=0.0634,\quad95\%\ \operatorname{CI}=(0.180,0.436).}
$$

These correspond to estimated proportions 46.2% and 28.0%, not to the probability of surviving five or ten additional years conditional on being sampled at an arbitrary age. A's corresponding estimates $0.650$ and $0.407$ use the inappropriate [risk sets](../../../survival-analysis.md#risk-set).

This interpretation assumes appropriately independent entry and censoring and a suitable common lifetime distribution across entry cohorts. A delayed-entry correction does not remove arbitrary informative sampling or calendar effects. More generally, if no observation covers the earliest ages, absolute survival from opening requires additional information about survival before the first observable age; the reported product-limit normalization is the one used in the supplied analysis.

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

Converting size to a [regression factor](../../../statistical-modelling.md#regression-factor) allows two unrestricted contrasts rather than imposing a linear trend on numerical size codes. The command relevel with a numeric second argument selects the second existing factor level as its [reference level](../../../statistical-modelling.md#reference-level-in-a-regression-factor). For sorted codes $0,1,2$ this is medium, coded $1$. However, the displayed coefficient labels size1 and size3 instead correspond to codes $1,2,3$ with code $2$ as reference. **The printed coding and coefficient labels are inconsistent.** The actual factor levels and labels must be checked. Under the intended medium-size reference, the two reported contrasts compare small and large businesses with medium ones; with literal $0,1,2$ coding their printed names would be size0 and size2.

Using B's delayed-entry survival object, the [Cox proportional-hazards model](../../../survival-analysis.md#cox-proportional-hazards-model) is

$$
h(t\mid c,s)=h_0(t)\exp\{\beta_c c+\beta_{\mathrm{small}}\mathbf1_{\{s=\mathrm{small}\}}+\beta_{\mathrm{large}}\mathbf1_{\{s=\mathrm{large}\}}\}.
$$

Here $h_0$ is the unspecified [baseline hazard](../../../survival-analysis.md#baseline-hazard) for a medium-size village business and $c$ is the Cambridge indicator. The fitted [hazard ratios](../../../survival-analysis.md#hazard-ratio) are conditional on the other [covariates](../../../statistical-model.md#covariate) and constant over business age under the [proportional hazards](../../../survival-analysis.md#proportional-hazards-model) assumption. The function fits [regression coefficients](../../../linear-regression.md#regression-coefficient) through [partial likelihood](../../../survival-analysis.md#partial-likelihood); its survival object must actually be B's version, rather than A's earlier object with the same name.

The location coefficient $-0.803$, with [standard error](../../../statistical-inference.md#standard-error) $0.344$, gives $z=-2.335$ and a two-sided [Wald test](../../../statistical-modelling.md#wald-test) [p-value](../../../statistical-modelling.md#p-value) about $0.02$. Its reported [hazard ratio](../../../survival-analysis.md#hazard-ratio) is $0.448$, with 95% [confidence interval](../../../statistical-inference.md#confidence-interval) $(0.228,0.879)$. At the same age and size, a Cambridge business therefore has an estimated closure hazard about 55.2% lower than a village business. The reciprocal ratio is $2.23$. **A hazard ratio is not a survival-probability ratio or a proportional increase in lifetime.**

The intended small-versus-medium contrast is $-0.322$, with [standard error](../../../statistical-inference.md#standard-error) $0.482$, $z=-0.669$ and [p-value](../../../statistical-modelling.md#p-value) $0.50$. Its [hazard ratio](../../../survival-analysis.md#hazard-ratio) is $0.724$, with 95% [confidence interval](../../../statistical-inference.md#confidence-interval) $(0.282,1.863)$. The intended large-versus-medium contrast is $-0.224$, with [standard error](../../../statistical-inference.md#standard-error) $0.375$, $z=-0.598$ and [p-value](../../../statistical-modelling.md#p-value) $0.55$; its [hazard ratio](../../../survival-analysis.md#hazard-ratio) is $0.799$, with interval $(0.383,1.666)$. Neither size contrast provides convincing evidence of an effect. The wide intervals also show why these results do not establish equality of size-specific hazards.

The sample has $60$ businesses. The [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test), [Wald test](../../../statistical-modelling.md#wald-test) and [score test](../../../statistical-modelling.md#score-test) jointly test all three coefficients being zero; their statistics are $5.45$, $5.76$ and $6.01$ on three [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom), with [p-values](../../../statistical-modelling.md#p-value) $0.142$, $0.124$ and $0.111$. None rejects at 5%. This is compatible with the significant one-coefficient location test: testing a specified one-dimensional contrast and testing three coefficients together are different questions. The location result offers some adjusted evidence, but the joint output does not demonstrate a strong overall improvement, and interpretation should acknowledge the uncertainty and the number of comparisons.

The reported $R^2=0.087$ is a [Cox–Snell likelihood pseudo-R-squared](../../../survival-analysis.md#cox-snell-likelihood-pseudo-r-squared), here $1-e^{-5.45/60}\approx0.087$. It measures likelihood improvement rather than a literal fraction of variance in lifetimes explained. Its attainable maximum is reported as $0.979$. It does not validate the [proportional hazards](../../../survival-analysis.md#proportional-hazards-model) assumption or establish useful predictive performance. Adjusted survival predictions would require estimating the [baseline survival function](../../../survival-analysis.md#baseline-survival-function) as well: $S(t\mid z)=S_0(t)^{e^{\beta^Tz}}$. The coefficient summary alone does not supply adjusted five- or ten-year survival probabilities.

Before reporting results, check the size coding discrepancy, the precise sampling dates and the survival records. The stated January 2000–December 2005 span is six calendar years, despite being called five years. Check nonnegative ages, entry no later than exit, correctly recorded closure indicators and the same opening-based clock throughout. Establish whether inclusion and [censoring](../../../survival-analysis.md#censoring-statistics) are plausibly independent of lifetime given the [covariates](../../../statistical-model.md#covariate), and whether different opening cohorts or calendar environments can reasonably share the fitted lifetime model. Simply including delayed entry does not cure informative selection, omitted [confounders](../../../causal-inference.md#confounder) or dependence between businesses.

Assess [proportional hazards](../../../survival-analysis.md#proportional-hazards-model) using [Schoenfeld residuals](../../../survival-analysis.md#schoenfeld-residual) against time and a [proportional hazards assumption test](../../../survival-analysis.md#proportional-hazards-assumption-test), supplemented by groupwise log-minus-log survival plots. Investigate influential observations with coefficient-deletion diagnostics and [deviance residuals](../../../statistical-modelling.md#deviance-residual), and inspect overall fit using [Cox–Snell residuals](../../../survival-analysis.md#cox-snell-residual). Consider a city-by-size [interaction](../../../statistical-model.md#interaction-statistics) or time-varying effects if supported by the available events, rather than relying on the displayed three main effects. Finally, report the uncertainty and declining late [risk sets](../../../survival-analysis.md#risk-set)—only six remain at the final listed event—and distinguish a conditional association from a causal explanation or a prediction for all future businesses.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
