# Paper 218

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_218.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_218.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
  - [f](#1/f)
    - [Solution](#1/f/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [i](#2/d/i)
      - [Solution](#2/d/i/solution)
    - [ii](#2/d/ii)
      - [Solution](#2/d/ii/solution)
    - [iii](#2/d/iii)
      - [Solution](#2/d/iii/solution)
    - [iv](#2/d/iv)
      - [Solution](#2/d/iv/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
  - [f](#3/f)
    - [Solution](#3/f/solution)
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
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
  - [e](#5/e)
    - [Solution](#5/e/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [i](#6/c/i)
      - [Solution](#6/c/i/solution)
    - [ii](#6/c/ii)
      - [Solution](#6/c/ii/solution)
    - [iii](#6/c/iii)
      - [Solution](#6/c/iii/solution)

## 1

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For individual $i$, let $Y_i$ be the reported count, $g_i\in\{0,1\}$ the gender indicator, and $m_i\in\{0,1\}$ the minority indicator. The fitted [Poisson regression](../../../statistical-modelling.md#poisson-regression) is

$$
Y_i\mathrel{\perp\!\!\!\perp}Y_j,
\qquad
Y_i\sim\operatorname{Poisson}(\mu_i),
\qquad
\log\mu_i=\beta_0+\beta_1g_i+\beta_2m_i.
$$

Its [log-likelihood](../../../statistical-modelling.md#log-likelihood) is

$$
\ell(\beta)=\sum_{i=1}^{1308}
\{Y_i x_i^T\beta-e^{x_i^T\beta}-\log(Y_i!)\},
\qquad x_i=(1,g_i,m_i)^T.
$$

The [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator) is

$$
(\widehat\beta_0,\widehat\beta_1,\widehat\beta_2)
=(-2.2959,-0.1916,1.7293).
$$

Holding minority status fixed, changing the gender indicator from zero to one multiplies the fitted [conditional expected value](../../../measure-theory.md#conditional-expectation) by $e^{-0.1916}=0.826$. Thus the fitted mean count for men is about $17.4\%$ lower than that for women with the same minority status.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The researcher computed the [Pearson chi-squared statistic](../../../statistical-modelling.md#pearson-chi-squared-statistic)

$$
X_P^2=\sum_i\frac{(Y_i-\widehat\mu_i)^2}{\widehat\mu_i}
$$

and compared it with a $\chi^2_{1305}$ distribution, using $1308-3=1305$ [residual degrees of freedom](../../../statistical-modelling.md#residual-degrees-of-freedom). Under an adequate large-sample [Poisson regression](../../../statistical-modelling.md#poisson-regression), $X_P^2$ should be roughly the residual degrees of freedom. The reported tail probability rounds numerically to zero and gives strong evidence of [overdispersion](../../../exponential-family.md#overdispersion).

Possible causes include unobserved heterogeneity or omitted covariates, dependence among respondents, excess zeros, or an incorrect mean function. The conclusion that the Poisson variance assumption fails is well supported, although this test alone does not identify the cause or establish that the [Quasi-Poisson regression](../../../statistical-modelling.md#quasi-poisson-regression) variance $\operatorname{Var}(Y_i)=\phi\mu_i$ is correct.

The reported [Pearson dispersion estimator](../../../statistical-modelling.md#pearson-dispersion-estimator) is $\widehat\phi=X_P^2/1305=1.719346$, so

$$
X_P^2=1305(1.719346)=2243.75
$$

up to rounding.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

With $X$ having rows $x_i^T=(1,g_i,m_i)$ and $\mu_i(\beta)=e^{x_i^T\beta}$, the [quasi-score equation](../../../statistical-modelling.md#quasi-score-equation) is

$$
X^T\{Y-\mu(\beta)\}=0.
$$

It is the same coefficient equation as for Poisson maximum likelihood, explaining why the two models have identical coefficient estimates.

Let $W=\operatorname{diag}(\widehat\mu_1,\ldots,\widehat\mu_n)$ and let coordinate $2$ denote gender. The model-based [standard error](../../../statistical-inference.md#standard-error) is

$$
\boxed{\operatorname{se}(\widehat\beta_1)
=\sqrt{\widehat\phi\,[(X^TWX)^{-1}]_{22}},
\qquad
\widehat\phi=\frac{X_P^2}{n-3}.}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The Quasi-Poisson standard errors are trustworthy only if observations are independent, the log-linear mean is correct, and the variance is proportional to the mean with one common dispersion. Dependence, zero inflation, or covariate-dependent dispersion can invalidate this covariance formula.

A [parametric bootstrap](../../../statistical-modelling.md#parametric-bootstrap) under model 1 proceeds as follows. Fit the Poisson model once and retain $X$ and the fitted means $\widehat\mu_i$. For bootstrap repetition $b$, independently draw

$$
Y_i^{*(b)}\sim\operatorname{Poisson}(\widehat\mu_i),
$$

refit the same Poisson regression to $(X,Y^{*(b)})$, and save its gender estimate $\widehat\beta_1^{*(b)}$. The sample standard deviation of these estimates over many repetitions estimates the model-1 standard error. This bootstrap deliberately measures uncertainty under the fitted Poisson model; it does not repair real overdispersion unless the resampling model is enlarged to represent its cause.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The [generalized linear mixed model](../../../statistical-modelling.md#generalized-linear-mixed-model) tries to explain overdispersion by replacing the fixed minority coefficient with a Gaussian [random intercept](../../../statistical-modelling.md#random-intercept). Conditional on the group effect $b_m$,

$$
Y_i\sim\operatorname{Poisson}(\mu_i),
\qquad
\log\mu_i=\beta_0+\beta_1g_i+b_{m_i},
\qquad b_0,b_1\sim N(0,\tau^2).
$$

This is a poor use of a random effect because minority has only two levels. Two realized intercepts contain almost no information about a random-effects distribution or its variance, and the two levels are substantively fixed categories rather than a sample from a population of groups. The model also has worse [Akaike information criterion](../../../statistical-modelling.md#akaike-information-criterion) than model 1, $1132.8>1122.3$, and its fit does not establish that the original overdispersion has disappeared.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

Because models 1 and 3 are full likelihood models for the same response, one can compare their [Akaike information criterion](../../../statistical-modelling.md#akaike-information-criterion) values; that favors model 1. One can also compare held-out count prediction by [K-fold cross-validation](../../../statistical-learning.md#k-fold-cross-validation), using a common loss such as Poisson deviance or negative log predictive density.

The AIC comparison cannot include model 2 because a Quasi-Poisson fit specifies only mean and variance and has no full likelihood. Cross-validation can compare model 2 with model 3 if all predictions are scored by the same proper out-of-sample loss.

## 2

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A process $(X_t)_{t\in\mathbb Z}$ is [weakly stationary](../../../time-series.md#weakly-stationary-process) when it has finite second moments, a time-independent mean $\mathbb E X_t=\mu$, and an [autocovariance function](../../../time-series.md#autocovariance)

$$
\operatorname{Cov}(X_t,X_s)=\gamma(t-s)
$$

that depends only on the lag.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

At lag $h$, the plot shows the [sample autocorrelation function](../../../time-series.md#sample-autocorrelation-function)

$$
\widehat\rho(h)=
\frac{\sum_{t=h+1}^n(X_t-\overline X)(X_{t-h}-\overline X)}
{\sum_{t=1}^n(X_t-\overline X)^2}.
$$

Under a [white noise process](../../../time-series.md#white-noise), each fixed nonzero-lag sample autocorrelation is approximately $N(0,1/n)$, so the dashed pointwise $95\%$ reference lines are approximately $\pm1.96/\sqrt n$.

The first nonzero-lag bar is well above the upper line, which contradicts the zero autocorrelation expected from white noise. Since the plot then largely cuts off, an [moving-average process of order one](../../../time-series.md#moving-average-process-of-order-one) is a plausible model; with the sampling interval as the time unit this is an $\operatorname{ARMA}(0,1)$ model.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The selected zero-mean [autoregressive moving-average process](../../../time-series.md#autoregressive-moving-average-model) is

$$
X_t=\phi X_{t-1}+\varepsilon_t+\theta\varepsilon_{t-1},
\qquad
\varepsilon_t\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

The reported [maximum-likelihood estimates](../../../statistical-modelling.md#maximum-likelihood-estimator) are

$$
\widehat\phi=0.6997,
\qquad \widehat\theta=0.9510,
\qquad \widehat\sigma^2=0.4944.
$$

Using the displayed asymptotic standard error gives the [Wald confidence interval](../../../statistical-inference.md#wald-confidence-interval)

$$
0.9510\pm1.96(0.3287)=[0.307,1.595].
$$

This normal interval is unreliable and likely too narrow because the series has only about twenty observations, the moving-average estimate is near the noninvertibility boundary $\theta=1$, and the same data were used to select the model. The finite-sample likelihood is consequently skewed and model-selection uncertainty is omitted.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/i">i</h4>

↑ **Parent:** [D](#2/d)

<h5 id="2/d/i/solution">Solution</h5>

↑ **Parent:** [I](#2/d/i)

The [autoregressive process of order one](../../../time-series.md#autoregressive-process-of-order-one) is causal exactly when

$$
|\phi|<1,
$$

because then $X_t=\sum_{j\geq0}\phi^j\varepsilon_{t-j}$ converges in mean square. Its autocovariance is

$$
\boxed{\gamma_X(h)=\frac{\sigma^2}{1-\phi^2}\phi^{|h|},
\qquad h\in\mathbb Z.}
$$

<h4 id="2/d/ii">ii</h4>

↑ **Parent:** [D](#2/d)

<h5 id="2/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/d/ii)

Under the intended assumption that the two white-noise sequences are mutually uncorrelated at every pair of times, $X$ and $W$ are uncorrelated. Their sum is therefore weakly stationary with

$$
\mathbb EY_t=0,
\qquad
\gamma_Y(h)=
\frac{\sigma^2}{1-\phi^2}\phi^{|h|}
+\sigma_W^2\mathbf1_{\{h=0\}}.
$$

Strictly, the printed condition $\mathbb E[\varepsilon_tW_t]=0$ only at equal times is insufficient. For example, $W_t=(-1)^t\varepsilon_{t-1}$ is itself white noise and is contemporaneously uncorrelated with $\varepsilon_t$, but the cross-covariance contribution can depend on $t$. The displayed answer therefore uses the standard intended cross-series white-noise assumption $\mathbb E[\varepsilon_tW_s]=0$ for all $s,t$.

<h4 id="2/d/iii">iii</h4>

↑ **Parent:** [D](#2/d)

<h5 id="2/d/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/d/iii)

Using $X_t-\phi X_{t-1}=\varepsilon_t$ gives

$$
U_t=Y_t-\phi Y_{t-1}
=\varepsilon_t+W_t-\phi W_{t-1}.
$$

Under the cross-series uncorrelatedness used in part ii, terms in $U_t$ and $U_{t-h}$ involve disjoint white-noise times whenever $|h|>1$. Hence

$$
\gamma_U(h)=0\qquad(|h|>1).
$$

For completeness,

$$
\gamma_U(0)=\sigma^2+(1+\phi^2)\sigma_W^2,
\qquad
\gamma_U(1)=-\phi\sigma_W^2.
$$

<h4 id="2/d/iv">iv</h4>

↑ **Parent:** [D](#2/d)

<h5 id="2/d/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/d/iv)

Part iii and the stated characterization imply that $U$ has a [moving-average process of order one](../../../time-series.md#moving-average-process-of-order-one) representation $U_t=\eta_t+\theta\eta_{t-1}$. Since

$$
(1-\phi B)Y_t=U_t,
$$

where $B$ is the [backshift operator](../../../time-series.md#backshift-operator),

$$
(1-\phi B)Y_t=(1+\theta B)\eta_t.
$$

**Thus $Y$ is a causal [autoregressive moving-average process](../../../time-series.md#autoregressive-moving-average-model) of order $(1,1)$.**

## 3

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $T_i>0$ be record time and let $x_i=(1,c_i,d_i)^T$ contain standardized climb and distance. Model 1 is the [normal linear model](../../../statistical-modelling.md#normal-linear-model)

$$
T_i=x_i^T\beta+\varepsilon_i,
\qquad \varepsilon_i\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

Model 2 applies the same model after a [logarithmic transformation](../../../statistical-modelling.md#logarithmic-transformation):

$$
\log T_i=x_i^T\alpha+e_i,
\qquad e_i\overset{\mathrm{iid}}\sim N(0,\tau^2),
$$

so $T_i$ is conditionally log-normal. Model 3 is a [Gamma regression with logarithmic link](../../../statistical-modelling.md#gamma-regression-with-logarithmic-link):

$$
\boxed{\mathbb E(T_i\mid x_i)=\mu_i,
\qquad
\operatorname{Var}(T_i\mid x_i)=\phi\mu_i^2,
\qquad
\log\mu_i=x_i^T\gamma.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Model 1's residuals have a systematic curved pattern and a spread that grows strongly with fitted time. This indicates an incorrect linear mean on the original scale and [heteroscedasticity](../../../statistical-modelling.md#heteroscedastic); several observations are also influential or outlying. The constant-variance assumption is therefore implausible.

Logging time greatly stabilizes the spread and removes most of the mean pattern, so model 2 is much more compatible with constant conditional variance and linearity. A few conspicuous residuals remain. A residual-versus-fitted plot alone does not check [independence](../../../random-variable.md#independent-random-variables) or fully establish [normality](../../../probability-theory.md#normal-distribution).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For a likelihood $L(\theta)$ with $k$ estimated parameters, the [Akaike information criterion](../../../statistical-modelling.md#akaike-information-criterion) is

$$
\operatorname{AIC}=-2\log L(\widehat\theta)+2k,
$$

where $\widehat\theta$ is the [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator). Among likelihoods for the same observed response and reference measure, smaller AIC estimates smaller expected out-of-sample [Kullback-Leibler divergence](../../../probability-and-statistics.md#kullback-leibler-divergence) up to a model-independent constant.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The printed values appear to favor model 2 because $-12.529<336.381$. They are not directly comparable: model 2 reports the Gaussian likelihood of $Z_i=\log T_i$, whereas model 3 reports a density for $T_i$. The [change-of-variables formula for a probability density](../../../continuous-probability-distribution.md#change-of-variables-formula-for-a-probability-density) gives

$$
\ell_T=\ell_Z-\sum_{i=1}^{35}\log T_i,
$$

so the transformed model's AIC on the original response scale is

$$
\operatorname{AIC}_{2,T}
=\operatorname{AIC}_{2,Z}+2\sum_i\log T_i.
$$

Because the standardized predictors have zero sample means and the ordinary-least-squares residuals sum to zero,

$$
\sum_i\log T_i=35\widehat\alpha_0=35(4.99902).
$$

Therefore

$$
\operatorname{AIC}_{2,T}
=-12.52943+70(4.99902)=337.402,
$$

which is slightly worse than model 3's $336.381$.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares) equations for model 2 are

$$
X^T(\log T-X\widehat\alpha)=0.
$$

For the Gamma [generalized linear model](../../../statistical-modelling.md#generalized-linear-model), $V(\mu)=\mu^2$ and $d\mu/d\eta=\mu$, so its score equation under the logarithmic link is

$$
X^T\left(\frac{T}{\mu}-\mathbf1\right)=0,
\qquad \mu_i=e^{x_i^T\widehat\gamma}.
$$

When $T_i$ is close to $\mu_i$,

$$
\frac{T_i}{\mu_i}-1
=e^{\log T_i-\log\mu_i}-1
\simeq\log T_i-x_i^T\widehat\gamma
$$

by the first-order [Taylor expansion](../../../calculus.md#taylor-expansion) of the exponential function. The Gamma score equations then become the model-2 normal equations, so their coefficient estimates are close.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

Model 3 directly specifies the conditional mean and variance of the positive response on its observed scale. Its coefficients give multiplicative effects on mean record time, its prediction intervals concern time itself, and its likelihood can be compared directly with other original-scale models.

Model 2 instead models the mean of $\log T$. Back-transformation does not give the mean time without a [retransformation bias](../../../statistical-modelling.md#retransformation-bias) correction; for a log-normal model, $\mathbb E(T\mid x)=\exp(x^T\alpha+\tau^2/2)$. The Gamma model also represents the increasing original-scale variance seen in the diagnostic plot, so it is preferable here.

## 4

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

With $f=\mathbf1_{\{\mathrm{font}=\mathrm{serif}\}}$ and $d=\mathbf1_{\{\mathrm{display}=\mathrm{popup}\}}$, the model-matrix input is

$$
x=(f,d,fd)^T\in\mathbb R^3.
$$

The [feedforward neural network](../../../statistical-learning.md#feedforward-neural-network) has three inputs, a fully connected layer of two [ReLU](../../../statistical-learning.md#rectified-linear-unit) units, and a fully connected two-class [softmax](../../../statistical-learning.md#softmax-function) output. Algebraically,

$$
h=\operatorname{ReLU}(Wx+b),
\qquad
z=Vh+c,
\qquad
p_k=\frac{e^{z_k}}{e^{z_0}+e^{z_1}},
$$

where $W\in\mathbb R^{2\times3}$, $b\in\mathbb R^2$, $V\in\mathbb R^{2\times2}$, and $c\in\mathbb R^2$. The coding is $0$ for no click and $1$ for a click. There are

$$
2(3)+2+2(2)+2=14
$$

parameters.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The fitted classifier is

$$
\widehat C(x)=\operatorname*{argmax}_{k\in\{0,1\}}\widehat p_k(x),
$$

and training minimizes the empirical [categorical cross-entropy loss](../../../statistical-learning.md#categorical-cross-entropy-loss)

$$
-\sum_i\sum_{k=0}^1y_{ik}\log p_{ik}.
$$

The [softmax non-identifiability](../../../statistical-learning.md#softmax-non-identifiability) already proves that the coefficient vector is not unique. For any $a\in\mathbb R^2$ and $r\in\mathbb R$, replace both rows of $V$ by $V_{k\cdot}+a^T$ and both output biases by $c_k+r$. Every logit then gains the same value $a^Th+r$, so all softmax probabilities, classifications, and losses remain unchanged. Permuting the two hidden units supplies another non-uniqueness.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For the one-layer softmax fit, write its class logits as $z_k=a_k+b_k^Tx$. Then

$$
\log\frac{p_1(x)}{p_0(x)}
=(a_1-a_0)+(b_1-b_0)^Tx.
$$

Thus an equivalent [logistic regression](../../../statistical-modelling.md#logistic-regression) classifier predicts a click exactly when

$$
\delta_0+\delta^Tx\geq0,
\qquad
\delta_0=a_1-a_0,
\quad \delta=b_1-b_0.
$$

Using one reference class removes the common-logit-shift non-identifiability. Subject to the usual full-rank and no-separation conditions, the logistic parameter is identifiable. It uses four effective parameters rather than an eight-parameter redundant softmax representation, has a convex loss, and gives directly interpretable log-odds coefficients, so it is preferable for this binary linear classifier.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The first observation has $x=(1,0,0)^T$ and one-hot label $y=(0,1)^T$ in the output order $(\mathrm{no},\mathrm{yes})$. If every kernel weight and bias initially equals one, each hidden preactivation is two, so $h=(2,2)^T$. Both logits equal five and $p=(1/2,1/2)^T$.

For [stochastic gradient descent](../../../numerical-analysis.md#stochastic-gradient-descent) on one cross-entropy observation,

$$
\frac{\partial L}{\partial z}=p-y=(1/2,-1/2)^T.
$$

Hence the output-weight gradient has first row $(1,1)$ and second row $(-1,-1)$, while the output-bias gradient is $(1/2,-1/2)$. With learning rate one,

$$
V^{\mathrm{new}}=
\begin{pmatrix}0&0\\2&2\end{pmatrix},
\qquad
c^{\mathrm{new}}=(1/2,3/2)^T.
$$

Using the old output weights for backpropagation gives

$$
V^T(p-y)=(0,0)^T,
$$

so every entry of $W$ and $b$ remains equal to one after this batch.

## 5

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For fixed $\lambda_2$, letting $\lambda_1\downarrow0$ gives [ridge regression](../../../linear-regression.md#ridge-regression), including ordinary least squares when $\lambda_2=0$; letting $\lambda_1\to\infty$ forces every coefficient to zero. For fixed $\lambda_1$, letting $\lambda_2\downarrow0$ gives the [Lasso](../../../probability-and-statistics.md#lasso). Letting both penalties vanish gives an [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares) solution, unique when $X$ has full column rank and otherwise potentially nonunique or path-dependent.

When $\lambda_2>0$, the term $\lambda_2\lVert\beta\rVert_2^2$ is strictly convex. Its sum with the convex squared loss and $\ell^1$ penalty is strictly convex and coercive, so the [elastic net](../../../probability-and-statistics.md#elastic-net-regularization) solution exists and is unique.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For coordinate $j$, hold all other coefficients fixed and form the partial residual

$$
r_j=Y-\sum_{k\ne j}x_k\beta_k.
$$

The one-coordinate [coordinate descent](../../../convex-optimization.md#coordinate-descent) problem is

$$
\min_b\ \lVert r_j-x_jb\rVert^2+\lambda_1|b|+\lambda_2b^2.
$$

Its exact update is

$$
\beta_j\leftarrow
\frac{S_{\lambda_1}(x_j^Tr_j)}{\lVert x_j\rVert^2+\lambda_2},
\qquad
S_\lambda(u)=\operatorname{sgn}(u)(|u|-\lambda/2)_+.
$$

Cyclically update coordinates and their residuals until the objective or coefficients converge. Convexity makes every limit point a global minimizer, and $\lambda_2>0$ makes it the unique minimizer.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

When $X^TX=I_p$, expanding the objective separates it by coordinates:

$$
\lVert Y\rVert^2+
\sum_{j=1}^p\{(1+\lambda_2)\beta_j^2
-2(X^TY)_j\beta_j+\lambda_1|\beta_j|\}.
$$

The [soft thresholding](../../../probability-and-statistics.md#soft-thresholding) solution is therefore

$$
\boxed{\widehat\beta_j^E
=\frac{S_{\lambda_1}((X^TY)_j)}{1+\lambda_2},
\qquad j=1,\ldots,p.}
$$

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Model m1 is [ridge regression](../../../linear-regression.md#ridge-regression), while m2 is the [Lasso](../../../probability-and-statistics.md#lasso). Ridge shrinks but normally retains every coefficient; the Lasso's $\ell^1$ penalty sets many coefficients exactly to zero. Model m3 combines sparsity with the [grouping effect of the elastic net](../../../probability-and-statistics.md#grouping-effect-of-the-elastic-net): correlated predictors tend to enter together and receive more similar coefficients.

Accordingly, m3 keeps the weak variables age, lcp, and gleason at zero as m2 does, but retains lweight, lbph, svi, and pgg45 as the ridge fit does. The correlation $0.54$ between svi and lcavol explains why m3 keeps both with substantial coefficients, whereas m2 selects lcavol and discards svi. This lies between the dense ridge behavior and the more aggressively sparse Lasso behavior.

<h3 id="5/e">e</h3>

↑ **Parent:** [5](#5)

<h4 id="5/e/solution">Solution</h4>

↑ **Parent:** [E](#5/e)

Choose $(\lambda_1,\lambda_2)$ on a grid by [K-fold cross-validation](../../../statistical-learning.md#k-fold-cross-validation), comparing the same held-out prediction loss and optionally applying the one-standard-error rule for a simpler model. A genuinely untouched [test set](../../../statistical-learning.md#test-set) can then estimate final prediction error.

Ordinary model-based intervals after selecting nonzero coefficients ignore selection and are generally invalid. Valid approaches include [Debiased Lasso](../../../probability-and-statistics.md#debiased-lasso) or a selective-inference procedure under its assumptions, sample splitting followed by an unpenalized refit and inference on the independent half, or a bootstrap that repeats both tuning and fitting and is interpreted with care near the nonsmooth zero threshold.

## 6

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

The binary [regression functions](../../../statistical-learning.md#regression-function) are the [conditional class probabilities](../../../statistical-learning.md#conditional-class-probability)

$$
\eta_1(x)=\mathbb P(Y=1\mid X=x)=\mathbb E(Y\mid X=x),
\qquad
\eta_0(x)=1-\eta_1(x).
$$

Under zero-one loss, the [Bayes classifier](../../../statistical-inference.md#bayes-classifier) is

$$
C^*(x)=\mathbf1_{\{\eta_1(x)\geq1/2\}},
$$

with arbitrary tie breaking. Its [Bayes decision boundary](../../../statistical-learning.md#bayes-decision-boundary) is

$$
\boxed{\{x:\eta_1(x)=\eta_0(x)\}
=\{x:\eta_1(x)=1/2\}.}
$$

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Let $N_k(x)$ index the $k$ closest training covariates to $x$. The [K-nearest neighbors algorithm](../../../statistical-learning.md#k-nearest-neighbors-algorithm) estimates

$$
\widehat\eta_1(x)=\frac1k\sum_{i\in N_k(x)}Y_i
$$

and predicts one when this average is at least $1/2$.

Small $k$ gives low smoothing bias but high sampling variance and a jagged [decision boundary](../../../statistical-learning.md#decision-boundary). Larger $k$ averages more labels, reducing variance and producing a smoother boundary, but it mixes increasingly distant covariates and raises bias. The optimal balance depends on sample size, dimension, and smoothness of $\eta_1$, and is commonly selected by [cross-validation](../../../statistical-learning.md#cross-validation).

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/i">i</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/i/solution">Solution</h5>

↑ **Parent:** [I](#6/c/i)

For $\phi(x)=x$ and centered data, the objective is the [Rayleigh quotient](../../../linear-operator-theory.md#rayleigh-quotient)

$$
u^TSu,
\qquad
S=\frac1n\sum_{i=1}^nX_iX_i^T,
\qquad \lVert u\rVert_2=1.
$$

This is the first-direction optimization in [principal component analysis](../../../statistical-learning.md#principal-component-analysis). Therefore $\widehat u$ is any unit [eigenvector](../../../linear-operator-theory.md#eigenvector) of the sample [covariance matrix](../../../variance.md#covariance-matrix) $S$ corresponding to its largest [eigenvalue](../../../linear-operator-theory.md#eigenvalue).

<h4 id="6/c/ii">ii</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/c/ii)

Write $\Phi\alpha=\sum_i\alpha_i\phi(X_i)$. By the definition of the [kernel matrix](../../../probability-and-statistics.md#kernel-matrix),

$$
\lVert\Phi\alpha\rVert_{\mathcal H}^2=\alpha^TK\alpha
$$

and

$$
\frac1n\sum_{j=1}^n
\langle\Phi\alpha,\phi(X_j)\rangle_{\mathcal H}^2
=\frac1n\alpha^TK^2\alpha.
$$

The irrelevant positive factor $1/n$ gives exactly the stated constrained optimization.

Let $Kv_1=\lambda_1v_1$, where $\lambda_1>0$ is the largest [eigenvalue](../../../linear-operator-theory.md#eigenvalue) and $\lVert v_1\rVert_2=1$. The generalized [Rayleigh quotient](../../../linear-operator-theory.md#rayleigh-quotient) is maximized by

$$
\widehat\alpha=\frac{v_1}{\sqrt{\lambda_1}},
$$

up to sign and addition of a vector in $\ker K$, which does not change $\widehat u=\Phi\widehat\alpha$. Repeated leading eigenvectors give further principal directions.

<h4 id="6/c/iii">iii</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/c/iii)

[Kernel principal component analysis](../../../probability-and-statistics.md#kernel-principal-component-analysis) diagonalizes the centered $n$ by $n$ [kernel matrix](../../../probability-and-statistics.md#kernel-matrix) instead of an explicit covariance operator in a possibly infinite-dimensional feature space. A new point has coordinate

$$
\langle\widehat u_j,\phi(x)\rangle_{\mathcal H}
=\sum_i\widehat\alpha_{ji}k(X_i,x),
$$

so the leading coordinates require only evaluations of the [positive-semidefinite kernel](../../../probability-and-statistics.md#positive-semidefinite-kernel).

Running the [K-nearest neighbors algorithm](../../../statistical-learning.md#k-nearest-neighbors-algorithm) in a truncated collection of these coordinates can remove low-variance noise, reduce effective dimension, and allow a nonlinear boundary in the original covariates. This is the [kernel trick](../../../probability-and-statistics.md#kernel-trick): every feature-space inner product needed for fitting and projection is replaced by $k(x,z)=\langle\phi(x),\phi(z)\rangle_{\mathcal H}$ without constructing $\phi(x)$ explicitly.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
