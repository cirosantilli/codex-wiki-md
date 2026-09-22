# Paper 218

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_218.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_218.pdf)

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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
  - [d](#6/d)
    - [Solution](#6/d/solution)
  - [e](#6/e)
    - [Solution](#6/e/solution)
  - [f](#6/f)
    - [Solution](#6/f/solution)

## 1

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Put $s=x^Tx>0$ and $z=x^TY$. With objective $\lVert Y-x\beta\rVert_2^2+\lambda\beta^2$, [ridge regression](../../../linear-regression.md#ridge-regression) gives

$$
\widehat\beta=\frac z{s+\lambda}.
$$

For the duplicated design, the objective depends on $\beta_1+\beta_2$ through the loss and symmetry makes the minimum-penalty decomposition equal:

$$
\widehat\beta_1=\widehat\beta_2=\frac z{2s+\lambda},
\qquad
\widehat\beta_1+\widehat\beta_2=\frac{2z}{2s+\lambda}.
$$

Duplicating a predictor therefore halves its effective ridge penalty.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The one-variable constraint is $\beta^2\leq t$, an interval whose endpoints expand as $\sqrt t$. The duplicated constraint is the disk $\beta_1^2+\beta_2^2\leq t$; the loss contours are parallel strips perpendicular to $(1,1)$. Their first contact with the disk lies on $\beta_1=\beta_2$. Equivalently, the fitted total coefficient is the least-squares coefficient clipped to $[-\sqrt{2t},\sqrt{2t}]$, compared with $[-\sqrt t,\sqrt t]$ for one copy.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The two [Lasso](../../../probability-and-statistics.md#lasso) problems are

$$
\min_\beta\lVert Y-x\beta\rVert_2^2\quad\text{subject to }|\beta|\leq t
$$

and

$$
\min_{\beta_1,\beta_2}\lVert Y-x(\beta_1+\beta_2)\rVert_2^2
\quad\text{subject to }|\beta_1|+|\beta_2|\leq t.
$$

If $\widehat\beta$ solves the first problem, the complete solution set of the second is

$$
\boxed{\{(\beta_1,\beta_2):\beta_1+\beta_2=\widehat\beta,\ 
|\beta_1|+|\beta_2|\leq t\}}.
$$

Indeed, the feasible totals are exactly $[-t,t]$, the same as in the first problem.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The duplicated feasible set is the diamond $|\beta_1|+|\beta_2|\leq t$. A loss contour first touches an entire line segment of the diamond whenever the optimal total has the sign of a sloping face; all points on that segment give the same fit. As $t$ passes the unconstrained optimum, the solution set becomes the intersection of the interior diamond with the line $\beta_1+\beta_2=z/s$.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

For prediction at covariate value $u$, the intercept contributes variance $\sigma^2/n$ in every case because $x$ is centered. The one-copy ridge shrinkage is $a_1=s/(s+\lambda)$, while the duplicated-design total has $a_2=2s/(2s+\lambda)$. Thus

$$
\operatorname{Bias}\widehat m_j(u)=u(a_j-1)\beta_0,
$$

and

$$
\operatorname{Var}\widehat m_1(u)=\frac{\sigma^2}{n}
+\frac{u^2\sigma^2s}{(s+\lambda)^2},
\qquad
\operatorname{Var}\widehat m_2(u)=\frac{\sigma^2}{n}
+\frac{4u^2\sigma^2s}{(2s+\lambda)^2}.
$$

Since $a_2>a_1$, duplication reduces ridge bias and increases variance.

For constrained Lasso, let $Z=z/s\sim N(\beta_0,\sigma^2/s)$ and $C_t(Z)=\max(-t,\min(Z,t))$. Both designs have the identical fitted total $C_t(Z)$, so both have

$$
\operatorname{Bias}\widehat m(u)=u\{\mathbb EC_t(Z)-\beta_0\},
\qquad
\operatorname{Var}\widehat m(u)=\frac{\sigma^2}{n}+u^2\operatorname{Var}\{C_t(Z)\}.
$$

Duplicating the predictor has no effect on Lasso predictions, despite making the coefficient vector nonunique.

## 2

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For user $j$ and offer $r$, both fits use

$$
\operatorname{logit}(p_j)=\beta_0+\beta_1\operatorname{age}_j+\beta_2\operatorname{fitness}_j
+\gamma_{\operatorname{region}_j}+\delta_{\operatorname{sex}_j}.
$$

The first model treats each click as Bernoulli$(p_j)$. The grouped model treats the click count $C_j=m_j\operatorname{prop}_j$ as $\operatorname{Bin}(m_j,p_j)$. Their likelihoods differ only by binomial coefficients independent of the parameters, so their fitted coefficients agree.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The grouped binomial likelihood assumes conditional independence of repeated offers to one user. This is doubtful: persistent unmeasured user preferences and temporal feedback make clicks from the same user positively correlated.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For $m_j$ exchangeable Bernoulli responses of mean $p_j$ and pairwise correlation $\rho$,

$$
\mathbb E\widehat p_j=p_j,\qquad
\operatorname{Var}(\widehat p_j)
=\frac{p_j(1-p_j)}{m_j}\{1+(m_j-1)\rho\}.
$$

A standard quasi-binomial model uses a common dispersion multiplier $\phi$. It cannot represent this variance simultaneously when the offer counts $m_j$ vary, because the multiplier $1+(m_j-1)\rho$ then varies by user.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The beta-binomial regression is

$$
P_j\sim\operatorname{Beta}(\mu_j,\theta),\qquad
C_j\mid P_j\sim\operatorname{Bin}(m_j,P_j),
\qquad
\operatorname{logit}(\mu_j)=z_j^T\beta,
$$

where the beta distribution is parameterized by mean $\mu_j$ and variance parameter $\theta$. Marginally,

$$
\operatorname{Var}(C_j/m_j)
=\frac{\mu_j(1-\mu_j)}{m_j}
\left\{1+(m_j-1)\frac{\theta}{1+\theta}\right\}.
$$

It matches part c when $\rho=\theta/(1+\theta)$, so it is appropriate at the mean-variance level for a common nonnegative intraclass correlation.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

The beta-binomial model mixes binomials over a beta-distributed success probability. The random-intercept generalized linear mixed model instead takes

$$
\operatorname{logit}(P_j)=z_j^T\beta+b_j,\qquad b_j\sim N(0,\tau^2).
$$

Both create within-user dependence and overdispersion, but use different mixing distributions. The mixed-model coefficients are conditional on the random effect, while beta-binomial regression is naturally phrased through a marginal mean.

## 3

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Time is exposure: doubling the public duration should double the expected count without changing the viewing rate. Modeling the rate is therefore preferable to treating time as an additive linear predictor. In a [Poisson regression](../../../statistical-modelling.md#poisson-regression) the exact implementation should be

$$
\log\mathbb E(N_i)=\log t_i+\beta_0+\beta_1I_i,
$$

using $\log t_i$ as an offset; directly supplying noninteger $N_i/t_i$ without exposure weights is not generally likelihood-equivalent.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

[Overdispersion](../../../exponential-family.md#overdispersion) means that conditional variance exceeds the Poisson mean. Under a correctly specified Poisson model, the Pearson statistic is approximately chi-squared with $149$ residual degrees of freedom. Here

$$
X^2=149(1.3119)\simeq195.5,\qquad
\frac{X^2-149}{\sqrt{2(149)}}\simeq2.69>1.645,
$$

so a one-sided five-percent test rejects. The displayed model-based confidence interval is too narrow. A quasi-Poisson fit can multiply standard errors by $\sqrt{1.3119}$; [negative binomial regression](../../../statistical-modelling.md#negative-binomial-regression) or a random-effects count model can model the extra variation directly.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

There is one row per video. Giving every video its own categorical coefficient saturates the linear predictor. The investment column is a linear combination of the video indicator columns, so the design matrix loses full rank and the investment effect can be shifted into the video effects without changing any fitted value. The model is nonidentifiable.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Fit the exposure-offset Poisson model

$$
N_i\sim\operatorname{Poisson}\{t_i\exp(\beta_0+\beta_1I_i+\gamma_{g_i})\}.
$$

For a new video with investment $I$ and genre $g$, put $\mu=90\exp(\beta_0+\beta_1I+\gamma_g)$, compute

$$
\mathbb P_\mu(N\leq9999),\quad
\mathbb P_\mu(10000\leq N\leq49999),\quad
\mathbb P_\mu(N\geq50000),
$$

and select the largest. For fixed genre these probabilities are nonlinear functions of investment, so this is a nonlinear classifier.

## 4

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For hidden layers $h^{(r)}=\phi_r(W_rh^{(r-1)}+b_r)$ with $h^{(0)}=x$, the output logits are $z=W_{R+1}h^{(R)}+b_{R+1}$ and the [softmax function](../../../statistical-learning.md#softmax-function) gives

$$
\boxed{p_\ell(x)=\frac{e^{z_\ell}}{\sum_{j=1}^Le^{z_j}}.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Multinomial [logistic regression](../../../statistical-modelling.md#logistic-regression) is the network with no hidden layer: $z=Wx+b$ followed by softmax. Binary logistic classification uses one logit $w^Tx+b$ followed by the sigmoid function.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Deep sigmoid networks suffer from vanishing gradients because derivatives become small in saturated units and multiply across layers. The [ReLU](../../../statistical-learning.md#rectified-linear-unit) has derivative one on its positive half-line and therefore propagates gradients more effectively there.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

For all weights and biases collected in $\vartheta$, fit

$$
\min_\vartheta\left\{
-\sum_{i=1}^n\sum_{\ell=1}^LY_{i\ell}\log p_\ell(x_i;\vartheta)
+\lambda_1\lVert\vartheta\rVert_1+\lambda_2\lVert\vartheta\rVert_2^2
\right\}.
$$

Use backpropagation with stochastic gradient descent or a modern adaptive variant, treating the absolute-value derivative at zero as stated. Select $(\lambda_1,\lambda_2)$ by validation or cross-validation and refit using the selected pair.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

A dead ReLU unit has nonpositive preactivation for every training input, so its output and gradient are always zero. Replace $\max(0,z)$ by the leaky ReLU

$$
\phi_a(z)=\max(z,az),\qquad0<a<1.
$$

Its negative-side derivative $a$ permits recovery while it remains nonsaturating, preserving the gradient advantage over sigmoid activation.

## 5

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For $\eta(x)=\mathbb P(Y=1\mid X=x)$, the risk is

$$
R(\psi)=\mathbb P\{\psi(X)\ne Y\}.
$$

The [Bayes classifier](../../../statistical-inference.md#bayes-classifier) is $\psi^{\mathrm{Bayes}}(x)=\mathbf1_{\{\eta(x)\geq1/2\}}$, with risk $\mathbb E\min\{\eta(X),1-\eta(X)\}$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The [K-nearest neighbors algorithm](../../../statistical-learning.md#k-nearest-neighbors-algorithm) takes the majority label among the $k$ training features closest to the query, with a stated tie rule. Its data-dependent risk is the conditional test error given the training sample, and $R_n$ denotes its expectation over that sample.

For one nearest neighbour, condition on a feature value $X=x$ and couple the coincident nearest feature as $X_1=x$. The two labels are conditionally independent Bernoulli$(\eta(x))$, so their mismatch probability is

$$
2\eta(x)\{1-\eta(x)\}
\leq2\min\{\eta(x),1-\eta(x)\}.
$$

Integration over $X$ gives

$$
\boxed{R_n(\psi^{1\mathrm{NN}})\leq2R(\psi^{\mathrm{Bayes}}).}
$$

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

For each $k=1,\ldots,100$, the call to knn.cv performs leave-one-out nearest-neighbour classification and the third line stores the fraction of omitted observations misclassified. Choose a minimizer of ls, then fit the nearest-neighbour classifier with that $k$ to the full data.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

A weighted nearest-neighbours classifier predicts one when

$$
\sum_{i=1}^kw_iY_{(i)}\geq\frac12,
\qquad w_i\geq0,\quad\sum_iw_i=1,
$$

where neighbours are distance ordered. Under the usual smooth-density and smooth-regression assumptions, asymptotically optimal weights downweight distant neighbours, for example normalized positive parts of $1-(i/k)^{2/p}$. The optimal weighted-nearest-neighbour theorem gives smaller leading asymptotic regret than equal weights.

## 6

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

A [weakly stationary process](../../../time-series.md#weakly-stationary-process) has a constant finite mean and covariance $\operatorname{Cov}(X_t,X_{t+h})$ depending only on lag $h$. The plotted process is not stationary: it has a declining trend and a pronounced oscillation of period about $25$, so its mean depends on time.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Fit a trend $\widehat T_t$, form $D_t=X_t-\widehat T_t$, and estimate the period-25 seasonal effect by

$$
\widehat S_j=\frac1M\sum_{r=0}^{M-1}D_{j+25r},
\qquad j=1,\ldots,25.
$$

The residual is $R_t=X_t-\widehat T_t-\widehat S_{t\bmod25}$. This additive decomposition is sensible when seasonal amplitude does not systematically change with the level or trend; multiplicative seasonality would require a logarithmic transform or ratio decomposition.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

A period-50 business cycle can be a stochastic cycle in the residual process and need not violate additive trend-plus-period-25 seasonality. Applying $1-B^{50}$ discards the first 50 of only 100 observations and introduces a noninvertible seasonal moving-average factor, creating strong artificial dependence and risking overdifferencing rather than modeling the cycle.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

The sample autocorrelation has one substantial positive spike at lag one and then cuts off, while the partial autocorrelation tails off with alternating signs. This is the characteristic pattern of a [moving-average process of order one](../../../time-series.md#moving-average-process-of-order-one).

<h3 id="6/e">e</h3>

↑ **Parent:** [6](#6)

<h4 id="6/e/solution">Solution</h4>

↑ **Parent:** [E](#6/e)

The first line searches candidate ARIMA models and selects the one with smallest [Akaike information criterion](../../../statistical-modelling.md#akaike-information-criterion). The second constructs a one-step-ahead point forecast and nominal 95-percent prediction interval from the fitted values of the selected model.

<h3 id="6/f">f</h3>

↑ **Parent:** [6](#6)

<h4 id="6/f/solution">Solution</h4>

↑ **Parent:** [F](#6/f)

The interval treats the selected model and estimated detrending and seasonal components as fixed, often assumes approximately Gaussian homoscedastic innovations, and ignores model-selection and parameter uncertainty. With only 100 observations these omissions can materially reduce coverage. A residual or parametric [bootstrap](../../../statistical-modelling.md#bootstrapping-statistics) that repeats decomposition, model selection, fitting, and forecasting can propagate those sources of uncertainty; time-series cross-validation can additionally assess empirical one-step coverage.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
