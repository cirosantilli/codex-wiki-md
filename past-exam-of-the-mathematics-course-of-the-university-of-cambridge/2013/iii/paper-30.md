# Paper 30

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_30.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_30.pdf)

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
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
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
    - [iv](#5/b/iv)
      - [Solution](#5/b/iv/solution)
    - [v](#5/b/v)
      - [Solution](#5/b/v/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [i](#6/b/i)
      - [Solution](#6/b/i/solution)
    - [ii](#6/b/ii)
      - [Solution](#6/b/ii/solution)
    - [iii](#6/b/iii)
      - [Solution](#6/b/iii/solution)

## 1

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use the [normal linear model](../../../statistical-modelling.md#normal-linear-model)

$$
\boxed{Y=X\beta+\varepsilon,\qquad \varepsilon\sim N_n(0,\sigma^2I_n).}
$$

Here $Y$ is the response [random vector](../../../random-variable.md#random-vector), $X$ is the known [design matrix](../../../linear-regression.md#design-matrix), $\beta\in\mathbb R^p$ contains the unknown [regression coefficients](../../../linear-regression.md#regression-coefficient), and $\sigma^2>0$ is the common error [variance](../../../variance.md). Conditional on $X$, the errors have [normal distributions](../../../probability-theory.md#normal-distribution) and are [independent random variables](../../../random-variable.md#independent-random-variables). Require $\operatorname{rank}X=p\leq n$ for [identifiability](../../../statistical-model.md#identifiability) of $\beta$ and invertibility of $X^TX$. Usually $n>p$ is needed to estimate the error [variance](../../../variance.md) from the [regression residuals](../../../probability-and-statistics.md#regression-residual). An intercept, when included, is represented by a column of ones in $X$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Full column [matrix rank](../../../vector-space.md#matrix-rank) makes $X^TX$ a [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix), and its [matrix inverse](../../../linear-algebra.md#matrix-inverse) is symmetric. Thus the [hat matrix](../../../statistical-modelling.md#hat-matrix) satisfies

$$
P^T=X\bigl((X^TX)^{-1}\bigr)^TX^T=P,
\qquad P^2=X(X^TX)^{-1}(X^TX)(X^TX)^{-1}X^T=P.
$$

Also $PX=X$ and the image of $P$ is contained in the [column space](../../../vector-space.md#column-space) of $X$. These identities show that **$P$ is the [orthogonal projection matrix](../../../linear-algebra.md#orthogonal-projection-matrix) onto the [column space](../../../vector-space.md#column-space) of $X$**.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares) estimator is $\widehat\beta=(X^TX)^{-1}X^TY$. Consequently the [fitted values](../../../linear-regression.md#fitted-values) and [regression residuals](../../../probability-and-statistics.md#regression-residual) are

$$
\widehat Y=X\widehat\beta=PY,\qquad e=Y-\widehat Y=(I_n-P)Y.
$$

An affine transformation of a [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution) is again [multivariate normal](../../../probability-and-statistics.md#multivariate-normal-distribution), possibly with a singular [covariance matrix](../../../variance.md#covariance-matrix). For a [random vector](../../../random-variable.md#random-vector) with [covariance matrix](../../../variance.md#covariance-matrix) $\Sigma$, its transformed [covariance matrix](../../../variance.md#covariance-matrix) is $A\Sigma A^T$. Since $PX=X$, $P^2=P=P^T$ and $(I-P)^2=I-P$, these results give

$$
\boxed{\widehat Y\sim N_n(X\beta,\sigma^2P),\qquad e\sim N_n(0,\sigma^2(I_n-P)).}
$$

Both [multivariate normal distributions](../../../probability-and-statistics.md#multivariate-normal-distribution) are supported on their respective projected subspaces. In particular, $\widehat Y_i$ has [variance](../../../variance.md) $\sigma^2P_{ii}$ and $e_i$ has [variance](../../../variance.md) $\sigma^2(1-P_{ii})$; the [regression residuals](../../../probability-and-statistics.md#regression-residual) need not be mutually independent.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Because both vectors are linear transformations of the same [multivariate normal](../../../probability-and-statistics.md#multivariate-normal-distribution) response, $(\widehat Y,e)$ is jointly [multivariate normal](../../../probability-and-statistics.md#multivariate-normal-distribution). Its cross-[covariance matrix](../../../variance.md#covariance-matrix) is

$$
\operatorname{Cov}(\widehat Y,e)=P(\sigma^2I_n)(I_n-P)^T
=\sigma^2(P-P^2)=0.
$$

Zero cross-[covariance](../../../variance.md#covariance) implies independence for jointly [multivariate normal](../../../probability-and-statistics.md#multivariate-normal-distribution) vectors, including singular ones. Therefore **the [fitted values](../../../linear-regression.md#fitted-values) and the entire vector of [regression residuals](../../../probability-and-statistics.md#regression-residual) are independent**. The [fitted-residual orthogonality](../../../statistical-modelling.md#fitted-residual-orthogonality) identity gives the zero [covariance](../../../variance.md#covariance); the [normal distribution](../../../probability-theory.md#normal-distribution) assumption is what upgrades it to independence.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The [simple linear regression](../../../linear-regression.md#simple-linear-regression) assumes a straight conditional mean, $E(Y_i\mid x_i)=\beta_0+\beta_1x_i$, so that errors are centred at zero throughout the predictor range. The displayed [regression residuals](../../../probability-and-statistics.md#regression-residual) are predominantly positive at both ends and negative in the middle. This is a [residual curvature diagnostic](../../../probability-and-statistics.md#residual-curvature-diagnostic): the fitted straight line misses a curved conditional mean. **The main concern is the shape of the mean function.** The plot alone does not establish failure of the [normal distribution](../../../probability-theory.md#normal-distribution) assumption or a particular error [variance](../../../variance.md) model.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

A natural next fit is [quadratic regression](../../../linear-regression.md#quadratic-regression), which remains a [normal linear model](../../../statistical-modelling.md#normal-linear-model) in its unknown [regression coefficients](../../../linear-regression.md#regression-coefficient):

$$
\boxed{Y_i=\beta_0+\beta_1x_i+\beta_2x_i^2+\varepsilon_i,
\qquad \varepsilon_i\overset{\mathrm{iid}}\sim N(0,\sigma^2).}
$$

The new [design matrix](../../../linear-regression.md#design-matrix) has rows $(1,x_i,x_i^2)$ and must have [matrix rank](../../../vector-space.md#matrix-rank) three; three distinct predictor values suffice. The curved [regression residual](../../../probability-and-statistics.md#regression-residual) pattern suggests trying a positive quadratic term, but its sign and adequacy should be checked after fitting. Inspect the new [regression residuals](../../../probability-and-statistics.md#regression-residual) to see whether the systematic curvature has disappeared.

## 2

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Write $m_i=\mu+\alpha_i$. Apart from a constant, the [log-likelihood](../../../statistical-modelling.md#log-likelihood) is

$$
\ell=-\frac{IJ}{2}\log\sigma^2-\frac{1}{2\sigma^2}\sum_{i=1}^I\sum_{j=1}^J(Y_{ij}-m_i)^2.
$$

For each group,

$$
\sum_j(Y_{ij}-m_i)^2=\sum_j(Y_{ij}-\overline Y_i)^2+J(\overline Y_i-m_i)^2,
\qquad \overline Y_i=J^{-1}\sum_jY_{ij}.
$$

Thus [maximum likelihood estimation](../../../statistical-modelling.md#maximum-likelihood-estimation) sets $\widehat m_i=\overline Y_i$. The [corner-point constraint](../../../statistical-model.md#corner-point-constraint) $\alpha_1=0$ identifies $m_1=\mu$, giving

$$
\boxed{\widehat\mu=\overline Y_1,\qquad
\widehat\alpha_i=\overline Y_i-\overline Y_1\quad(i=2,\ldots,I).}
$$

The baseline mean is the first group mean, rather than the grand mean, because of the chosen [identifiability](../../../statistical-model.md#identifiability) constraint.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Group means are [independent random variables](../../../random-variable.md#independent-random-variables) with [normal distributions](../../../probability-theory.md#normal-distribution)

$$
\overline Y_i\sim N(\mu+\alpha_i,\sigma^2/J).
$$

The resulting univariate [sampling distributions](../../../statistical-modelling.md#sampling-distribution) are

$$
\boxed{\widehat\mu\sim N(\mu,\sigma^2/J),\qquad
\widehat\alpha_2\sim N(\alpha_2,2\sigma^2/J).}
$$

The same [variance](../../../variance.md) calculation holds for every $i\geq2$, since the difference involves two independent group means. Therefore the [standard errors](../../../statistical-inference.md#standard-error) satisfy

$$
\frac{\operatorname{se}(\widehat\alpha_i)}{\operatorname{se}(\widehat\mu)}
=\frac{\sqrt{2}\sigma/\sqrt J}{\sigma/\sqrt J}=\boxed{\sqrt2}.
$$

Replacing $\sigma$ by a common estimated error [standard deviation](../../../variance.md#standard-deviation) preserves this ratio. Although the individual group means are independent, the contrasts $\widehat\alpha_i$ share the baseline mean and have [covariance](../../../variance.md#covariance) $\sigma^2/J$ for distinct $i\geq2$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Index chocolate by $a\in\{A,B,C,D\}$, day by $d$ in the three observed categories, and replicate by $r\in\{1,2\}$. The additive [two-factor normal linear model](../../../statistical-modelling.md#two-factor-normal-linear-model) is

$$
Y_{adr}=\mu+\alpha_a+\gamma_d+\varepsilon_{adr},\qquad
\varepsilon_{adr}\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

Here $Y_{adr}$ is the board count, $\mu$ is the mean for the reference chocolate and reference day, and $\alpha_a,\gamma_d$ are chocolate and day [fixed effects](../../../statistical-modelling.md#fixed-effect). With [corner-point constraints](../../../statistical-model.md#corner-point-constraint), set $\alpha_A=0$ and $\gamma_{d_0}=0$, where $d_0$ is the first level in the day factor. The printed coefficient-free output does not determine that factor ordering; the model is unchanged by a different reference category. There is **no chocolate–day [interaction term](../../../statistical-model.md#interaction-term) in this fit**. The six free mean [statistical parameters](../../../statistical-model.md#statistical-parameter) consist of one baseline, three chocolate contrasts and two day contrasts; the common error [variance](../../../variance.md) supplies a further [statistical parameter](../../../statistical-model.md#statistical-parameter).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Test $H_0:\gamma_d=0$ for both nonreference days, against at least one nonzero day [fixed effect](../../../statistical-modelling.md#fixed-effect), conditional on chocolate. There are two added [regression coefficients](../../../linear-regression.md#regression-coefficient) and $24-6=18$ residual [statistical degrees of freedom](../../../statistical-inference.md#statistical-degrees-of-freedom). The [nested-model F-test](../../../probability-and-statistics.md#nested-model-f-test) statistic is

$$
\boxed{F=\frac{9.750/2}{107.083/18}=\frac{4.875}{5.9491}\simeq0.8195.}
$$

Under $H_0$ and the [normal linear model](../../../statistical-modelling.md#normal-linear-model) assumptions, $F\sim F_{2,18}$. Its 5% upper critical value is $3.555$, so **do not reject the absence of day effects**; the [p-value](../../../statistical-modelling.md#p-value) is approximately $0.456$. Thus the missing row has two [statistical degrees of freedom](../../../statistical-inference.md#statistical-degrees-of-freedom), mean square $4.875$, and the [F-test](../../../probability-and-statistics.md#f-test) value above. These observations do not provide evidence that including day improves the chocolate-adjusted mean model. They do not prove that every possible day effect or chocolate–day [interaction term](../../../statistical-model.md#interaction-term) is absent.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

The [analysis of variance](../../../linear-regression.md#analysis-of-variance) provides evidence of a chocolate effect both with day included ($F_{3,18}=3.9665$, [p-value](../../../statistical-modelling.md#p-value) $0.02473$) and with day omitted ($F_{3,20}=4.039$, [p-value](../../../statistical-modelling.md#p-value) $0.02133$). Because every chocolate–day cell has the same replication, [balanced factorial orthogonality](../../../linear-regression.md#balanced-factorial-orthogonality) separates the two main effects; the chocolate row is meaningful despite being entered first.

The chocolate-only fitted group means are approximately $14.17,11.67,9.33,11.33$ boards for A, B, C, D respectively. Thus **A has the largest fitted lecturing speed and C the smallest**. Relative to A, the fitted differences are $-2.50,-4.83,-2.83$ boards. The printed individual [Student t-tests](../../../statistical-modelling.md#student-s-t-test) give strong evidence for the A–C contrast ([p-value](../../../statistical-modelling.md#p-value) $0.00245$); B and D versus A have [p-values](../../../statistical-modelling.md#p-value) $0.08835$ and $0.05582$, respectively. Those latter contrasts are not significant at 5%, and the output does not test all other pairwise comparisons. Simultaneous claims would require accounting for [multiple hypothesis testing](../../../statistical-modelling.md#multiple-hypothesis-testing).

There is little evidence of a day effect after adjusting for chocolate. A chocolate-only [normal linear model](../../../statistical-modelling.md#normal-linear-model) is therefore a reasonable simpler summary, with residual [standard deviation](../../../variance.md#standard-deviation) about $2.42$ boards and explained variation $R^2\simeq0.377$. This is an association under the additive [statistical model](../../../statistical-model.md); a causal claim would additionally require an appropriate assignment of chocolate and checks of the [regression residuals](../../../probability-and-statistics.md#regression-residual) and possible [interaction terms](../../../statistical-model.md#interaction-term).

## 3

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

An [exponential dispersion family](../../../exponential-family.md#exponential-dispersion-model) has density or mass function, relative to a fixed measure,

$$
f(y;\theta,\phi)=\exp\left\{\frac{y\theta-b(\theta)}{\phi}+c(y,\phi)\right\},\qquad \phi>0.
$$

Here $\theta$ is the [natural parameter](../../../exponential-family.md#natural-parameter-of-an-exponential-family), $b$ is the [cumulant function](../../../exponential-family.md#cumulant-function-of-an-exponential-family), and $\phi$ is the [dispersion parameter](../../../exponential-family.md#dispersion-parameter). Assume the [natural parameter](../../../exponential-family.md#natural-parameter-of-an-exponential-family) lies in the interior of its domain and derivatives can pass through the normalizing integral. Differentiating normalization once and twice gives

$$
\boxed{\mu=E(Y)=b'(\theta),\qquad
\operatorname{Var}(Y)=\phi b''(\theta)=\phi V(\mu).}
$$

The [variance function](../../../exponential-family.md#variance-function) is $V(\mu)=b''((b')^{-1}(\mu))$, where the mean-to-natural-parameter inverse exists. The [dispersion parameter](../../../exponential-family.md#dispersion-parameter) may be fixed, as in a [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution), rather than estimated.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For $y=0,1,2,\ldots$ and $\lambda>0$, the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) has mass

$$
\Pr(Y=y)=\frac{e^{-\lambda}\lambda^y}{y!}
=\exp\{y\log\lambda-\lambda-\log(y!)\}.
$$

Match this to the [exponential dispersion family](../../../exponential-family.md#exponential-dispersion-model) with

$$
\boxed{\theta=\log\lambda,\quad b(\theta)=e^\theta,\quad
\phi=1,\quad c(y,1)=-\log(y!).}
$$

Then $\mu=b'(\theta)=e^\theta=\lambda$ and $V(\mu)=b''(\theta)=\mu$. The [canonical link function](../../../statistical-modelling.md#canonical-link-function) expresses the [natural parameter](../../../exponential-family.md#natural-parameter-of-an-exponential-family) in terms of the mean, so the [Poisson canonical link](../../../statistical-modelling.md#poisson-canonical-link) is **$g(\mu)=\log\mu$**. Its conditional [variance](../../../variance.md) equals its conditional mean.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The coefficient labelled `yr2` identifies year as a factor. With $z_i=0$ in the first year and $z_i=1$ in the second, the [Poisson regression](../../../statistical-modelling.md#poisson-regression) assumes independent daily counts conditional on year,

$$
Y_i\sim\operatorname{Pois}(\mu_i),\qquad
\log\mu_i=\beta_0+\beta_1z_i.
$$

The unknown mean [statistical parameters](../../../statistical-model.md#statistical-parameter) are the first-year log daily rate $\beta_0$ and the second-year log rate ratio $\beta_1$; the [dispersion parameter](../../../exponential-family.md#dispersion-parameter) is fixed at one. Approximate 95% [Wald confidence intervals](../../../statistical-inference.md#wald-confidence-interval) are

$$
\begin{aligned}
\widehat\beta_0&=1.78810,&\quad \beta_0&\in1.78810\pm1.96(0.02141)=(1.74614,1.83006),\\
\widehat\beta_1&=-0.09816,&\quad \beta_1&\in-0.09816\pm1.96(0.03105)=(-0.15902,-0.03730).
\end{aligned}
$$

Exponentiating yields the first-year fitted daily mean $5.978$, with [confidence interval](../../../statistical-inference.md#confidence-interval) $(5.732,6.234)$, and

$$
\boxed{\frac{\widehat\mu_2}{\widehat\mu_1}=0.9065,\qquad
\frac{\mu_2}{\mu_1}\in(0.8530,0.9634).}
$$

The second-year fitted daily mean is $e^{1.78810-0.09816}=5.419$. Thus this [Poisson regression](../../../statistical-modelling.md#poisson-regression) estimates a 9.35% fall, with an approximate interval for the percentage fall from 3.66% to 14.70%. These [confidence intervals](../../../statistical-inference.md#confidence-interval) rely on the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) and independence assumptions.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The [Quasi-Poisson regression](../../../statistical-modelling.md#quasi-poisson-regression) retains the same conditional mean but permits

$$
E(Y_i\mid z_i)=\mu_i,\qquad \log\mu_i=\beta_0+\beta_1z_i,
\qquad \operatorname{Var}(Y_i\mid z_i)=\phi\mu_i.
$$

This is a mean–[variance function](../../../exponential-family.md#variance-function) specification through [quasi-likelihood](../../../statistical-modelling.md#quasi-likelihood); it does not assign a full [probability distribution](../../../probability-theory.md#probability-distribution) to each count. For independent observations, the [quasi-score equation](../../../statistical-modelling.md#quasi-score-equation) is proportional to $\sum_i x_i(Y_i-\mu_i)=0$, so the mean [statistical parameter](../../../statistical-model.md#statistical-parameter) estimates equal those from [Poisson regression](../../../statistical-modelling.md#poisson-regression). The output estimates $\widehat\phi=3.515351$ through the [Pearson dispersion estimator](../../../statistical-modelling.md#pearson-dispersion-estimator), and inflates the [standard errors](../../../statistical-inference.md#standard-error) by approximately $\sqrt{\widehat\phi}=1.875$.

The large [residual deviance](../../../statistical-modelling.md#residual-deviance) relative to 728 residual [statistical degrees of freedom](../../../statistical-inference.md#statistical-degrees-of-freedom) also signals substantial [overdispersion](../../../exponential-family.md#overdispersion). Daily weather, traffic and other omitted conditions may produce greater count variation than a homogeneous [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) allows. The [Quasi-Poisson regression](../../../statistical-modelling.md#quasi-poisson-regression) accounts for that extra marginal [variance](../../../variance.md). It still requires a correct conditional mean and an appropriate independence assumption; a common [dispersion parameter](../../../exponential-family.md#dispersion-parameter) alone does not repair [serial correlation](../../../variance.md#serial-correlation).

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Under the more plausible [Quasi-Poisson regression](../../../statistical-modelling.md#quasi-poisson-regression), the year [Wald statistic](../../../statistical-modelling.md#wald-test) is $-1.686$, with reported [p-value](../../../statistical-modelling.md#p-value) $0.0922$. An approximate 95% [confidence interval](../../../statistical-inference.md#confidence-interval) is

$$
\beta_1\in-0.09816\pm1.96(0.05821)=(-0.21225,0.01593),
\qquad e^{\beta_1}\in(0.8088,1.0161).
$$

Thus **the estimated fall is about 9.35%, but the data do not establish a reduction at the 5% level after allowing for [overdispersion](../../../exponential-family.md#overdispersion)**. The interval allows both a sizeable reduction and a small increase. The before–after comparison also lacks a contemporaneous randomized control, so [causal inference](../../../causal-inference.md) about the campaign would require addressing other changes between years. The small [Poisson regression](../../../statistical-modelling.md#poisson-regression) [p-value](../../../statistical-modelling.md#p-value) is not sufficient evidence of a campaign effect when its [variance](../../../variance.md) assumption is unsuitable.

## 4

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Measurements from the same person share baseline strength and likely share an individual response to training. An [ordinary linear model](../../../statistical-modelling.md#normal-linear-model) with independent errors treats all 600 readings as independent conditional on week; that fails to represent their within-person [correlation](../../../variance.md#pearson-correlation-coefficient). The [regression residuals](../../../probability-and-statistics.md#regression-residual) can remain associated even when the population mean is linear in time. A [random intercept](../../../statistical-modelling.md#random-intercept) captures differences in baseline strength, and a [random slope](../../../statistical-modelling.md#random-slope) can additionally describe differences in progress.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For subject $i=1,\ldots,100$ and $t_j\in\{0,2,4,6,8,10\}$, the [random-intercept linear mixed model](../../../statistical-modelling.md#random-intercept-linear-mixed-model) is

$$
Y_{ij}=\beta_0+\beta_1t_j+b_i+\varepsilon_{ij},\qquad
b_i\overset{\mathrm{iid}}\sim N(0,\tau^2),\qquad
\varepsilon_{ij}\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

All subject [random effects](../../../statistical-modelling.md#random-effect) and measurement errors are mutually independent. The [fixed effects](../../../statistical-modelling.md#fixed-effect) $\beta_0,\beta_1$ describe the population mean baseline and weekly gain. Conditional on $b_i$, a person's observations have independent [normal distributions](../../../probability-theory.md#normal-distribution); after integrating out $b_i$, their [covariance](../../../variance.md#covariance) is $\tau^2$ at distinct weeks and their common [variance](../../../variance.md) is $\tau^2+\sigma^2$. Therefore their [correlation](../../../variance.md#pearson-correlation-coefficient) is $\tau^2/(\tau^2+\sigma^2)$.

This [Gaussian linear mixed model](../../../statistical-modelling.md#gaussian-linear-mixed-model) permits correlated repeated readings while keeping different subjects independent. The fitted [standard deviations](../../../variance.md#standard-deviation) are $\widehat\tau=21.67593$ kg and $\widehat\sigma=14.23496$ kg, giving within-person [correlation](../../../variance.md#pearson-correlation-coefficient) about $0.699$. All persons still have the same latent weekly slope in this model.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Allow each subject to have a separate baseline and slope through a [correlated random-intercept and random-slope model](../../../statistical-modelling.md#correlated-random-intercept-and-random-slope-model):

$$
Y_{ij}=\beta_0+\beta_1t_j+b_{0i}+b_{1i}t_j+\varepsilon_{ij},\qquad
\begin{pmatrix}b_{0i}\\b_{1i}\end{pmatrix}\overset{\mathrm{iid}}\sim
N_2\left(0,
\begin{pmatrix}\tau_0^2&\rho\tau_0\tau_1\\\rho\tau_0\tau_1&\tau_1^2\end{pmatrix}\right),
\qquad \varepsilon_{ij}\overset{\mathrm{iid}}\sim N(0,\sigma^2).
$$

The subject [random effects](../../../statistical-modelling.md#random-effect) are independent of all measurement errors, and subjects are independent. The within-person [covariance](../../../variance.md#covariance) between times $s,t$ is $\tau_0^2+(s+t)\rho\tau_0\tau_1+st\tau_1^2$, with an additional $\sigma^2$ when the same reading is used twice.

**Prefer the model with a [random slope](../../../statistical-modelling.md#random-slope).** The [maximum likelihood estimation](../../../statistical-modelling.md#maximum-likelihood-estimation) refits improve twice the [log-likelihood](../../../statistical-modelling.md#log-likelihood) by $227.9604$ while adding two [covariance](../../../variance.md#covariance) [statistical parameters](../../../statistical-model.md#statistical-parameter). Both the [Akaike information criterion](../../../statistical-modelling.md#akaike-information-criterion) ($5165.779$ to $4941.819$) and [Bayesian information criterion](../../../statistical-modelling.md#bayesian-information-criterion) ($5183.367$ to $4968.200$) strongly favour it. The printed nominal [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test) is overwhelming. The usual reference [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) with two [statistical degrees of freedom](../../../statistical-inference.md#statistical-degrees-of-freedom) is not an exact regular calibration, since zero slope [variance](../../../variance.md) is a boundary and the intercept–slope [correlation](../../../variance.md#pearson-correlation-coefficient) is then unidentified; a design-specific [parametric bootstrap](../../../statistical-modelling.md#parametric-bootstrap) could calibrate it. This qualification does not undermine the substantial descriptive improvement shown by both information criteria.

The preferred fit estimates population mean baseline strength $\widehat\beta_0=61.09286$ kg and weekly gain $\widehat\beta_1=2.83143$ kg/week. The between-person baseline [standard deviation](../../../variance.md#standard-deviation) is $\widehat\tau_0=15.785582$ kg, and the between-person slope [standard deviation](../../../variance.md#standard-deviation) is $\widehat\tau_1=2.738666$ kg/week. Their estimated [correlation](../../../variance.md#pearson-correlation-coefficient) $\widehat\rho=0.117$ is weakly positive, giving random-effect [covariance](../../../variance.md#covariance) about $5.058$ kg$^2$/week; its uncertainty is not supplied. The measurement-error [standard deviation](../../../variance.md#standard-deviation) is $\widehat\sigma=9.923280$ kg. The printed $-0.038$ instead describes the [correlation](../../../variance.md#pearson-correlation-coefficient) between the estimated [fixed effects](../../../statistical-modelling.md#fixed-effect), not between the subject [random effects](../../../statistical-modelling.md#random-effect). These [statistical parameter](../../../statistical-model.md#statistical-parameter) estimates come from [restricted maximum likelihood](../../../statistical-modelling.md#restricted-maximum-likelihood); the model comparison uses the separate [maximum likelihood estimation](../../../statistical-modelling.md#maximum-likelihood-estimation) fits.

The population mean fitted trajectory is $61.09286+2.83143t$ kg. Hence

$$
\boxed{\text{mean ten-week gain}=10\widehat\beta_1=28.3143\ \mathrm{kg},
\qquad \text{mean at week ten}=89.40716\ \mathrm{kg}.}
$$

Using the reported slope [standard error](../../../statistical-inference.md#standard-error), an approximate 95% [confidence interval](../../../statistical-inference.md#confidence-interval) for the population mean gain is $28.3143\pm1.96(2.984464)=(22.46,34.16)$ kg; a [Student t confidence interval](../../../statistical-inference.md#student-t-confidence-interval) with 499 [statistical degrees of freedom](../../../statistical-inference.md#statistical-degrees-of-freedom) is almost identical.

Successful individuals can improve far more than the average. Their latent ten-week gains have fitted [normal distribution](../../../probability-theory.md#normal-distribution)

$$
G_i=10(\beta_1+b_{1i})\sim N(28.3143,27.38666^2).
$$

A clear estimate for an upper-performing group uses a [between-person slope quantile](../../../statistical-modelling.md#between-person-slope-quantile): the 95th percentile is $28.3143+1.645(27.38666)\simeq73.4$ kg, and the 97.5th percentile is about $82.0$ kg. **The upper 5% of fitted underlying gains begin around 73 kg.** These are person-to-person performance [quantiles](../../../probability-theory.md#quantile-function), not [confidence intervals](../../../statistical-inference.md#confidence-interval) for the population mean. Identifying the best observed trainee would require that person's data or fitted subject [random effects](../../../statistical-modelling.md#random-effect); the aggregate output cannot identify a literal maximum. If performance means the observed difference of endpoint readings, add the measurement-error [variance](../../../variance.md) $2\sigma^2$ to the latent gain [variance](../../../variance.md).

## 5

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

[Observed heterogeneity](../../../statistical-modelling.md#observed-heterogeneity) is variation in outcome propensities explained by measured [covariates](../../../statistical-model.md#covariate), such as age or sex. In [logistic regression](../../../statistical-modelling.md#logistic-regression), subjects with different recorded predictor values may have different success [probabilities](../../../probability-theory.md#probability), even before allowing for their previous outcomes. This is heterogeneity visible through observed predictors.

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

[Unobserved heterogeneity](../../../statistical-modelling.md#unobserved-heterogeneity) is persistent variation between subjects arising from unmeasured characteristics. A subject-specific [latent variable](../../../statistical-modelling.md#latent-variable) or [random intercept](../../../statistical-modelling.md#random-intercept) can represent it. Subjects with high latent success propensities tend to succeed repeatedly, so their observed outcomes can have positive [serial correlation](../../../variance.md#serial-correlation) even when outcomes are conditionally independent given that propensity. Apparent persistence therefore need not imply [true state dependence](../../../statistical-modelling.md#true-state-dependence).

<h4 id="5/a/iii">iii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/a/iii)

[True state dependence](../../../statistical-modelling.md#true-state-dependence), also called [true contagion](../../../statistical-modelling.md#true-state-dependence), means that a previous outcome changes the distribution of a subsequent outcome after controlling both measured [covariates](../../../statistical-model.md#covariate) and persistent [unobserved heterogeneity](../../../statistical-modelling.md#unobserved-heterogeneity). For example, an earlier successful week may make later success more likely through habit formation. A lagged-outcome coefficient in an inadequate [statistical model](../../../statistical-model.md) can also reflect omitted subject differences, so positive observed persistence alone does not distinguish [true state dependence](../../../statistical-modelling.md#true-state-dependence) from [unobserved heterogeneity](../../../statistical-modelling.md#unobserved-heterogeneity).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

Let $Y_{it}\in\{0,1\}$ indicate a smoking-free week, $S_i$ the recorded sex indicator, $A_i$ age in years and $T_i$ assigned treatment. The screening history supplies $Y_{i0}=0$; earlier lag initializations are also zero. A [history-dependent logistic regression](../../../statistical-modelling.md#conditional-logistic-model-for-longitudinal-binary-data) for the first model is

$$
Y_{it}\mid\mathcal H_{i,t-1},S_i,A_i,T_i\sim\operatorname{Bernoulli}(p_{it}),\qquad
\log\frac{p_{it}}{1-p_{it}}=\beta_0+\beta_SS_i+\beta_AA_i+\beta_TT_i+\gamma Y_{i,t-1}.
$$

Here $t=1,\ldots,10$, $\mathcal H_{i,t-1}$ is the observed past, and the five unknown [regression coefficients](../../../linear-regression.md#regression-coefficient) have time-invariant values. Conditional on baseline [covariates](../../../statistical-model.md#covariate), this model has the first-order [Markov property](../../../markov-process.md#markov-property): only the immediately preceding outcome enters the current conditional [probability](../../../probability-theory.md#probability). Distinct subjects have independent histories. There is no subject [random effect](../../../statistical-modelling.md#random-effect) or additional time trend in this fit.

Using the [chain rule for probabilities](../../../probability-theory.md#chain-rule-for-probabilities), the individual conditional [likelihood](../../../statistical-modelling.md#likelihood-function) is

$$
\boxed{L_i(\beta,\gamma)=\prod_{t=1}^{10}p_{it}^{y_{it}}(1-p_{it})^{1-y_{it}},\qquad
p_{it}=\frac{e^{\eta_{it}}}{1+e^{\eta_{it}}}.}
$$

The lagged values in $\eta_{it}$ are the individual's actual preceding outcomes. This product is a sequential conditional [likelihood](../../../statistical-modelling.md#likelihood-function), not an assertion of unconditional independence of the ten readings. The full conditional [likelihood](../../../statistical-modelling.md#likelihood-function) is $\prod_iL_i$; no extra [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution) factor is attached to the fixed screening history.

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

The second [logistic regression](../../../statistical-modelling.md#logistic-regression) adds $\gamma_2Y_{i,t-2}$ while retaining the first lag and baseline [covariates](../../../statistical-model.md#covariate). The models are nested under $H_0:\gamma_2=0$. Their [likelihood-ratio test statistic](../../../statistical-modelling.md#likelihood-ratio-test-statistic) is the reduction in [binomial deviance](../../../statistical-modelling.md#binomial-deviance),

$$
\boxed{2(\widehat\ell_2-\widehat\ell_1)=1164.4-1155.0=9.4.}
$$

Under the null and regular large-sample conditions for the correctly specified conditional [likelihood](../../../statistical-modelling.md#likelihood-function), this has an approximate [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) with one [statistical degree of freedom](../../../statistical-inference.md#statistical-degrees-of-freedom). Since $9.4>3.841$, reject at 5%; the approximate [p-value](../../../statistical-modelling.md#p-value) is $0.0022$. **Prefer the two-lag model to the one-lag model.** Its additional lag captures statistically useful information in the history.

<h4 id="5/b/iii">iii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/b/iii)

The [cumulative-response logistic model](../../../statistical-modelling.md#cumulative-response-logistic-model) uses $C_{it}=\sum_{s<t}Y_{is}$ instead of the two individual lag predictors. It and the two-lag [history-dependent logistic regression](../../../statistical-modelling.md#conditional-logistic-model-for-longitudinal-binary-data) are nonnested: the entire accumulated history generally cannot be represented using only the two recent outcomes. Their [binomial deviance](../../../statistical-modelling.md#binomial-deviance) difference therefore has no ordinary nested [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) calibration.

Use the [Akaike information criterion](../../../statistical-modelling.md#akaike-information-criterion), which up to the same saturated-model constant equals $D+2k$ for these [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution) conditional [likelihoods](../../../statistical-modelling.md#likelihood-function). The two-lag fit has six coefficients, while the cumulative fit has five:

$$
\operatorname{AIC}_2\doteq1155+2(6)=1167,\qquad
\operatorname{AIC}_3\doteq1122+2(5)=1132.
$$

Thus **prefer the cumulative-history model**, whose [Akaike information criterion](../../../statistical-modelling.md#akaike-information-criterion) is lower by 35 despite its smaller number of [statistical parameters](../../../statistical-model.md#statistical-parameter). This is a model-selection comparison of conditional histories, not a nested [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test).

<h4 id="5/b/iv">iv</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#5/b/iv)

The preferred [cumulative-response logistic model](../../../statistical-modelling.md#cumulative-response-logistic-model) estimates

$$
\operatorname{logit}(p_{it})=-1.417630-0.364092S_i+0.001224A_i
+0.327118T_i+0.399296C_{it},\qquad C_{it}=\sum_{s<t}Y_{is}.
$$

Its [logit link](../../../statistical-modelling.md#logit) describes conditional smoking-free [probability](../../../probability-theory.md#probability) given baseline predictors and prior successful weeks. Holding the other predictors fixed, males have $e^{-0.364092}=0.695$ times the female success [odds](../../../probability-theory.md#odds); the reported [p-value](../../../statistical-modelling.md#p-value) is $0.0152$, and the approximate 95% [odds ratio](../../../statistical-modelling.md#odds-ratio) [confidence interval](../../../statistical-inference.md#confidence-interval) is $(0.518,0.932)$. Age has estimated [odds ratio](../../../statistical-modelling.md#odds-ratio) $e^{0.001224}=1.0012$ per additional year, with [p-value](../../../statistical-modelling.md#p-value) $0.918$, giving little evidence for an age association in this fit.

The combined treatment has conditional success [odds ratio](../../../statistical-modelling.md#odds-ratio) $e^{0.327118}=1.387$ versus the reference treatment, with approximate 95% [confidence interval](../../../statistical-inference.md#confidence-interval) $(1.035,1.859)$ and [p-value](../../../statistical-modelling.md#p-value) $0.0285$. **The fitted conditional odds are about 39% higher for the combined treatment.** The trial randomization supports treatment comparisons, but conditioning on accumulated post-treatment outcomes means this coefficient is not directly the marginal total treatment effect.

Each previous successful week multiplies current success [odds](../../../probability-theory.md#odds) by $e^{0.399296}=1.491$, with approximate 95% [confidence interval](../../../statistical-inference.md#confidence-interval) $(1.329,1.673)$ and very small [p-value](../../../statistical-modelling.md#p-value) $1.06\times10^{-11}$. This is strong fitted persistence. It can reflect [true state dependence](../../../statistical-modelling.md#true-state-dependence), [unobserved heterogeneity](../../../statistical-modelling.md#unobserved-heterogeneity), or an omitted calendar-time trend; this fit alone cannot distinguish them. The baseline intercept implies success [probability](../../../probability-theory.md#probability) $\operatorname{logit}^{-1}(-1.417630)\simeq0.195$ for a reference-treatment female aged zero with no previous success. That age is outside the study's useful interpretation range, so the intercept chiefly anchors the regression. The [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution) [dispersion parameter](../../../exponential-family.md#dispersion-parameter) is fixed at one, and the residual [binomial deviance](../../../statistical-modelling.md#binomial-deviance) is 1122 on 995 [statistical degrees of freedom](../../../statistical-inference.md#statistical-degrees-of-freedom). With individual binary outcomes, comparing that [binomial deviance](../../../statistical-modelling.md#binomial-deviance) mechanically to a [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) is not a reliable general goodness-of-fit test.

<h4 id="5/b/v">v</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/v/solution">Solution</h5>

↑ **Parent:** [V](#5/b/v)

Take the event to mean three smoking-free weeks in succession, $Y_{i1}=Y_{i2}=Y_{i3}=1$. The initial cumulative count is zero. Along this path it equals $0,1,2$ in weeks one, two, three, respectively. In the [cumulative-response logistic model](../../../statistical-modelling.md#cumulative-response-logistic-model), define

$$
\pi_c=\frac{\exp(-1.417630+0.001224(20)+0.399296c)}
{1+\exp(-1.417630+0.001224(20)+0.399296c)}.
$$

The [chain rule for probabilities](../../../probability-theory.md#chain-rule-for-probabilities) then gives

$$
\boxed{\Pr(Y_{i1}=Y_{i2}=Y_{i3}=1\mid S_i=0,A_i=20,T_i=0,\mathcal H_{i0})
=\pi_0\pi_1\pi_2\simeq0.01911.}
$$

The three conditional [probabilities](../../../probability-theory.md#probability) are approximately $0.19891,0.27015,0.35559$. If “stop during the first three weeks” instead means at least one smoking-free week by week three, its different event has [probability](../../../probability-theory.md#probability) $1-(1-\pi_0)^3\simeq0.48590$: along the all-failure path the cumulative count stays zero. Stating the event resolves this wording ambiguity.

## 6

↑ **Parent:** [Paper 30](paper-30.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Let $q_{rs}$ be the [transition intensity](../../../survival-analysis.md#transition-intensity) from state $r$ to $s$, and let $Q$ be the [transition intensity matrix](../../../markov-process.md#transition-intensity-matrix), with $q_{rr}=-\sum_{s\ne r}q_{rs}$. For a [continuous-time multi-state model](../../../survival-analysis.md#continuous-time-multi-state-model) with the [time-homogeneous Markov property](../../../markov-process.md#time-homogeneous-markov-property), the [transition probability matrix](../../../markov-process.md#transition-semigroup-of-a-continuous-time-markov-chain) is $P(u)=e^{uQ}$, with entry $p_{rs}(u)$. Condition on each recorded initial state. Panel visits contribute [transition probabilities](../../../markov-process.md#transition-probability); an exact entry into the absorbing death state contributes a [statistical probability density](../../../continuous-probability-distribution.md#probability-density-function)

$$
g_{r3}(u)=\sum_{s=1}^2p_{rs}(u)q_{s3}.
$$

This [mixed panel and exact-death likelihood](../../../survival-analysis.md#mixed-panel-and-exact-death-likelihood) sums over the living state just before death. It accounts for survival until the event; replacing its final factor by $p_{r3}(u)$ would count deaths throughout the interval.

Using the actual visit times recovered from the PDF, the three individual [likelihood](../../../statistical-modelling.md#likelihood-function) contributions are

$$
\begin{aligned}
L_7={}&p_{12}(2.473380)p_{22}(3.708143)p_{22}(0.114158)
 p_{22}(0.811791)p_{22}(0.359291)p_{22}(0.457878)g_{23}(0.065913),\\
L_8={}&p_{11}(3.261286)p_{11}(1.231073),\\
L_9={}&p_{11}(1.289561)p_{11}(2.694442)p_{11}(0.450082)
 p_{12}(4.338740)p_{22}(0.273262).
\end{aligned}
$$

Here $g_{23}$ means $g_{r3}$ with $r=2$, not a [transition probability](../../../markov-process.md#transition-probability). Subjects 8 and 9 supply no event-density factor after their last panel observation. Assume independent subjects and noninformative examination and [censoring](../../../survival-analysis.md#censoring-statistics) times; conditional on their observation schedule, its distribution supplies no additional [statistical parameter](../../../statistical-model.md#statistical-parameter)-dependent factor. The patients' [covariates](../../../statistical-model.md#covariate) can be incorporated by using their own $Q_i$ in these same expressions.

For the progressive structure used in the subsequent output, put $a=q_{12}$, $b=q_{13}$, $c=q_{23}$ and $\lambda=a+b$. The [progressive illness-death model](../../../survival-analysis.md#progressive-illness-death-model) permits no recovery, so

$$
p_{11}(u)=e^{-\lambda u},\qquad p_{22}(u)=e^{-cu},\qquad
p_{12}(u)=\frac{a}{\lambda-c}(e^{-cu}-e^{-\lambda u}),\qquad
 g_{23}(u)=ce^{-cu}.
$$

When $\lambda=c$, the continuous limit is $p_{12}(u)=au e^{-cu}$. Thus the [likelihood](../../../statistical-modelling.md#likelihood-function) contributions simplify to

$$
\boxed{\begin{aligned}
L_7&=p_{12}(2.473380)c\,e^{-c(7.990554-2.473380)},\\
L_8&=e^{-\lambda(4.492359)},\\
L_9&=e^{-\lambda(4.434085)}p_{12}(4.338740)e^{-c(0.273262)}.
\end{aligned}}
$$

Intermediate unobserved disease transitions remain integrated into each panel [transition probability](../../../markov-process.md#transition-probability).

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/i">i</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/i/solution">Solution</h5>

↑ **Parent:** [I](#6/b/i)

The fitted [progressive illness-death model](../../../survival-analysis.md#progressive-illness-death-model) has three allowed arrows: $1\to2$ with estimated [transition intensity](../../../survival-analysis.md#transition-intensity) $0.1849$, $1\to3$ with $0.01935$, and $2\to3$ with $0.06143$, all in years$^{-1}$. State 3 is an [absorbing state](../../../markov-process.md#absorbing-state), and state 2 has no return arrow.

<a id="6/b/i/image-progressive-three-state-model-with-estimated-annual-transition-intensities"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-30-state-transitions.png)

**[Figure 1](#6/b/i/image-progressive-three-state-model-with-estimated-annual-transition-intensities). Progressive three-state model with estimated annual transition intensities**.

Once in state 2, the [holding time](../../../markov-process.md#holding-time) has an [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) with rate $q_{23}$, so the [mean holding time from a transition intensity matrix](../../../markov-process.md#mean-holding-time-from-a-transition-intensity-matrix) is

$$
\boxed{\widehat E(T_2)=\frac1{0.06143}=16.28\ \text{years}.}
$$

Apply a [confidence interval for an inverse rate](../../../markov-process.md#confidence-interval-for-an-inverse-rate) to the printed rate interval $(0.03552,0.1063)$: since inversion reverses order, the approximate 95% interval for the mean is

$$
\boxed{\left(\frac1{0.1063},\frac1{0.03552}\right)=(9.41,28.15)\ \text{years}.}
$$

The [time-homogeneous Markov property](../../../markov-process.md#time-homogeneous-markov-property) makes the future depend only on the current state; the [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) also has the [memoryless property](../../../continuous-probability-distribution.md#memorylessness-of-the-exponential-distribution). For a person currently in state 2,

$$
\boxed{p_{23}(2)=1-e^{-2(0.06143)}=0.11561.}
$$

Equivalently, $p_{22}(2)=p_{22}(1)^2\simeq0.9404163^2$. Thus the fitted two-year death [probability](../../../probability-theory.md#probability) is approximately **11.6%**.

<h4 id="6/b/ii">ii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/b/ii)

Let $z_i=(S_i,E_i,A_i)^T$ contain sex, the education indicator, and age at diagnosis. Write $\overline z$ for the sample means. The output's baseline [transition intensities](../../../survival-analysis.md#transition-intensity) are evaluated at those means, so use the centred [log-linear transition intensity model](../../../survival-analysis.md#log-linear-transition-intensity-model)

$$
q_{rs}(z_i)=q_{rs}(\overline z)\exp\{\beta_{rs}^T(z_i-\overline z)\},
\qquad (r,s)\in\{(1,2),(1,3),(2,3)\}.
$$

The full [transition intensity matrix](../../../markov-process.md#transition-intensity-matrix) is

$$
Q_i=\begin{pmatrix}
-q_{12}(z_i)-q_{13}(z_i)&q_{12}(z_i)&q_{13}(z_i)\\
0&-q_{23}(z_i)&q_{23}(z_i)\\
0&0&0
\end{pmatrix}.
$$

The fitted centred baselines are $(q_{12},q_{13},q_{23})(\overline z)=(0.1821,0.0126,0.0450)$, and fitted slope vectors in sex–education–age order are

$$
\widehat\beta_{12}=(0.09534,-0.4306,0.007627)^T,\qquad
\widehat\beta_{13}=(0,1.223,0.1262)^T,\qquad
\widehat\beta_{23}=(0,-1.490,0.07984)^T.
$$

The two sex coefficients displayed as zero are fixed by the specified constraints; they are not estimated to be exactly zero. There are three free baseline [transition intensities](../../../survival-analysis.md#transition-intensity) and seven free covariate slopes. The sample means are not printed, so uncentred intercepts at $z=0$ cannot be recovered numerically from this output.

Conditional on fixed [covariates](../../../statistical-model.md#covariate), subjects follow independent, correctly classified [continuous-time multi-state models](../../../survival-analysis.md#continuous-time-multi-state-model) obeying the [time-homogeneous Markov property](../../../markov-process.md#time-homogeneous-markov-property), with $P_i(u)=e^{uQ_i}$. The progression is irreversible and death absorbing, with constant [transition intensities](../../../survival-analysis.md#transition-intensity) during follow-up for each subject. In particular, the model uses fixed age at diagnosis rather than attained age. It assumes noninformative observation and [censoring](../../../survival-analysis.md#censoring-statistics), and treats death times as exact through the [mixed panel and exact-death likelihood](../../../survival-analysis.md#mixed-panel-and-exact-death-likelihood). The [Markov property](../../../markov-process.md#markov-property) rules out an additional effect of elapsed time in the current state after conditioning on it and the recorded predictors.

<h4 id="6/b/iii">iii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/b/iii)

Under $H_0$, the seven free covariate coefficients all equal zero. The [likelihood-ratio test statistic](../../../statistical-modelling.md#likelihood-ratio-test-statistic) is

$$
\boxed{2(\widehat\ell_1-\widehat\ell_0)=462.7531-442.0713=20.6818.}
$$

The larger fit has ten free [statistical parameters](../../../statistical-model.md#statistical-parameter), compared with three in the constant-rate fit, so the reference [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) has **seven [statistical degrees of freedom](../../../statistical-inference.md#statistical-degrees-of-freedom)**. Its 95th percentile is $14.06714$. Therefore reject $H_0$ at 5%; the [p-value](../../../statistical-modelling.md#p-value) is approximately $0.0043$, and the covariate model is preferred. The two constrained sex coefficients add no free [statistical parameters](../../../statistical-model.md#statistical-parameter).

For the dementia-to-death arrow, the [hazard ratio](../../../survival-analysis.md#hazard-ratio) for higher versus lower education is $e^{-1.490}=0.2254$, with approximate 95% [confidence interval](../../../statistical-inference.md#confidence-interval) $(e^{-2.547},e^{-0.4327})=(0.0783,0.6488)$. Thus higher education is associated with a roughly **77.5% lower fitted death [transition intensity](../../../survival-analysis.md#transition-intensity)**, conditional on diagnosis age; the interval excludes one. This is an observational association and is not a direct multiplicative statement about death [probability](../../../probability-theory.md#probability).

Each additional year of age at diagnosis multiplies the dementia-to-death [transition intensity](../../../survival-analysis.md#transition-intensity) by $e^{0.07984}=1.0831$, with [confidence interval](../../../statistical-inference.md#confidence-interval) $(e^{-0.007765},e^{0.1674})=(0.9923,1.1822)$. The estimate suggests an increase, but the interval includes one, so this individual age coefficient is not significant at 5%. Sex has [hazard ratio](../../../survival-analysis.md#hazard-ratio) one for this transition **by the model's imposed constraint**. The output supplies no estimated sex effect or test of that constraint for this arrow. The nonzero sex coefficient for $1\to2$ must not be mistaken for a sex effect on $2\to3$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
