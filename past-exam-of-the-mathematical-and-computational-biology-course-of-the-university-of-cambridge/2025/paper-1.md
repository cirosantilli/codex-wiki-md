# Paper 1

↑ **Parent:** [2025](../2025.md)

[Original paper, released PDF pages 114–125](https://www.whatdotheyknow.com/request/past_exam_information_of_nst_ib_2/response/3538010/attach/2/FOI%202026%20642%20Cui%20materials%20Part2.pdf?cookie_passthrough=1#page=114)

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
  - [g](#3/g)
    - [Solution](#3/g/solution)
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
  - [f](#4/f)
    - [Solution](#4/f/solution)
  - [g](#4/g)
    - [Solution](#4/g/solution)
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
  - [f](#5/f)
    - [Solution](#5/f/solution)
  - [g](#5/g)
    - [Solution](#5/g/solution)
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
  - [g](#6/g)
    - [Solution](#6/g/solution)
- [7](#7)
  - [a](#7/a)
    - [Solution](#7/a/solution)
  - [b](#7/b)
    - [Solution](#7/b/solution)
  - [c](#7/c)
    - [Solution](#7/c/solution)
  - [d](#7/d)
    - [Solution](#7/d/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

It tests whether the input [string](../../foundations-of-mathematics.md#string) is a [palindrome](../../foundations-of-mathematics.md#palindrome): reversing the characters leaves the [string](../../foundations-of-mathematics.md#string) unchanged. Comparisons are case-sensitive and include spaces and punctuation. For example, `mystery1("level")` returns **`True`**, whereas `mystery1("lever")` returns **`False`**.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

It performs a [trial division](../../prime-number.md#trial-division) test for a [prime number](../../prime-number.md). An [integer](../../integer.md) below $2$ is rejected; otherwise the function searches for a [divisor](../../divisibility.md#divisor) from $2$ through $\lfloor\sqrt n\rfloor$. A [composite number](../../number-theory.md#composite-number) has a [prime factor](../../prime-number.md#prime-factor) no larger than its [square root](../../algebra.md#square-root), so finding no such [divisor](../../divisibility.md#divisor) proves [primality](../../prime-number.md#primality). For example, `mystery2(97)` returns **`True`**, while `mystery2(91)` returns **`False`**, since $91=7\cdot13$.

This describes the intended mathematical test. For extremely large [integers](../../integer.md), the floating-point computation `n**0.5` can round or overflow; an implementation intended for arbitrary-size [integers](../../integer.md) should use an exact [integer square root](../../algebra.md#integer-square-root).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

It filters the first [list](../../data-structure.md#list-abstract-data-type) by membership in the second [list](../../data-structure.md#list-abstract-data-type), retaining the order and all repetitions of qualifying entries in the first [list](../../data-structure.md#list-abstract-data-type). For example, `mystery3([3, 1, 3, 2], [3, 4])` returns **`[3, 3]`**. Thus it is related to [set intersection](../../set.md#set-intersection), but its result is a [list](../../data-structure.md#list-abstract-data-type) and does not discard repeated elements.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

With its default argument and a nonnegative [integer](../../integer.md) input, it prints the decimal [digits](../../integer.md#numerical-digit) of $n$ in order, one per line. For example, `mystery4(407)` prints **`4`, then `0`, then `7`**. [Integer division](../../arithmetic.md#integer-division) removes the final [digit](../../integer.md#numerical-digit), [recursion](../../algorithm.md#recursion-computer-science) handles the preceding [digits](../../integer.md#numerical-digit), and the [remainder](../../integer.md#remainder) gives the final [digit](../../integer.md#numerical-digit). The function returns `None`.

There is a subtlety for a nondefault base: the recursive call omits `m`, so it resets to $10$. For $m\ge2$ and $n\ge m$, the actual output is the decimal [digits](../../integer.md#numerical-digit) of $\lfloor n/m\rfloor$, followed by the [remainder](../../integer.md#remainder) $n\bmod m$. For example, `mystery4(13, 2)` prints **`6`, then `1`**, rather than the binary [digits](../../integer.md#numerical-digit) of $13$. Passing `m` on to the recursive call would give a consistent base-$m$ [positional notation](../../integer.md#positional-notation). The interpretation as [digits](../../integer.md#numerical-digit) assumes $n\ge0$ and $m\ge2$; arbitrary [integer](../../integer.md) arguments need not satisfy those conditions.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Using the [probability density function](../../continuous-probability-distribution.md#probability-density-function) of the [Erlang distribution](../../continuous-probability-distribution.md#erlang-distribution), the [expected value](../../expected-value.md) is

$$
\mathbb E X=\theta^2\int_0^\infty x^2e^{-\theta x}\,dx
=\frac1\theta\int_0^\infty u^2e^{-u}\,du
=\boxed{\frac2\theta}.
$$

Here $u=\theta x$, and two applications of [integration by parts](../../calculus.md#integration-by-parts) give $\int_0^\infty u^2e^{-u}\,du=2\int_0^\infty ue^{-u}\,du=2$. The boundary terms vanish because [exponential decay](../../analysis.md#exponential-decay) dominates these powers.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Put $S=\sum_{i=1}^N x_i$. Since the observations are [independent random variables](../../random-variable.md#independent-random-variables), their joint [probability density function](../../continuous-probability-distribution.md#probability-density-function) is a product. Therefore the [likelihood function](../../maximum-likelihood-estimation.md#likelihood-function) and [log-likelihood](../../maximum-likelihood-estimation.md#log-likelihood) are

$$
\boxed{\mathcal L(\theta)=\theta^{2N}e^{-\theta S}\prod_{i=1}^N x_i},\qquad
\boxed{\ell(\theta)=2N\log\theta-\theta S+\sum_{i=1}^N\log x_i}.
$$

These expressions assume positive observed values, as occurs with [probability](../../probability-theory.md#probability) one under this continuous [Erlang distribution](../../continuous-probability-distribution.md#erlang-distribution).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The [score function](../../statistical-modelling.md#informant-function) and the [observed Fisher information](../../statistical-modelling.md#observed-fisher-information) are

$$
\ell'(\theta)=\frac{2N}{\theta}-S,\qquad
j(\theta)=-\ell''(\theta)=\frac{2N}{\theta^2}>0.
$$

Solving the [score equation](../../statistical-modelling.md#score-equation) gives the [maximum-likelihood estimate](../../maximum-likelihood-estimation.md#maximum-likelihood-estimator)

$$
\boxed{\widehat\theta=\frac{2N}{S}=\frac2{\bar x}}.
$$

The positive [observed Fisher information](../../statistical-modelling.md#observed-fisher-information) means that the [log-likelihood](../../maximum-likelihood-estimation.md#log-likelihood) is strictly [concave](../../real-analysis.md#concave-function) on $\theta>0$. Its unique [stationary point](../../calculus-of-variations.md#stationary-point) is therefore the global maximum. Equivalently, the [score function](../../statistical-modelling.md#informant-function) changes from positive to negative at this point. At the estimate, $j(\widehat\theta)=S^2/(2N)$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Test the [null hypothesis](../../statistical-hypothesis-test.md#null-hypothesis) $H_0:\theta_m=\theta_f=\theta$ against the [alternative hypothesis](../../statistical-hypothesis-test.md#alternative-hypothesis) that the two rate parameters differ. Under $H_0$, the pooled [maximum-likelihood estimate](../../maximum-likelihood-estimation.md#maximum-likelihood-estimator) is $\widehat\theta_0=16/36.8\simeq0.434783$. Under the alternative, the estimates are $\widehat\theta_m=8/22\simeq0.363636$ and $\widehat\theta_f=8/14.8\simeq0.540541$.

In the [likelihood-ratio test statistic](../../statistical-hypothesis-test.md#likelihood-ratio-test-statistic), the data-only terms cancel, and both fitted models have total $\widehat\theta S=16$. Consequently,

$$
T=2(\ell_1-\ell_0)
=16\log\frac{\widehat\theta_m\widehat\theta_f}{\widehat\theta_0^2}
=16\log\frac{36.8^2}{4(22)(14.8)}\simeq0.6245.
$$

The [alternative hypothesis](../../statistical-hypothesis-test.md#alternative-hypothesis) adds one parameter, so [Wilks theorem](../../statistical-inference.md#wilks-theorem) gives an approximate [chi-squared distribution](../../probability-distribution.md#chi-squared-distribution) with one [degree of freedom](../../classical-mechanics.md#degree-of-freedom). **Do not reject the common-rate model at the 5% level**, since $T<3.841$. The corresponding approximate [p-value](../../statistical-hypothesis-test.md#p-value) is $0.43$. The fitted [expected values](../../expected-value.md) are $5.5$ and $3.7$ days, but four observations per group supply little evidence that the underlying [expected values](../../expected-value.md) differ; failure to reject does not establish equality. The [chi-squared distribution](../../probability-distribution.md#chi-squared-distribution) calibration is asymptotic and should be treated cautiously for these small samples.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The vector of column [sample means](../../variance.md#sample-mean) is $\bar x=(1,3,2)$. Subtract it from each observation. The centred data matrix, with cell types in the original order, is

$$
\boxed{X_c=\begin{pmatrix}-1&-3&-2\\-1&1&-2\\-1&1&2\\3&1&2\end{pmatrix}}.
$$

Each column now has [sample mean](../../variance.md#sample-mean) zero.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Using divisor $n=4$, the [covariance matrix](../../variance.md#covariance-matrix) is

$$
\boxed{\Sigma=\frac14X_c^{\mathsf T}X_c=
\begin{pmatrix}3&1&2\\1&3&2\\2&2&4\end{pmatrix}}.
$$

For example, the first [variance](../../variance.md) is $(1+1+1+9)/4=3$, and the first-second [covariance](../../variance.md#covariance) is $(3-1-1+3)/4=1$. If “sample [covariance matrix](../../variance.md#covariance-matrix)” means the unbiased convention, use divisor $n-1=3$ instead: $S=(4/3)\Sigma$. This multiplies every [eigenvalue](../../linear-operator-theory.md#eigenvalue) by $4/3$ and leaves all [principal component loadings](../../statistical-learning.md#principal-component-loading) and explained-[variance](../../variance.md) fractions unchanged.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The total [variance](../../variance.md) is the [trace](../../linear-algebra.md#matrix-trace) $\operatorname{tr}\Sigma=10$. Retaining two original genes preserves the sum of their marginal [variances](../../variance.md); the largest choice includes the third gene and either of the first two, giving $4+3=7$. Thus the largest proportion is **70%**. This refers to retaining measured coordinates themselves, rather than replacing them by [linear combinations](../../vector-space.md#linear-combination) as in [principal component analysis](../../statistical-learning.md#principal-component-analysis).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The [eigenvector](../../linear-operator-theory.md#eigenvector) $(1,-1,0)^{\mathsf T}$ has [eigenvalue](../../linear-operator-theory.md#eigenvalue) $2$. On its [orthogonal complement](../../hilbert-space.md#orthogonal-complement), write vectors as $(a,a,c)^{\mathsf T}$. The [eigenvalue equation](../../linear-operator-theory.md#eigenvalue-equation) becomes

$$
\begin{pmatrix}4&2\\4&4\end{pmatrix}\binom ac=\lambda\binom ac,
\qquad (4-\lambda)^2-8=0.
$$

Hence the ordered [eigenvalues](../../linear-operator-theory.md#eigenvalue) of the [covariance matrix](../../variance.md#covariance-matrix) are $4+2\sqrt2$, $2$, and $4-2\sqrt2$. The first two [principal components](../../statistical-learning.md#principal-component) explain

$$
\boxed{\frac{(4+2\sqrt2)+2}{10}=\frac{3+\sqrt2}{5}\simeq88.28\%}
$$

of the total [variance](../../variance.md). The denominator is the sum of all [eigenvalues](../../linear-operator-theory.md#eigenvalue), which equals the [trace](../../linear-algebra.md#matrix-trace).

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The second-largest [eigenvalue](../../linear-operator-theory.md#eigenvalue) is $2$, with [eigenvector](../../linear-operator-theory.md#eigenvector) $(1,-1,0)^{\mathsf T}$. A unit [principal component loading](../../statistical-learning.md#principal-component-loading) is therefore

$$
\boxed{u_2=\frac1{\sqrt2}(1,-1,0)^{\mathsf T}}.
$$

It is [orthogonal](../../inner-product.md#orthogonal-vectors) to the first loading $u_1=(1,1,\sqrt2)^{\mathsf T}/2$. Either sign of a loading is equivalent, provided its [principal component scores](../../statistical-learning.md#principal-component-score) use the same sign convention.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

The centred observation for D is $d=(3,1,2)^{\mathsf T}$. Taking [inner products](../../inner-product.md) with the unit [principal component loadings](../../statistical-learning.md#principal-component-loading) gives its [principal component scores](../../statistical-learning.md#principal-component-score):

$$
\boxed{(u_1^{\mathsf T}d,u_2^{\mathsf T}d)=(2+\sqrt2,\sqrt2)}.
$$

Normalizing the loadings matters: a direction alone does not fix the scale of the [coordinates](../../vector-space.md#coordinate-linear-algebra).

<h3 id="3/g">g</h3>

↑ **Parent:** [3](#3)

<h4 id="3/g/solution">Solution</h4>

↑ **Parent:** [G](#3/g)

After subtracting the same training [sample mean](../../variance.md#sample-mean), E has vector $e=(1,-1,0)^{\mathsf T}$ and [principal component scores](../../statistical-learning.md#principal-component-score) $(0,\sqrt2)$. The difference from D lies entirely along the first [principal component](../../statistical-learning.md#principal-component). Its [Euclidean distance](../../topological-analysis.md#euclidean-distance) in the retained plane is

$$
\boxed{\sqrt{(2+\sqrt2)^2+(\sqrt2-\sqrt2)^2}=2+\sqrt2\simeq3.4142}.
$$

The new point must use the original centring and loadings; recomputing them with E included would change the question.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For observation $j$ of bird $i$ in year $t(i,j)$, a [Gaussian linear mixed model](../../generalized-linear-model.md#gaussian-linear-mixed-model) with crossed [random intercepts](../../generalized-linear-model.md#random-intercept) is

$$
Y_{ij}=\beta_0+\beta_1 a_{ij}+u_i+v_{t(i,j)}+\varepsilon_{ij},
\quad
u_i\sim N(0,\tau_b^2),\quad v_t\sim N(0,\tau_y^2),\quad
\varepsilon_{ij}\sim N(0,\sigma^2),
$$

where the $u_i$, $v_t$, and $\varepsilon_{ij}$ are mutually [independent random variables](../../random-variable.md#independent-random-variables). Here $a_{ij}$ is age, $\beta_0$ is the population intercept at age zero, and $\beta_1$ is the change in conditional [expected value](../../expected-value.md) per year of age. The $u_i$ capture persistent between-bird variation, the $v_t$ capture shared annual conditions, and the [regression residuals](../../probability-and-statistics.md#regression-residual) capture remaining observation-level variation. Two observations from the same bird share [covariance](../../variance.md#covariance) $\tau_b^2$; two from the same year share $\tau_y^2$, with both contributions present if both group labels agree. The model also assumes the [random effects](../../latent-variable.md#random-effect) are independent of the age covariate.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Conditional predictions for observed birds and years add their fitted [random intercepts](../../generalized-linear-model.md#random-intercept) to the fixed part of the [Gaussian linear mixed model](../../generalized-linear-model.md#gaussian-linear-mixed-model):

$$
\boxed{\widehat Y_{11,2012}=2.274+0.123(3)+0.383420+0.023624=3.050044},
$$



$$
\boxed{\widehat Y_{12,2014}=2.274+0.123(7)-0.426676-0.056633=2.651691}.
$$

These are predicted [expected values](../../expected-value.md), so they need not be [integers](../../integer.md). The first is likely more reliable: age three is within the displayed age range, whereas age seven requires [extrapolation](../../interpolation.md#extrapolation) beyond ages one to six. A quantitative comparison would need the [prediction intervals](../../statistical-inference.md#prediction-interval), including uncertainty in both fixed coefficients and [random effects](../../latent-variable.md#random-effect); the displayed coefficients alone do not supply them.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [deviance](../../exponential-family.md#exponential-family-deviance) entries are $-2\ell$ for these fitted models. The completed values are

$$
\boxed{D_0=318.00,\quad D_1=305.96,\quad T=D_0-D_1=12.04,\quad\mathrm{df}=1}.
$$

The [likelihood-ratio test](../../statistical-hypothesis-test.md#likelihood-ratio-test) compares a model with one age coefficient against its restriction $\beta_1=0$. Its small [p-value](../../statistical-hypothesis-test.md#p-value), approximately $0.000529$, supports a positive age association under the assumed [Gaussian linear mixed model](../../generalized-linear-model.md#gaussian-linear-mixed-model). Refitting with [maximum likelihood estimation](../../maximum-likelihood-estimation.md) is essential here: [restricted maximum likelihood](../../normal-linear-model.md#restricted-maximum-likelihood) values from models with different fixed-effect design matrices cannot be compared by this [likelihood-ratio test](../../statistical-hypothesis-test.md#likelihood-ratio-test).

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Yes. The [bootstrap confidence interval](../../statistical-modelling.md#bootstrap-confidence-interval) for the age coefficient, $(0.057060,0.193584)$, excludes zero and supports the same positive association. A well-implemented [parametric bootstrap](../../statistical-modelling.md#parametric-bootstrap) can give better finite-sample calibration than the asymptotic [likelihood-ratio test](../../statistical-hypothesis-test.md#likelihood-ratio-test), especially with only eleven year groups and estimated [variance components](../../generalized-linear-model.md#variance-component). Its advantage depends on simulating the full fitted [Gaussian linear mixed model](../../generalized-linear-model.md#gaussian-linear-mixed-model) and refitting correctly; resampling individual records as if they were independent would discard the grouping. A [bootstrap confidence interval](../../statistical-modelling.md#bootstrap-confidence-interval) is also not literally the same procedure as a bootstrap-calibrated test.

The bird-level [standard deviation](../../variance.md#standard-deviation) is appreciable, with interval $(0.436,0.720)$ hatchlings, whereas the year-level estimate is much less precise, with interval $(0.0195,0.333)$. The residual [standard deviation](../../variance.md#standard-deviation) is approximately $0.381$–$0.493$. Boundary fits in 23 of the 1000 replicates indicate that at least one fitted [variance component](../../generalized-linear-model.md#variance-component) sometimes reaches zero; the convergence warning should also be investigated before trusting the reported intervals. Neither the asymptotic test nor a model-based [bootstrap](../../statistical-modelling.md#bootstrapping-statistics) repairs incorrect response-distribution or mean-structure assumptions.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

“After accounting for bird identity and year using [random intercepts](../../generalized-linear-model.md#random-intercept), hatching success increased by an estimated **0.123 hatchlings per additional year of age** (95% [bootstrap confidence interval](../../statistical-modelling.md#bootstrap-confidence-interval) 0.057–0.194).”

This describes an observational association under the fitted [Gaussian linear mixed model](../../generalized-linear-model.md#gaussian-linear-mixed-model), rather than a causal age effect. The diagnostic assessment below is needed before treating this inferential statement as reliable.

<h3 id="4/f">f</h3>

↑ **Parent:** [4](#4)

<h4 id="4/f/solution">Solution</h4>

↑ **Parent:** [F](#4/f)

The [regression diagnostics](../../linear-regression.md#regression-diagnostics) raise concerns about the mean and [variance](../../variance.md) assumptions. The residual-versus-fitted smoother is curved rather than horizontal, and the scale-location plot suggests changing residual spread, contrary to [homoscedasticity](../../statistical-model.md#homoscedasticity). Diagonal bands are expected when an [integer](../../integer.md)-valued response is fitted by a continuous model, since each fixed response value gives $r=y-\widehat y$. They are not, by themselves, proof of a failed mean model. The residual [Q-Q plot](../../probability-and-statistics.md#q-q-plot) is broadly linear but has tail departures and unusual observations, so exact [normality](../../probability-distribution.md#normality-statistics) is questionable.

The [Cook's distance](../../normal-linear-model.md#cook-s-distance) plot identifies observations worth checking for recording errors and influence on the age estimate. A rough $4/n\simeq0.023$ screening threshold flags several points, but it is not an automatic deletion rule. Repeat the fit with and without influential observations as a sensitivity analysis and report material changes.

The bird [random intercept](../../generalized-linear-model.md#random-intercept) [Q-Q plot](../../probability-and-statistics.md#q-q-plot) has a pronounced upper-tail departure; the year plot is closer to a line, although eleven groups give little power to assess [normality](../../probability-distribution.md#normality-statistics). These plotted effects are estimated, shrunken [conditional mode of Gaussian random effects](../../generalized-linear-model.md#conditional-mode-of-gaussian-random-effects), not independent observed draws from the latent [normal distribution](../../probability-distribution.md#normal-distribution), so their appearance requires care.

The analysis is therefore provisional. Check a nonlinear age effect, the changing residual [variance](../../variance.md), dependence beyond the fitted [random intercepts](../../generalized-linear-model.md#random-intercept), and a response model appropriate for counts. If clutch size is known, a [binomial distribution](../../discrete-probability-distribution.md#binomial-distribution) model for hatched eggs out of available eggs may be more meaningful. A bootstrap from the existing Gaussian model cannot validate the assumptions questioned by these plots. Distinguishing within-bird ageing from between-bird differences would also strengthen interpretation.

<h3 id="4/g">g</h3>

↑ **Parent:** [4](#4)

<h4 id="4/g/solution">Solution</h4>

↑ **Parent:** [G](#4/g)

The [Poisson generalized linear mixed model](../../generalized-linear-model.md#poisson-generalized-linear-mixed-model) assumes conditionally [Poisson distributed](../../discrete-probability-distribution.md#poisson-distribution) counts with a [log link](../../generalized-linear-model.md#logarithmic-link-function). The fitted [variance components](../../generalized-linear-model.md#variance-component) are both zero, so this fit lies on a boundary and reduces to ordinary [Poisson regression](../../generalized-linear-model.md#poisson-regression). It estimates

$$
\widehat\mu(a)=\exp(0.793+0.064a),\qquad
\boxed{\frac{\widehat\mu(a+1)}{\widehat\mu(a)}=e^{0.064}\simeq1.066}.
$$

Thus the fitted annual increase is about **6.6%**, with approximate 95% [confidence interval](../../statistical-inference.md#confidence-interval) for the [rate ratio](../../generalized-linear-model.md#rate-ratio) $(e^{0.001},e^{0.128})\simeq(1.001,1.137)$. The age evidence is much weaker than in the Gaussian fit: the quoted [p-value](../../statistical-hypothesis-test.md#p-value) is $0.047$. Zero estimated group variances do not prove that real bird and year differences are absent.

The [Poisson distribution](../../discrete-probability-distribution.md#poisson-distribution) forces conditional [variance](../../variance.md) to equal the conditional [expected value](../../expected-value.md). Here fitted means are around two to three hatchlings, whereas the Gaussian model estimated a residual [variance](../../variance.md) of only $0.188$. This suggests checking [underdispersion](../../exponential-family.md#underdispersion) and the bounded nature of hatching counts, rather than assuming a Poisson response solves the diagnostic problems. Inspect simulated count residuals and predictive distributions; if the number of eggs is observed, fit a binomial mixed model and check that model's dispersion too.

The displayed Gaussian and Poisson [Akaike information criterion](../../statistical-modelling.md#akaike-information-criterion) values should not simply be ranked as if they used the same likelihood convention: one evaluates a continuous density and the other a probability mass. Compare properly specified count models on the same observed response scale, with compatible likelihoods and predictive checks. A boundary fit, doubtful dispersion assumptions, and possible nonlinear age effects all warrant further work before a strong biological conclusion.

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The [product rule](../../calculus.md#product-rule) gives

$$
\boxed{f'(x)=1-(\log x+1)=-\log x},\qquad f''(x)=-1/x.
$$

In particular, the second [derivative](../../calculus.md#derivative) is negative throughout the domain.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The function is strictly [concave](../../real-analysis.md#concave-function) on $x>0$. Its [derivative](../../calculus.md#derivative) is positive for $0<x<1$, zero at $x=1$, and negative for $x>1$. Thus it rises from the limiting value $-1$ as $x\downarrow0$, touches the horizontal axis at its unique [maximum](../../set.md#maximum-of-a-subset-of-a-total-order) $(1,0)$, and then decreases to $-\infty$. It never crosses above the axis. The left endpoint is not included, and the slope tends to $+\infty$ there.

<a id="5/b/image-concave-logarithmic-function-and-the-beta-posterior-for-the-censored-observations"></a>
![](../../past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-1-sketches.png)

**[Figure 1](#5/b/image-concave-logarithmic-function-and-the-beta-posterior-for-the-censored-observations). Concave logarithmic function and the beta posterior for the censored observations**.

The left panel shows the required sketch; the right panel is used for question 6(e).

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

This is the [Nicholson-Bailey model](../../mathematical-biology.md#nicholson-bailey-model) for a [host](../../ecology.md#host-biology)-[parasitoid](../../ecology.md#parasitoid) interaction with discrete generations. The factor $r$ is the host multiplication factor in the absence of parasitism; $a$ measures effective attack or searching intensity per parasitoid; and $b$ is the number of next-generation parasitoids produced per attacked host, with any survival or unit conversion absorbed into it.

If the number of attacks on a host has a [Poisson distribution](../../discrete-probability-distribution.md#poisson-distribution) with [expected value](../../expected-value.md) $aP_t$, then the [probability](../../probability-theory.md#probability) of no attack is $e^{-aP_t}$. Consequently $e^{-aP_t}$ is the surviving, unparasitized host fraction, and $1-e^{-aP_t}$ is the attacked fraction. The two update equations count host descendants from surviving hosts and parasitoid descendants from attacked hosts, respectively.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

At an [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system), $H=rHe^{-aP}$ and $P=bH(1-e^{-aP})$. Taking $H=0$ forces $P=0$, giving extinction. If $H\ne0$, the first equation gives $e^{-aP}=1/r$ and hence

$$
\boxed{P_*=\frac{\log r}{a},\qquad H_*=
\frac{r\log r}{ab(r-1)}}\qquad(r\ne1).
$$

These are the only isolated candidates obtained from the equations. There is an exceptional parameter case: at $r=1$, $P=0$ and every $H\ge0$ is an [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system). Thus the assertion of exactly two [equilibria](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) needs $r\ne1$, and only the positive candidate belongs to the biological state space when $r>1$.

<h3 id="5/e">e</h3>

↑ **Parent:** [5](#5)

<h4 id="5/e/solution">Solution</h4>

↑ **Parent:** [E](#5/e)

Since $a,b>0$, the coexistence value $P_*=(\log r)/a$ is positive exactly when $r>1$. Under that condition, $H_*>0$ as well. Therefore the required condition is

$$
\boxed{r>1}.
$$

For $0<r<1$, the formal nonzero candidate has negative parasitoid density and is not biologically admissible; $r=1$ gives only the host-only line of [equilibria](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system).

<h3 id="5/f">f</h3>

↑ **Parent:** [5](#5)

<h4 id="5/f/solution">Solution</h4>

↑ **Parent:** [F](#5/f)

The [Jacobian matrix](../../multivariable-calculus.md#jacobian-matrix) of the update map is

$$
J(H,P)=\begin{pmatrix}
r e^{-aP}&-arHe^{-aP}\\
b(1-e^{-aP})&abHe^{-aP}
\end{pmatrix},\qquad
J(0,0)=\begin{pmatrix}r&0\\0&0\end{pmatrix}.
$$

Its [eigenvalues](../../linear-operator-theory.md#eigenvalue) are $r$ and zero. The extinction [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) is locally [asymptotically stable](../../dynamical-systems.md#asymptotic-stability) for $0<r<1$ and unstable for $r>1$, by [linear stability analysis](../../dynamical-systems.md#linear-stability) for a [discrete dynamical system](../../discrete-dynamical-system.md). In the latter case, even a small perturbation along $P=0$ grows as $H_t=r^tH_0$.

At $r=1$, an [eigenvalue](../../linear-operator-theory.md#eigenvalue) equals one, so the strict linear criterion does not decide stability. Directly, $0\le H_{t+1}\le H_t$ and $0\le P_{t+1}\le bH_t$. Starting sufficiently close to extinction therefore keeps both coordinates close for all time, proving [Lyapunov stability](../../dynamical-systems.md#lyapunov-stability) in the nonnegative state space. It is not [asymptotically stable](../../dynamical-systems.md#asymptotic-stability), since every nearby $(H,0)$ is another [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system). This distinction makes the statement “stable when $r>1$ fails” precise.

<h3 id="5/g">g</h3>

↑ **Parent:** [5](#5)

<h4 id="5/g/solution">Solution</h4>

↑ **Parent:** [G](#5/g)

Suppose $r>1$ and set $q=\log r/(r-1)$. Substitution of the positive [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) into the [Jacobian matrix](../../multivariable-calculus.md#jacobian-matrix) gives

$$
J_*=
\begin{pmatrix}
1&-r\log r/[b(r-1)]\\
b(r-1)/r&q
\end{pmatrix},\quad
\operatorname{tr}J_*=1+q,\quad
\det J_*=q+\log r=\frac{r\log r}{r-1}.
$$

Part (b) showed $f(x)<0$ whenever $x\ne1$. In particular,

$$
f(1/r)=\frac{1-r+\log r}{r}<0
$$

gives $\log r<r-1$, whereas

$$
f(r)=r-1-r\log r<0
$$

gives $\det J_*>1$. The latter already violates the [Jury stability criterion](../../discrete-dynamical-system.md#jury-stability-criterion) condition $1-\det J_*>0$. More directly, the product of the two [eigenvalues](../../linear-operator-theory.md#eigenvalue) is greater than one, so at least one has [modulus](../../complex-analysis.md#modulus) greater than one. Therefore the positive [equilibrium](../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) is **unstable**. This is the [instability of the Nicholson-Bailey equilibrium](../../mathematical-biology.md#instability-of-the-nicholson-bailey-equilibrium); parasitoid feedback in this simple model does not stabilize coexistence.

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

For independent [geometric random variables](../../discrete-probability-distribution.md#geometric-distribution) supported on $1,2,\ldots$, put $S=\sum_i x_i$. Multiplication of their [probability mass functions](../../probability-distribution.md#probability-mass-function) gives the [likelihood function](../../maximum-likelihood-estimation.md#likelihood-function)

$$
\boxed{\mathcal L(p)=p^n(1-p)^{S-n}},\qquad0<p<1.
$$

There are $n$ terminal successes and $S-n$ preceding failures.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

The [beta distribution](../../probability-distribution.md#beta-distribution) [prior density](../../bayesian-statistics.md#prior-density) is proportional to $p^{a-1}(1-p)^{b-1}$. By [Bayes' theorem](../../probability-theory.md#bayes-theorem), its product with the [likelihood function](../../maximum-likelihood-estimation.md#likelihood-function) gives the [posterior density](../../bayesian-statistics.md#posterior-density)

$$
\pi(p\mid x)\propto p^{a+n-1}(1-p)^{b+S-n-1}.
$$

This is again a [beta distribution](../../probability-distribution.md#beta-distribution), namely

$$
\boxed{p\mid x\sim\operatorname{Beta}(a+n,b+S-n)}.
$$

Thus the beta family is a [conjugate prior](../../exponential-family.md#conjugate-prior) family for the [geometric distribution](../../discrete-probability-distribution.md#geometric-distribution). The update is an instance of [beta-geometric conjugacy](../../bayesian-statistics.md#beta-geometric-conjugacy): counts of observed successes and failures are added to the two beta parameters.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Using the [expected value](../../expected-value.md) of a [beta distribution](../../probability-distribution.md#beta-distribution), the [posterior mean](../../bayesian-statistics.md#posterior-mean) is

$$
\boxed{\mathbb E[p\mid x]=\frac{a+n}{a+b+S}}.
$$

Equivalently, it is the weighted average

$$
\frac{a+b}{a+b+S}\frac{a}{a+b}
+\frac{S}{a+b+S}\frac{n}{S}
$$

of the [prior mean](../../bayesian-statistics.md#prior-mean) and the [maximum-likelihood estimate](../../maximum-likelihood-estimation.md#maximum-likelihood-estimator) $n/S$.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

For fixed prior parameters, divide numerator and denominator by $n$:

$$
\mathbb E[p\mid x]=\frac{1+a/n}{S/n+(a+b)/n}\longrightarrow\frac1{\mathbb E X}=p_0,
$$

under independent sampling from a [geometric distribution](../../discrete-probability-distribution.md#geometric-distribution) with true success probability $p_0>0$. The [law of large numbers](../../convergence-of-random-variables.md#law-of-large-numbers) gives $S/n\to1/p_0$. In a large finite sample the [posterior mean](../../bayesian-statistics.md#posterior-mean) is close to $n/S=1/\bar x$, the [maximum-likelihood estimate](../../maximum-likelihood-estimation.md#maximum-likelihood-estimator). The fixed prior's influence vanishes, and the estimate is [consistent](../../statistical-inference.md#consistency-statistics).

<h3 id="6/e">e</h3>

↑ **Parent:** [6](#6)

<h4 id="6/e/solution">Solution</h4>

↑ **Parent:** [E](#6/e)

The two colonies with no observed cheaters are [right-censored](../../survival-analysis.md#right-censoring) after seven days. Each contributes $\Pr(X>7)=(1-p)^7$, not the [probability](../../probability-theory.md#probability) of an event on day seven or eight. The four observed first events contribute four factors of $p$ and $(6-1)+(7-1)+(5-1)+(5-1)=19$ failures. Including the two censored exposures gives

$$
\mathcal L(p)\propto p^4(1-p)^{19+7+7}=p^4(1-p)^{33}.
$$

The [beta distribution](../../probability-distribution.md#beta-distribution) prior therefore yields

$$
\boxed{p\mid D\sim\operatorname{Beta}(9,38)},\qquad
\mathbb E[p\mid D]=\frac9{47}\simeq0.19149.
$$

Its [probability density function](../../continuous-probability-distribution.md#probability-density-function) is proportional to $p^8(1-p)^{37}$ for $0<p<1$: it vanishes at both endpoints, is unimodal, and has its [mode](../../probability-and-statistics.md#mode-statistics) at $8/45\simeq0.17778$. The right panel of the sketch in question 5(b) shows this moderately right-skewed density. The calculation assumes daily observations detect the first event and that stopping the experiment after seven days is [independent censoring](../../survival-analysis.md#independent-censoring).

<h3 id="6/f">f</h3>

↑ **Parent:** [6](#6)

<h4 id="6/f/solution">Solution</h4>

↑ **Parent:** [F](#6/f)

The trace has long, slowly changing stretches, indicating strong [autocorrelation](../../time-series.md#autocorrelation) and poor exploration of the [posterior distribution](../../bayesian-statistics.md#bayesian-posterior). The reported [effective sample size of a Markov chain](../../bayesian-statistics.md#effective-sample-size-of-a-markov-chain) is only $36$, so the number of stored draws greatly exaggerates the information in the simulation. The [potential scale reduction factor](../../bayesian-statistics.md#potential-scale-reduction-factor) $\widehat R=1.21$ is appreciably above one and does not support convergence between chains. The reported [Monte Carlo standard error](../../monte-carlo-method.md#monte-carlo-standard-error) $0.04$ is also large relative to a posterior mean near $0.2$.

The exact [beta distribution](../../probability-distribution.md#beta-distribution) gives [posterior mean](../../bayesian-statistics.md#posterior-mean) $9/47\simeq0.19149$ and [standard deviation](../../variance.md#standard-deviation)

$$
\sqrt{\frac{9\cdot38}{47^2\cdot48}}\simeq0.0568,
$$

so the simulation's reported spread $0.11$ is another warning. Do not interpret its mean or interval estimates as reliable yet. Run multiple chains from dispersed starts, improve and tune the proposal or sampler, and use longer runs after adaptation. Recheck the traces, [potential scale reduction factor](../../bayesian-statistics.md#potential-scale-reduction-factor), and [effective sample size of a Markov chain](../../bayesian-statistics.md#effective-sample-size-of-a-markov-chain). More iterations help only if the chain actually explores its target well; thinning alone does not fix poor mixing.

<h3 id="6/g">g</h3>

↑ **Parent:** [6](#6)

<h4 id="6/g/solution">Solution</h4>

↑ **Parent:** [G](#6/g)

**Direct independent sampling is preferable.** The [posterior distribution](../../bayesian-statistics.md#bayesian-posterior) is the standard [beta distribution](../../probability-distribution.md#beta-distribution) $\operatorname{Beta}(9,38)$, for which exact [posterior moments](../../bayesian-statistics.md#posterior-moment) and standard random-number generators are available. For example, draw independent $U\sim\operatorname{Gamma}(9,1)$ and $V\sim\operatorname{Gamma}(38,1)$ with the same rate, and return $U/(U+V)$. This has the required [beta distribution](../../probability-distribution.md#beta-distribution) and avoids [Markov chain Monte Carlo](../../bayesian-statistics.md#markov-chain-monte-carlo) convergence problems. A correct, converged MCMC method could sample this target, but it is unnecessarily complicated here.

## 7

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

Write $n_k=|C_k|$ and suppose the cluster is nonempty. Expanding the [Euclidean norm](../../normed-vector-space.md#euclidean-norm) through its [inner product](../../inner-product.md) gives

$$
\|x-z\|^2=\|(x-\bar x_k)-(z-\bar x_k)\|^2
=\|x-\bar x_k\|^2-2(x-\bar x_k)^{\mathsf T}(z-\bar x_k)
+\|z-\bar x_k\|^2.
$$

Sum over $x\in C_k$. The final term does not depend on $x$, so its sum is $n_k\|z-\bar x_k\|^2$, which proves the requested identity. This expansion is the starting point for the [centroid sum-of-squares identity](../../statistical-learning.md#centroid-sum-of-squares-identity).

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

The centred observations sum to zero:

$$
\sum_{x\in C_k}(x-\bar x_k)=\sum_{x\in C_k}x-n_k\bar x_k=0.
$$

By [linearity](../../vector-space.md#linearity) of the [inner product](../../inner-product.md),

$$
\sum_{x\in C_k}(x-\bar x_k)^{\mathsf T}(z-\bar x_k)
=\left(\sum_{x\in C_k}(x-\bar x_k)\right)^{\mathsf T}(z-\bar x_k)=0.
$$

This cancellation holds for every $z$.

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/solution">Solution</h4>

↑ **Parent:** [C](#7/c)

Combining the first two parts gives the [centroid sum-of-squares identity](../../statistical-learning.md#centroid-sum-of-squares-identity)

$$
J_k(z)=J_k(\bar x_k)+n_k\|z-\bar x_k\|^2.
$$

The added term is nonnegative and, since $n_k>0$, vanishes exactly at $z=\bar x_k$. Thus the unique minimizing [centroid](../../euclidean-geometry.md#centroid) in this step of [K-means clustering](../../statistical-learning.md#k-means-clustering) is

$$
\boxed{z_k=\bar x_k}.
$$

An empty cluster needs a separate algorithmic convention because its [sample mean](../../variance.md#sample-mean) is undefined and its objective is identically zero.

<h3 id="7/d">d</h3>

↑ **Parent:** [7](#7)

<h4 id="7/d/solution">Solution</h4>

↑ **Parent:** [D](#7/d)

Expanding the squared [Euclidean distances](../../topological-analysis.md#euclidean-distance) gives

$$
\|x-z_1\|^2-\|x-z_2\|^2
=-2x^{\mathsf T}(z_1-z_2)+\|z_1\|^2-\|z_2\|^2.
$$

For distinct [centroids](../../euclidean-geometry.md#centroid), choose

$$
\boxed{w=2(z_1-z_2),\qquad b=\|z_2\|^2-\|z_1\|^2}.
$$

A point assigned to $C_1$ has the displayed distance difference at most zero and therefore $w^{\mathsf T}x+b\ge0$; assignment to $C_2$ gives the reverse inequality. The separating [hyperplane](../../vector-space.md#hyperplane) is the [perpendicular bisector](../../euclidean-geometry.md#perpendicular-bisector) of the line segment joining the two [centroids](../../euclidean-geometry.md#centroid). Points tied between them lie on that [hyperplane](../../vector-space.md#hyperplane). This is the [nearest-centroid decision hyperplane](../../statistical-learning.md#nearest-centroid-decision-hyperplane).

The requested nonzero $w$ needs the additional assumption $z_1\ne z_2$. It does not follow from the stated algorithm alone. In one dimension, take $C_1=\{-1,1\}$ and $C_2=\{0\}$, whose [centroids](../../euclidean-geometry.md#centroid) are both zero. A tie rule that retains previous assignments can leave this configuration after an iteration. The inequalities at $-1,1$ imply $b\ge|w|$, while the inequality at zero implies $b\le0$, forcing $w=0$. Thus the unconditional nonzero-separator claim has this degenerate exception.

## ↑ Ancestors (10)

1. [2025](../2025.md)
2. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
3. [Mathematical and Computational Biology course of the University of Cambridge](../../university-of-cambridge.md#mathematical-and-computational-biology-course-of-the-university-of-cambridge)
4. [Year 2 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-2-of-the-natural-sciences-course-of-the-university-of-cambridge)
5. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
7. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
8. [University of Cambridge](../../university-of-cambridge.md)
9. [List of universities](../../README.md#list-of-universities)
10. [Codex Wiki](../../README.md)
