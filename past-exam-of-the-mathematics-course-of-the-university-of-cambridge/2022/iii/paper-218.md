# Paper 218

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_218.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_218.pdf)

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
  - [d](#4/d)
    - [Solution](#4/d/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [i](#5/c/i)
      - [Solution](#5/c/i/solution)
    - [ii](#5/c/ii)
      - [Solution](#5/c/ii/solution)
    - [iii](#5/c/iii)
      - [Solution](#5/c/iii/solution)
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

## 1

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Put $\phi=1/\gamma$ and $\theta=-1/\alpha$. The density can be written

$$
f(y;\theta,\phi)
=\exp\left[
\frac{y\theta-b(\theta)}{\phi}+c(y,\phi)
\right],
\qquad
b(\theta)=-\log(-\theta),
$$

where

$$
c(y,\phi)
=-\log\Gamma(1/\phi)-\phi^{-1}\log\phi
+(\phi^{-1}-1)\log y.
$$

Thus this is an [exponential dispersion family](../../../exponential-family.md#exponential-dispersion-model). Its derivative identities give

$$
\mathbb EY=b'(\theta)=-\frac1\theta=\alpha,
\qquad
\operatorname{Var}(Y)=\phi b''(\theta)
=\phi\alpha^2=\frac{\alpha^2}{\gamma}.
$$

The [variance function](../../../exponential-family.md#variance-function) is $V(\mu)=\mu^2$. In the usual Gamma-GLM convention the canonical inverse link is

$$
g(\mu)=\frac1\mu;
$$

it differs by a minus sign from the natural parameter $\theta=-1/\mu$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $x_i^T$ be row $i$ of the design matrix, $\eta_i=x_i^T\beta=1/\mu_i$, and $\gamma=1/\phi$. The full [log-likelihood](../../../statistical-modelling.md#log-likelihood) is

$$
\ell(\beta,\gamma)
=\sum_{i=1}^{61}
\left\{
\gamma\log\gamma+\gamma\log\eta_i-\log\Gamma(\gamma)
+(\gamma-1)\log y_i-\gamma y_i\eta_i
\right\}.
$$

Differentiation gives the [score function](../../../statistical-modelling.md#informant-function)

$$
\nabla_\beta\ell
=\gamma X^T(\mu-Y),
\qquad
\mu_i=\eta_i^{-1},
$$

and

$$
-\nabla_\beta^2\ell
=\gamma X^T\operatorname{diag}(\mu_i^2)X.
$$

The Hessian does not depend on $Y$, so the [Fisher information matrix](../../../statistical-modelling.md#fisher-information-matrix) is

$$
\boxed{\mathcal I_\beta
=\frac1\phi X^TWX,
\qquad
W=\operatorname{diag}(\mu_i^2).}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The score equation $X^T(\mu-Y)=0$ is independent of $\gamma$, because $\gamma>0$ is only a common factor. Fixing $\phi=1$ or estimating it therefore gives the same [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator) $\widehat\beta$.

Under the usual full-rank and regularity conditions,

$$
\widehat\beta
\mathrel{\dot\sim}
N_4\!\left(
\beta,\,
\phi(X^TWX)^{-1}
\right),
$$

with $W$ evaluated consistently at the fitted means. Consequently every standard error from "mod2" is $\sqrt{\widehat\phi}$ times the corresponding standard error computed with dispersion one in "mod1". In particular,

$$
\boxed{\operatorname{SE}_{\rm mod2}(\widehat\beta_{\rm posout})
=\sqrt{0.3103711}\,(0.04556).}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The null hypothesis is

$$
H_0:\beta_{\rm type2}=\beta_{\rm type3}
=\beta_{\rm posout}=0,
$$

against the alternative that at least one coefficient is nonzero. The code uses the scaled reduction in [exponential-family deviance](../../../exponential-family.md#exponential-family-deviance),

$$
T=\frac{21.061-18.185}{0.31},
$$

and compares it with $\chi_3^2$.

That chi-squared calibration is appropriate when the dispersion is known, and is asymptotically valid after consistent dispersion estimation. With unknown Gamma dispersion, the standard finite-sample GLM comparison instead uses

$$
F=\frac{(21.061-18.185)/3}{0.3103711}
$$

against an $F_{3,57}$ distribution. Its p-value is approximately $0.034$, so the correctly calibrated test still rejects at the 5% level and gives evidence that component type or position contributes to mean failure time.

## 2

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

First recode the labels as $y_i=2Y_i-1\in\{-1,1\}$; with labels $0$ and $1$, the displayed constraints for class zero can never hold. Add an unpenalized intercept $b$ so that the separating hyperplane need not pass through the origin, and solve

$$
\min_{b,\beta}\frac12\|\beta\|_2^2
\quad\text{subject to}\quad
y_i(b+X_i^T\beta)\geq1.
$$

Centering and scaling predictor columns is also advisable because the Euclidean penalty depends on their units.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [support vector machine](../../../statistical-learning.md#support-vector-machine) classifier is

$$
\widehat C(x)=\mathbf1_{\{\widehat b+x^T\widehat\beta\geq0\}}.
$$

Under the constraints, the two classes lie beyond the parallel [support-vector-machine margin boundaries](../../../statistical-learning.md#support-vector-machine-margin-boundaries) $b+x^T\beta=\pm1$. Their distance is $2/\|\beta\|_2$, so minimizing the norm maximizes the geometric margin. The observations touching the margin are the [support vectors](../../../statistical-learning.md#support-vector).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The hard-margin constraints are feasible exactly when the classes are separated by a [separating hyperplane](../../../statistical-learning.md#separating-hyperplane). Failure after the corrections in part a therefore means the classes overlap.

Introduce [slack variables of a support vector machine](../../../statistical-learning.md#slack-variables-of-a-support-vector-machine) and solve the soft-margin problem

$$
\min_{b,\beta,\xi}
\left\{\frac12\|\beta\|_2^2+C\sum_i\xi_i\right\}
$$

subject to

$$
y_i(b+X_i^T\beta)\geq1-\xi_i,
\qquad \xi_i\geq0.
$$

Large $C$ strongly penalizes violations and approaches the hard-margin solution when separation is possible. Small $C$ tolerates more violations in exchange for a wider, more strongly regularized margin.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The [kernel trick](../../../probability-and-statistics.md#kernel-trick) replaces inner products $\phi(x_i)^T\phi(x_j)$ by evaluations of a [positive-semidefinite kernel](../../../probability-and-statistics.md#positive-semidefinite-kernel) $k(x_i,x_j)$ without explicitly constructing the feature vectors. In the corresponding reproducing-kernel Hilbert space, the hard-margin problem is

$$
\min_{b,f\in\mathcal H}\frac12\|f\|_{\mathcal H}^2
\quad\text{subject to}\quad
y_i\{b+f(X_i)\}\geq1.
$$

Equivalently, its dual is

$$
\max_{\alpha_i\geq0}
\left\{
\sum_i\alpha_i
-\frac12\sum_{i,j}\alpha_i\alpha_jy_iy_jk(X_i,X_j)
\right\},
\qquad
\sum_i\alpha_iy_i=0.
$$

There is no upper bound $\alpha_i\leq C$ because this is the hard-margin, rather than soft-margin, problem.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

The successful hard-margin fit proves that the transformed observations are separable. This creates [complete separation](../../../statistical-modelling.md#complete-separation) in unpenalized [logistic regression](../../../statistical-modelling.md#logistic-regression): scaling a separating coefficient vector continually raises the likelihood, so no finite maximum-likelihood estimate exists. The nearly singular observed information produces the enormous reported standard errors.

A ridge-penalized logistic regression, or equivalently a Bayesian logistic model with a proper Gaussian prior, gives finite, stable coefficients. Firth bias reduction is another standard remedy.

## 3

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For word-count vector $x$, the fitted [logistic model](../../../statistical-modelling.md#logistic-model) is

$$
\log\frac{\widehat p(x)}{1-\widehat p(x)}
=-5.391451+1.859318x_{\rm dollar}
+5.680691x_{\rm winner}+0.923072x_{\rm password}
-6.890095x_{\rm edu}+2.269523x_{\rm credit}
$$



$$
{}+1.198028x_{\rm discount}-3.176676x_{\rm as}
-1.866328x_{\rm I}+4.347929x_{\rm fun}
+0.864456x_{\rm trial}.
$$

Holding other counts fixed, one additional occurrence of "dollar" multiplies the fitted spam odds by $e^{1.859318}$.

The logistic classifier is

$$
\widehat C^{\rm logit}(x)
=\mathbf1_{\{\widehat p(x)>1/2\}}
=\mathbf1_{\{\widehat\beta_0+x^T\widehat\beta>0\}}.
$$

The coefficients maximize the [Bernoulli logistic-regression model](../../../statistical-modelling.md#bernoulli-logistic-regression-model) likelihood over the training emails.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [decision boundary](../../../statistical-learning.md#decision-boundary) is the hyperplane

$$
\widehat\beta_0+x^T\widehat\beta=0.
$$

At threshold $q$ the classifier predicts spam when

$$
\widehat\beta_0+x^T\widehat\beta
>\log\frac q{1-q},
$$

so $q=1/2$ gives the original classifier. Varying $q$ translates the boundary parallel to itself: raising $q$ shrinks the region classified as spam and generally trades fewer false positives for more false negatives.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Writing $\eta_i=\beta_0+x_i^T\beta$, the [log-likelihood](../../../statistical-modelling.md#log-likelihood) is

$$
\ell(\beta_0,\beta)
=\sum_{i=1}^n
\left\{y_i\eta_i-\log(1+e^{\eta_i})\right\}.
$$

With 500 observations and 5000 word predictors, the augmented design matrix cannot have full column rank. There are nonzero coefficient directions that leave every $\eta_i$ unchanged, so any maximizer belongs to an affine family and is not unique. In addition, the high-dimensional features may completely separate the classes, in which case no finite maximizer exists at all.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

[Principal component analysis](../../../statistical-learning.md#principal-component-analysis) centers the word-count vectors, diagonalizes their sample [covariance matrix](../../../variance.md#covariance-matrix), and projects onto the eigenvectors with the largest eigenvalues. Fitting logistic regression to $d<n$ principal-component scores removes exact collinearity and yields a lower-dimensional design.

Each principal component is an unsupervised linear combination of many words chosen to explain predictor variance; it is not a word selected for association with spam. The dimension can be chosen from a scree plot or cumulative explained variance, but cross-validating the downstream classification loss better targets prediction.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

For fixed $A$, differentiating under the constraint $\sum_i z_i=0$ gives

$$
\widehat\mu=\overline X,
\qquad
\widehat z_i=(A^TA)^{-1}A^T(X_i-\overline X).
$$

Because the columns $u_j$ are orthogonal,

$$
\widehat z_{ij}
=\frac{u_j^T(X_i-\overline X)}{\|u_j\|_2^2}.
$$

The fitted value is therefore $\overline X+\Pi_A(X_i-\overline X)$, where $\Pi_A$ is the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) onto the column space of $A$.

The residual sum of squares is minimized by choosing this column space to be the span of the $d$ leading eigenvectors of

$$
\sum_i(X_i-\overline X)(X_i-\overline X)^T.
$$

**Thus $\widehat A$ may be taken to have those orthonormal eigenvectors as columns. Their nonzero scales are immaterial because inverse scaling of the scores leaves $Az_i$ unchanged.**

## 4

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For student $i$ in school $j$, "lme1" is the [random-intercept linear mixed model](../../../statistical-modelling.md#random-intercept-linear-mixed-model)

$$
\operatorname{THK}_{ij}
=\beta_0+\beta_1\operatorname{PTHK}_{ij}
+\beta_2\operatorname{TV}_j+\beta_3\operatorname{SC}_j
+b_j+\varepsilon_{ij},
$$

where

$$
b_j\overset{\rm iid}\sim N(0,\tau^2),
\qquad
\varepsilon_{ij}\overset{\rm iid}\sim N(0,\sigma^2),
$$

independently. The estimates are

$$
(\widehat\beta_0,\widehat\beta_1,\widehat\beta_2,\widehat\beta_3)
=(1.78880,0.30973,0.02175,0.47023),
$$



$$
\widehat\tau^2=0.0437,
\qquad
\widehat\sigma^2=1.6531.
$$

The fixed intercept is the population-average expected post-study score for an untreated reference student with PTHK zero. The random intercept $b_j$ is school $j$'s deviation from that population intercept.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Treatment was assigned by school, so observations within one school are [clustered data](../../../statistical-modelling.md#clustered-data) and plausibly correlated. A [random intercept](../../../statistical-modelling.md#random-intercept) models shared unobserved school characteristics and prevents the effective amount of treatment-level information from being exaggerated by treating all students as independent.

The fitted school standard deviation is $0.209$, so the estimated between-school variation is nonzero. Accounting for it raises the TV and SC standard errors from about $0.065$ in "lm1" to about $0.105$ in "lme1", reflecting that only 28 independently randomized schools identify those effects.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Conditionally on the school effect, the response variance is $\widehat\sigma^2=1.6531$. Marginally,

$$
\widehat{\operatorname{Var}}(\operatorname{THK}_{ij})
=\widehat\tau^2+\widehat\sigma^2
=0.0437+1.6531,
$$

and two distinct students in the same school have estimated covariance $0.0437$.

There is no single coefficient estimate for the random effect because the 28 school deviations are modeled as draws from a mean-zero distribution. The summary reports the estimated distributional variance; individual empirical Bayes predictions can be extracted separately.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Model "lme2" replaces $b_j$ by a random intercept and random PTHK slope:

$$
\operatorname{THK}_{ij}
=x_{ij}^T\beta+b_{0j}+b_{1j}\operatorname{PTHK}_{ij}
+\varepsilon_{ij},
$$

with a fitted bivariate normal covariance matrix for $(b_{0j},b_{1j})$. This adds a random-slope variance and an intercept-slope covariance.

The likelihood-ratio statistic is

$$
2\{-2680.4-(-2684.6)\}=8.4.
$$

An ordinary chi-squared reference is unreliable because the null random-slope variance is on the boundary and its correlation is unidentified there; the reported correlation of one also signals a nearly singular fit. A valid practical test is a [parametric bootstrap](../../../statistical-modelling.md#parametric-bootstrap): simulate many datasets from fitted "lme1", refit both models by maximum likelihood to each, recompute the likelihood-ratio statistic, and estimate the p-value by the fraction at least $8.4$. The AIC favors "lme2" slightly, whereas its BIC is larger, so the descriptive criteria do not agree.

## 5

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For a model with $k$ fitted parameters and maximized likelihood $L(\widehat\theta)$, the [Akaike information criterion](../../../statistical-modelling.md#akaike-information-criterion) is

$$
\operatorname{AIC}=-2\log L(\widehat\theta)+2k.
$$

Backward selection starts with the full model, deletes the single variable giving the smallest AIC when that AIC is lower than the current value, and repeats until no deletion improves it. The first deletion is "indus", which gives AIC $1597.8$.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Adding variables can reduce training bias and increase the maximized likelihood, but it also increases estimation variance and optimism. The $2k$ penalty estimates this optimism, so minimizing AIC implements a [bias-variance tradeoff](../../../statistical-modelling.md#bias-variance-tradeoff) aimed at expected out-of-sample Kullback–Leibler performance.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/i">i</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/i/solution">Solution</h5>

↑ **Parent:** [I](#5/c/i)

For $Y\sim N_n(X\beta,\sigma^2I)$,

$$
\ell(\beta,\sigma^2)
=-\frac n2\log(2\pi)-\frac n2\log\sigma^2
-\frac1{2\sigma^2}\|Y-X\beta\|_2^2.
$$

<h4 id="5/c/ii">ii</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/c/ii)

At the maximum-likelihood estimates,

$$
\widehat\sigma_1^2=\frac1n\|Y-X\widehat\beta\|_2^2,
$$

so

$$
-2\ell(\widehat\beta,\widehat\sigma_1^2)
=n\{\log(2\pi\widehat\sigma_1^2)+1\}.
$$

There are $p$ regression coefficients and one variance parameter. Adding twice this parameter count gives

$$
\boxed{\operatorname{AIC}(M_1)
=n\{\log(2\pi\widehat\sigma_1^2)+1\}+2(p+1).}
$$

<h4 id="5/c/iii">iii</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/c/iii)

The common terms cancel, and

$$
\operatorname{AIC}(M_2)-\operatorname{AIC}(M_1)
=n\log\frac{\widehat\sigma_2^2}{\widehat\sigma_1^2}+2q.
$$

This is negative exactly when

$$
\boxed{\frac{\widehat\sigma_2^2}{\widehat\sigma_1^2}<e^{-2q/n}.}
$$

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

There are three regression coefficients and $97$ residual degrees of freedom, so $n=100$. The reported residual standard error uses the unbiased divisor:

$$
\operatorname{RSS}=97(1.359)^2.
$$

**Hence the maximum-likelihood variance estimate is $\widehat\sigma^2=\operatorname{RSS}/100$. Substituting this, $n=100$, and the four fitted parameters—three coefficients plus $\sigma^2$—into the formula in part c(ii) gives the AIC.**

## 6

↑ **Parent:** [Paper 218](paper-218.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

The prior is

$$
\beta_1,\beta_2\overset{\rm iid}\sim N(0,1).
$$

The software samples from the [Bayesian posterior](../../../statistical-inference.md#bayesian-posterior); the displayed "Estimate" values are posterior means computed from the Markov-chain Monte Carlo draws.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

With unit error variance, the [Gaussian likelihood](../../../statistical-modelling.md#gaussian-likelihood) has log-likelihood

$$
\ell(\beta)
=-\frac n2\log(2\pi)-\frac12\|Y-X\beta\|_2^2.
$$

Full column rank gives $\widehat\beta=(X^TX)^{-1}X^TY$ and the least-squares identity

$$
\|Y-X\beta\|_2^2
=\|Y-X\widehat\beta\|_2^2
+(\beta-\widehat\beta)^TX^TX(\beta-\widehat\beta).
$$

Multiplying the likelihood by $\prod_j\phi(\beta_j)$ and absorbing all terms independent of $\beta$ into $C$ gives

$$
\boxed{\pi(\beta\mid Y)
=C\exp\left[
-\frac12(\beta-\widehat\beta)^TX^TX(\beta-\widehat\beta)
+\sum_{j=1}^p\log\phi(\beta_j)
\right].}
$$

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

For a Laplace prior $\phi(u)\propto e^{-\lambda|u|}$, maximizing the posterior is equivalent to minimizing

$$
\frac12\|Y-X\beta\|_2^2+\lambda\|\beta\|_1,
$$

so the posterior mode is the [Lasso](../../../probability-and-statistics.md#lasso). For a Gaussian prior $\phi(u)\propto e^{-\lambda u^2/2}$, the mode minimizes

$$
\frac12\|Y-X\beta\|_2^2+\frac\lambda2\|\beta\|_2^2
$$

and is the [ridge regression](../../../linear-regression.md#ridge-regression) estimator $(X^TX+\lambda I)^{-1}X^TY$. Gaussian conjugacy makes the posterior normal, so its mode and [posterior mean](../../../statistical-inference.md#posterior-mean) coincide at this ridge estimate.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

The nearly identical predictor columns create severe [multicollinearity](../../../statistical-modelling.md#multicollinearity). Their sum is well identified, as shown by the excellent fitted response, but their difference is weakly identified, allowing ordinary least squares to choose huge opposite coefficients with huge standard errors. The independent $N(0,1)$ priors impose the ridge penalty from part c, shrinking that unstable difference toward zero and producing the stable estimates near $(1,1)$.

<h3 id="6/e">e</h3>

↑ **Parent:** [6](#6)

<h4 id="6/e/solution">Solution</h4>

↑ **Parent:** [E](#6/e)

The reported 95% [credible interval](../../../statistical-inference.md#credible-interval) for $\beta_1$ is

$$
[-0.33,\,2.37].
$$

Conditional on the model, prior, and observed data, its posterior probability is 0.95. A frequentist 95% [confidence interval](../../../statistical-inference.md#confidence-interval) instead has 95% coverage under repeated sampling before the data are observed; it does not assign a sampling probability to the fixed parameter after observing this dataset.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
