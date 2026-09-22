# Paper 37

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper37.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper37.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
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
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [i](#5/b/i)
      - [Solution](#5/b/i/solution)
    - [ii](#5/b/ii)
      - [Solution](#5/b/ii/solution)
    - [iii](#5/b/iii)
      - [Solution](#5/b/iii/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)

## 1

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [least-squares estimator](../../../statistical-modelling.md#ordinary-least-squares-estimators) minimizes $(Y-Xb)^T(Y-Xb)$. Differentiation gives $X^TX\hat\beta=X^TY$, and the full column [rank](../../../linear-algebra.md#rank-one-quadratic-form) of $X$ makes $X^TX$ positive definite. Hence

$$
\boxed{\hat\beta=(X^TX)^{-1}X^TY.}
$$

The [fitted values](../../../linear-regression.md#fitted-values) are $\hat Y=X\hat\beta=HY$, where the [hat matrix](../../../statistical-modelling.md#hat-matrix) is $H=X(X^TX)^{-1}X^T$. The [regression residuals](../../../probability-and-statistics.md#regression-residual) are $\hat\varepsilon=Y-\hat Y=(I-H)Y$. Since $H$ is the [orthogonal projection matrix](../../../linear-algebra.md#orthogonal-projection-matrix) onto the column space of $X$, $(I-H)X=0$ and

$$
\boxed{\hat\varepsilon\sim N_n(0,\sigma^2(I-H)).}
$$

This is a singular [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution) supported on the $(n-p)$-dimensional orthogonal complement of the column space: its components are generally correlated. The equality $\hat Y=X\hat\beta$ puts the fitted vector in that column space, while $X^T\hat\varepsilon=0$ expresses [fitted-residual orthogonality](../../../statistical-modelling.md#fitted-residual-orthogonality). No residual component lies in an explanatory direction that could improve the least-squares fit.

For the calibration model, write $R_i$ for a reading and $a_i$ for the known amount. The first fit assumes $R_i=\alpha+\beta a_i+\varepsilon_i$ with independent $N(0,\sigma^2)$ errors. Its [residual-versus-fitted plot](../../../linear-regression.md#residual-versus-fitted-plot) has systematic changes in group means and an increasing within-group spread. These suggest both a nonlinear mean relationship and [heteroscedasticity](../../../statistical-modelling.md#heteroscedastic), rather than the random scatter expected from a satisfactory [normal linear model](../../../statistical-modelling.md#normal-linear-model).

The [Box–Cox transformation](../../../statistical-modelling.md#box-cox-transformation) plot is a profile [log-likelihood](../../../statistical-modelling.md#log-likelihood) for the power parameter $\lambda$. Its maximum is near $0.94$; the horizontal line gives an approximate 95% [likelihood-ratio confidence interval](../../../statistical-inference.md#likelihood-ratio-confidence-interval), which excludes the untransformed value $1$. Since affine rescaling of the response does not change the fitted mean space, fitting the raw power $R_i^{0.94}$ is equivalent to using $(R_i^{0.94}-1)/0.94$ with an intercept. The second model is

$$
R_i^{0.94}=\alpha+\beta a_i+\varepsilon_i,\qquad \varepsilon_i\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

Its residual spread is more even, but observation 17 has a conspicuously negative residual near $-9.95$. This motivates checking for an [outlier](../../../statistical-modelling.md#outlier) or recording error. The third fit omits that observation; omission should be justified by that investigation, since choosing exclusions from residuals can affect inference. Some group pattern still remains, so the transformation alone does not certify a perfect model.

At an amount of $3$ nanograms, the third fit predicts the transformed mean

$$
\hat m=-3.62509+30.87295(3)=88.99376.
$$

Simply applying the inverse power gives $\hat m^{1/0.94}=118.5187$. The requested expected reading needs [bias correction after an inverse transformation](../../../statistical-modelling.md#bias-correction-after-an-inverse-transformation), since $\mathbb E[g(Z)]\ne g(\mathbb E[Z])$ for nonlinear $g$. With $q=1/0.94$ and $s=2.832$, a second-order [Taylor expansion](../../../calculus.md#taylor-expansion) gives

$$
\boxed{\widehat{\mathbb E[R\mid a=3]}\simeq\hat m^q+\frac12q(q-1)\hat m^{q-2}s^2=118.5227.}
$$

Here the correction uses the residual variance, rather than the variance of the estimated fitted mean. The power-transformed Gaussian model is an approximation for positive readings; the fitted mean is over 31 residual standard deviations above zero, so the negative tail has negligible effect on this local approximation. The ordinary inverse-transformed prediction is therefore essentially $118.52$ at the displayed precision.

## 2

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The data do not cross every age with every gender: only age 21 has both genders, while age 30 has only women and age 40 only men. Thus a gender effect separate from age can be estimated under an additive model, but age-by-gender [interactions](../../../statistical-model.md#interaction-statistics) cannot all be estimated or checked. There is only one observation in each recorded combination of age, gender, policy, and points, so there is no within-cell replication for separating [pure error](../../../statistical-modelling.md#pure-error) from [lack of fit](../../../statistical-modelling.md#lack-of-fit). No sampling method or additional risk characteristics are supplied, limiting comparisons between policyholder categories.

There is also a source discrepancy: the printed table gives $268$ for one comprehensive premium, whereas the R data vector gives $368$ at the corresponding position. The supplied regression output is treated as referring to the R data. This should be resolved against the original data before substantive use.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $Y_{agpq}$ be the premium at age $a\in\{21,30,40\}$, gender $g\in\{F,M\}$, policy $p\in\{\mathrm{3rd},\mathrm{comp}\}$, and points $q\in\{0,3,6,9\}$, for the combinations actually observed. The additive [normal linear model](../../../statistical-modelling.md#normal-linear-model) is

$$
Y_{agpq}=\mu+\alpha_a+\gamma_g+\delta_p+\eta_q+\varepsilon_{agpq},\qquad \varepsilon_{agpq}\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

Its [corner-point constraints](../../../statistical-model.md#corner-point-constraint) are $\alpha_{21}=\gamma_F=\delta_{\mathrm{3rd}}=\eta_0=0$. Thus $\mu$ is the reference-category mean; the other coefficients are additive contrasts. The model assumes a common variance and excludes all [interactions](../../../statistical-model.md#interaction-statistics). It has $1+2+1+1+3=8$ estimable mean parameters and $32-8=24$ [residual degrees of freedom](../../../statistical-modelling.md#residual-degrees-of-freedom). The variance estimate is

$$
\boxed{\hat\sigma^2=19512/24=813.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The reduced model combines the 0-, 3-, and 6-point categories. Relative to the full model, the null hypothesis is $\eta_3=\eta_6=0$, leaving the 9-point contrast unrestricted. These are two linear restrictions on an otherwise unchanged [normal linear model](../../../statistical-modelling.md#normal-linear-model).

For nested normal models, the reduction in [residual sum of squares](../../../linear-regression.md#residual-sum-of-squares) divided by $\sigma^2$ has a [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) with degrees of freedom equal to the number of restrictions. It is independent of the full model's residual variance estimate. Hence the [F-test](../../../probability-and-statistics.md#f-test) statistic is

$$
F=\frac{(22323-19512)/2}{19512/24}=1.728782\sim F_{2,24}\quad\text{under }H_0.
$$

It is below the supplied 5% critical value $3.402826$, so **do not reject equal effects for 0, 3, and 6 points**. There is insufficient evidence that separating those categories improves this additive model; this does not prove that their true premiums are identical.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Let $h(q)=1$ for $q=0,3,6$ and $h(9)=2$. The new [normal linear model](../../../statistical-modelling.md#normal-linear-model) allows an age-by-policy [interaction](../../../statistical-model.md#interaction-statistics):

$$
Y_{agpq}=\mu+\alpha_a+\delta_p+\kappa_{ap}+\gamma_g+\xi_{h(q)}+\varepsilon_{agpq},\qquad \varepsilon_{agpq}\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

The [corner-point constraints](../../../statistical-model.md#corner-point-constraint) are $\alpha_{21}=\delta_{\mathrm{3rd}}=\gamma_F=\xi_1=0$ and $\kappa_{21,p}=\kappa_{a,\mathrm{3rd}}=0$. Compared with the six-parameter reduced additive model, there are two additional interaction coefficients. Its [F-test](../../../probability-and-statistics.md#f-test) gives

$$
\boxed{F=\frac{(22323-10028)/2}{10028/24}=14.7128,\qquad p\simeq6.75\times10^{-5}.}
$$

Thus the interaction model significantly improves the reduced additive model. Estimated premiums decrease with age. Men have an estimated premium $94.375$ higher than women at fixed other characteristics, and 9 points adds $41.708$ relative to 0, 3, or 6. Comprehensive cover costs more than third-party cover, but its increment depends on age: $175.375$ at 21, $148.500$ at 30, and $79.500$ at 40. These are model-based comparisons, including extrapolations into the unobserved age-gender combinations.

For a 40-year-old woman with comprehensive cover and 6 points, the gender and points contrasts vanish. The fitted premium is

$$
\boxed{269.760-207.812+175.375-95.875=141.448.}
$$

## 3

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution) probability mass function is

$$
\Pr(Y_i=y_i)=p_i^{y_i}(1-p_i)^{1-y_i}=\exp\left\{y_i\log\frac{p_i}{1-p_i}+\log(1-p_i)\right\}.
$$

Writing $\theta_i=\log[p_i/(1-p_i)]$ gives $p_i=e^{\theta_i}/(1+e^{\theta_i})$ and $\log(1-p_i)=-\log(1+e^{\theta_i})$. Therefore the [exponential family](../../../exponential-family.md) representation has

$$
\boxed{\theta_i=\operatorname{logit}(p_i)=\beta^Tx_i,\quad b(\theta)=\log(1+e^\theta),\quad\phi=1,\quad c(y,\phi)=0.}
$$

The [logit link](../../../statistical-modelling.md#logit) is the canonical link.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Independence gives the [log-likelihood](../../../statistical-modelling.md#log-likelihood)

$$
\ell(\beta)=\sum_i\left[y_i\beta^Tx_i-\log(1+e^{\beta^Tx_i})\right].
$$

Differentiating yields the [score equations](../../../statistical-modelling.md#score-equation)

$$
\boxed{\sum_i x_i\bigl[y_i-p_i(\hat\beta)\bigr]=0.}
$$

When a finite [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator) exists, multiplying these equations by $\hat\beta^T$ gives

$$
\sum_i y_i\operatorname{logit}p_i(\hat\beta)=\sum_i p_i(\hat\beta)\operatorname{logit}p_i(\hat\beta).
$$

The qualification about a finite estimator matters under [complete separation](../../../statistical-modelling.md#complete-separation) in [logistic regression](../../../statistical-modelling.md#logistic-regression), where coefficient estimates can escape to infinity.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For separate binary observations, the [saturated model](../../../foundations-of-mathematics.md#saturated-model) fits each outcome exactly and has maximized log-likelihood zero. With $\hat p_i=p_i(\hat\beta)$, the [residual deviance](../../../statistical-modelling.md#residual-deviance) is therefore

$$
D=-2\ell(\hat\beta)=-2\sum_i\left[y_i\operatorname{logit}\hat p_i+\log(1-\hat p_i)\right].
$$

Use the identity in part (b) to replace $y_i$ by $\hat p_i$ in its first term:

$$
\boxed{D=-2\sum_i\left[\hat p_i\operatorname{logit}\hat p_i+\log(1-\hat p_i)\right]=-2\sum_i\left[\hat p_i\log\hat p_i+(1-\hat p_i)\log(1-\hat p_i)\right].}
$$

Thus the deviance is twice the sum of the fitted binary [information entropies](../../../information-theory.md#information-entropy). A [deviance goodness-of-fit test](../../../statistical-modelling.md#deviance-goodness-of-fit-test) against $\chi^2_{n-p}$ is unreliable for individual ungrouped binary observations: there is only one trial per saturated-model parameter, so the usual large-cell-count approximation fails. Deviance differences between fixed-dimensional nested [logistic regression](../../../statistical-modelling.md#logistic-regression) models can still support a [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test), subject to its usual regularity assumptions.

The three tree models are respectively $\operatorname{logit}p_i=\beta_0$, $\operatorname{logit}p_i=\beta_0+\beta_1\log_2T_i$, and $\operatorname{logit}p_i=\beta_0+\beta_1\log_2T_i+\beta_2S_i$, with independent [Bernoulli random variables](../../../discrete-probability-distribution.md#bernoulli-distribution) conditional on the covariates. Testing the additional severity effect gives

$$
\boxed{2\{\ell(\widehat\beta_{\rm full})-\ell(\widehat\beta_{\rm reduced})\}=655.24-563.90=91.34.}
$$

Under $H_0:\beta_2=0$, its reference distribution is asymptotically $\chi^2_1$. The $p$-value is approximately $1.21\times10^{-21}$, giving overwhelming evidence that severity improves the fitted model. Holding severity fixed, doubling $T$ increases $\log_2T$ by one and multiplies the odds by

$$
\boxed{e^{2.2164}\simeq9.17.}
$$

This is an [odds ratio](../../../statistical-modelling.md#odds-ratio), not a multiplication of the event probability itself.

## 4

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The line compares the two pooled accident rates, dividing the total number of accidents by total observation years in each period. It gives the unadjusted [incidence rate ratio](../../../statistical-modelling.md#rate-ratio)

$$
\boxed{\frac{15/18}{114/68}=0.497076,}
$$

corresponding to an estimated reduction of about $50.3\%$. Pooling does not adjust for differences between locations or for the unequal location composition of observation time before and after installation.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $Y_{it}$ be the accident count at location $i$ in period $t\in\{0,1\}$, and $e_{it}$ its exposure in years, where $t=1$ denotes after installation. The [Poisson exposure model](../../../statistical-modelling.md#poisson-exposure-model) is

$$
Y_{it}\overset{\mathrm{ind}}\sim\operatorname{Poisson}(e_{it}e^{\alpha+\beta t}),\qquad\log\mathbb E[Y_{it}]=\log e_{it}+\alpha+\beta t.
$$

The [offset](../../../statistical-modelling.md#generalized-linear-model-offset) $\log e_{it}$ has its coefficient fixed at one. The model assumes constant rates within each period, a common before rate across locations, a common treatment rate ratio, independent counts, and Poisson variance equal to the mean. The [incidence rate ratio](../../../statistical-modelling.md#rate-ratio) is $r=e^\beta$, so

$$
\boxed{\hat r=e^{-0.69901}=0.497077.}
$$

An approximate 95% [Wald confidence interval](../../../statistical-inference.md#wald-confidence-interval) transforms the interval for $\beta$:

$$
\boxed{\left[e^{-0.69901-1.96(0.27466)},e^{-0.69901+1.96(0.27466)}\right]=[0.290,0.852].}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The second [Poisson exposure model](../../../statistical-modelling.md#poisson-exposure-model) allows each location its own baseline accident rate:

$$
Y_{it}\overset{\mathrm{ind}}\sim\operatorname{Poisson}(e_{it}e^{\alpha+\lambda_i+\beta t}),\qquad\lambda_1=0.
$$

The last equality is the [corner-point constraint](../../../statistical-model.md#corner-point-constraint). The common after-to-before [incidence rate ratio](../../../statistical-modelling.md#rate-ratio) remains $e^\beta$. This model is appropriate because the sites can have different background risks; treating those differences as unexplained Poisson variation made the first model fit poorly, with deviance $50.863$ on 14 [residual degrees of freedom](../../../statistical-modelling.md#residual-degrees-of-freedom).

Adding seven location effects to the first fitted model reduces the deviance by $50.863-16.275=34.588$, which is large relative to $\chi^2_7$. The supplied sequential [analysis of deviance](../../../statistical-modelling.md#analysis-of-deviance-for-nested-generalized-linear-models) reports a slightly different location contribution because it enters locations before the period indicator. The full model is much better but its deviance $16.275$ on 7 degrees of freedom still gives an approximate goodness-of-fit $p$-value $0.0227$. That suggests residual lack of fit or [overdispersion](../../../exponential-family.md#overdispersion), although sparse accident counts make the asymptotic [deviance goodness-of-fit test](../../../statistical-modelling.md#deviance-goodness-of-fit-test) approximate.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

After adjusting for location, adding the period effect reduces deviance by $9.750$ on one degree of freedom, giving the supplied [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test) $p\simeq0.002$. The adjusted [incidence rate ratio](../../../statistical-modelling.md#rate-ratio) is

$$
\boxed{e^{-0.7807}=0.4581,\qquad 95\%\text{ Wald interval }[e^{-0.7807-1.96(0.2754)},e^{-0.7807+1.96(0.2754)}]=[0.267,0.786].}
$$

Under this [Poisson exposure model](../../../statistical-modelling.md#poisson-exposure-model), the accident rate after installation is estimated to be about $54.2\%$ lower, with a statistically significant reduction. The remaining lack of fit merits residual checks and possibly a [Quasi-Poisson model](../../../statistical-modelling.md#quasi-poisson-regression) or a model allowing location-specific changes. This before-and-after observational study establishes an association under the fitted model; changes in traffic volume, broader trends, or [regression to the mean](../../../statistical-modelling.md#regression-to-the-mean) at sites chosen for high prior counts could also contribute, so the estimated reduction is not by itself a causal treatment effect.

## 5

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Let $I\in\{1,2\}$ denote eventual death or recovery, respectively; $T$ is the time from admission to that terminal event, and $\theta=\Pr(I=1)$. A patient still hospitalized at collection has [right censoring](../../../survival-analysis.md#right-censoring): only $T>c$ is known, where $c$ is the elapsed time since admission. Both eventual outcomes are then unobserved. A recorded death or discharge is an observed terminal event in this [competing risks model](../../../survival-analysis.md#competing-risks-model); discharge is not censoring of an otherwise observable later in-hospital death. Assume the observation deadline, conditional on relevant admission information, is noninformative for $(T,I)$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

Let $f_j(t)=f(t\mid I=j)$ and $S_j(t)=1-F(t\mid I=j)$. A recorded death observes both $T=t$ and $I=1$, so its [likelihood](../../../statistical-modelling.md#likelihood-function) contribution, omitting factors from the independent observation mechanism, is

$$
\boxed{\theta f_1(t).}
$$

Its integration over $t$ gives the eventual death probability $\theta$.

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

A recorded discharge observes $T=t$ and $I=2$. Its [likelihood](../../../statistical-modelling.md#likelihood-function) contribution is

$$
\boxed{(1-\theta)f_2(t).}
$$

The mixing probability distinguishes the joint outcome-and-time density from the conditional recovery-time density.

<h4 id="5/b/iii">iii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/b/iii)

For a patient still in hospital, sum over the unobserved eventual outcome. Its [likelihood](../../../statistical-modelling.md#likelihood-function) contribution is the mixture [survival function](../../../survival-analysis.md#survival-function)

$$
\boxed{\Pr(T>c)=\theta S_1(c)+(1-\theta)S_2(c).}
$$

The probability of eventual death among those still hospitalized is generally different from $\theta$, because the two conditional time distributions can have different tails.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

This is an [EM algorithm for a censored lognormal competing-risks mixture](../../../survival-analysis.md#em-algorithm-for-a-censored-lognormal-competing-risks-mixture). Write $Y_i=\log T_i$ and suppose $Y_i\mid I_i=j\sim N(\mu_j,\sigma_j^2)$, with mixing weights $\pi_1=\theta$, $\pi_2=1-\theta$. The missing data are $I_i$ and $Y_i$ for censored patients; neither is missing for recorded deaths or recoveries. The complete-data [log-likelihood](../../../statistical-modelling.md#log-likelihood), apart from terms independent of the parameters, is

$$
\ell_c=\sum_i\sum_{j=1}^2\mathbf1_{\{I_i=j\}}\left[\log\pi_j-\log\sigma_j-\frac{(Y_i-\mu_j)^2}{2\sigma_j^2}\right].
$$

The lognormal Jacobian $-\log T_i$ is also parameter-independent and therefore does not affect the maximization.

At iteration $k$, set $z_{ij}=(\log c_i-\mu_j^{(k)})/\sigma_j^{(k)}$ for each censored patient and let $\overline\Phi(z)=1-\Phi(z)$. Bayes' rule gives the E-step class weights

$$
\boxed{w_{ij}=\frac{\pi_j^{(k)}\overline\Phi(z_{ij})}{\sum_{\ell=1}^2\pi_\ell^{(k)}\overline\Phi(z_{i\ell})}.}
$$

Given that class, $Y_i$ has a [truncated normal distribution](../../../probability-theory.md#truncated-normal-distribution) above $\log c_i$. With the [Inverse Mills ratio](../../../probability-theory.md#inverse-mills-ratio) $\psi(z)=\varphi(z)/\overline\Phi(z)$, compute both moments needed for the E-step:

$$
\begin{aligned}
m_{ij}&=\mu_j^{(k)}+\sigma_j^{(k)}\psi(z_{ij}),\\
v_{ij}&=(\sigma_j^{(k)})^2\left[1-\psi(z_{ij})\bigl(\psi(z_{ij})-z_{ij}\bigr)\right],\\
s_{ij}&=m_{ij}^2+v_{ij}.
\end{aligned}
$$

Thus $\mathbb E[\mathbf1_{\{I_i=j\}}\mid\text{data}]=w_{ij}$, $\mathbb E[\mathbf1_{\{I_i=j\}}Y_i\mid\text{data}]=w_{ij}m_{ij}$, and the corresponding second moment is $w_{ij}s_{ij}$. For an observed outcome $j_i$ at time $t_i$, use $w_{ij}=\mathbf1_{\{j=j_i\}}$, $m_{ij}=\log t_i$, and $s_{ij}=(\log t_i)^2$. These specify the full conditional expectation of $\ell_c$.

Put $W_j=\sum_iw_{ij}$ and let $n$ be the total number of patients. Maximizing that expected complete-data log-likelihood gives the M-step

$$
\boxed{\begin{aligned}
\theta^{(k+1)}&=W_1/n,\\
\mu_j^{(k+1)}&=\frac{\sum_iw_{ij}m_{ij}}{W_j},\\
(\sigma_j^2)^{(k+1)}&=\frac{\sum_iw_{ij}s_{ij}}{W_j}-\bigl(\mu_j^{(k+1)}\bigr)^2.
\end{aligned}}
$$

All moments on the right are evaluated at the old parameters. Repeat the E-step and M-step until the observed [log-likelihood](../../../statistical-modelling.md#log-likelihood) stabilizes, using positive initial variances and mixing weights. The [expectation-maximization algorithm](../../../statistical-modelling.md#expectation-maximization-algorithm) increases that likelihood at each exact iteration, but need not find its global maximum; multiple starts help distinguish local optima. The resulting estimates give the case fatality probability $\hat\theta$ and

$$
\boxed{\widehat F(t\mid I=j)=\Phi\left(\frac{\log t-\hat\mu_j}{\hat\sigma_j}\right),\qquad t>0.}
$$

These are conditional event-time distributions, distinct from the [cumulative incidence functions](../../../survival-analysis.md#cumulative-incidence-function) $\hat\theta\widehat F(t\mid I=1)$ and $(1-\hat\theta)\widehat F(t\mid I=2)$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
