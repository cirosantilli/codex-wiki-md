# Paper 37

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_37.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_37.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
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
    - [i](#2/e/i)
      - [Solution](#2/e/i/solution)
    - [ii](#2/e/ii)
      - [Solution](#2/e/ii/solution)
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
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)
    - [iii](#4/c/iii)
      - [Solution](#4/c/iii/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [1](#5/d/1)
      - [Solution](#5/d/1/solution)
    - [2](#5/d/2)
      - [Solution](#5/d/2/solution)
    - [3](#5/d/3)
      - [i](#5/d/3/i)
        - [Solution](#5/d/3/i/solution)
      - [ii](#5/d/3/ii)
        - [Solution](#5/d/3/ii/solution)
- [6](#6)
  - [i](#6/i)
    - [a](#6/i/a)
      - [Solution](#6/i/a/solution)
    - [b](#6/i/b)
      - [Solution](#6/i/b/solution)
    - [c](#6/i/c)
      - [Solution](#6/i/c/solution)
    - [d](#6/i/d)
      - [Solution](#6/i/d/solution)
    - [e](#6/i/e)
      - [Solution](#6/i/e/solution)

## 1

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

**A stationary [causal time series](../../../time-series.md#causal-time-series) exists.** The [infinite moving-average representation](../../../time-series.md#infinite-moving-average-representation)

$$
X_t=\sum_{j=0}^\infty 2^{-j}\varepsilon_{t-j}
$$

converges in the sense of [mean-square convergence](../../../convergence-of-random-variables.md#convergence-in-l2) because the driving variables are [independent random variables](../../../random-variable.md#independent-random-variables) and $\sum_j4^{-j}<\infty$. Shifting the series gives $X_t=\tfrac12X_{t-1}+\varepsilon_t$. Its [expected value](../../../probability-theory.md#expected-value) is zero and its [autocovariance](../../../time-series.md#autocovariance) is

$$
\boxed{\gamma(h)=\frac{4\sigma^2}{3}\,2^{-|h|}.}
$$

Thus it is a [weakly stationary process](../../../time-series.md#weakly-stationary-process); since the driving variables have a [normal distribution](../../../probability-theory.md#normal-distribution), it is also a [Gaussian process](../../../stochastic-process.md#gaussian-process) and a [strictly stationary process](../../../time-series.md#strictly-stationary-process). Throughout the stationarity discussion, take $\sigma^2>0$; degenerate zero noise permits trivial constant solutions.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

**No [weakly stationary process](../../../time-series.md#weakly-stationary-process) solves the model with nondegenerate noise.** Iteration would give

$$
X_t-X_{t-m}=\sum_{j=0}^{m-1}\varepsilon_{t-j},\qquad \operatorname{Var}(X_t-X_{t-m})=m\sigma^2.
$$

For a [weakly stationary process](../../../time-series.md#weakly-stationary-process) with finite [variance](../../../variance.md) $V$, the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) instead gives $\operatorname{Var}(X_t-X_{t-m})=2V-2\gamma(m)\leq4V$. These two bounds contradict each other for large $m$. This argument does not assume that $X_{t-m}$ is independent of the intervening noise, so it excludes noncausal solutions too. The corresponding [unit-root autoregressive process](../../../time-series.md#unit-root-autoregressive-process) has persistent [random walk](../../../markov-process.md#random-walk) behavior rather than stationary fluctuations.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

**A [noncausal stationary autoregression](../../../time-series.md#noncausal-stationary-autoregression) exists.** On the two-sided time axis define

$$
X_t=-\sum_{j=1}^\infty2^{-j}\varepsilon_{t+j}.
$$

This series converges in the sense of [mean-square convergence](../../../convergence-of-random-variables.md#convergence-in-l2), and direct subtraction gives $X_t-2X_{t-1}=\varepsilon_t$. The [expected value](../../../probability-theory.md#expected-value) and [autocovariance](../../../time-series.md#autocovariance) are

$$
\boxed{\mathbb EX_t=0,\qquad\gamma(h)=\frac{\sigma^2}{3}\,2^{-|h|}.}
$$

Consequently this is a [weakly stationary process](../../../time-series.md#weakly-stationary-process) and, by Gaussianity, a [strictly stationary process](../../../time-series.md#strictly-stationary-process). It is an example of [noncausal stationary autoregression](../../../time-series.md#noncausal-stationary-autoregression), since $X_t$ uses future noise. In particular, $X_{t-1}$ is correlated with $\varepsilon_t$, so the usual causal [variance](../../../variance.md) recursion is inapplicable. If an additional assumption required the driving noise to be independent of past observations, this solution would be excluded; that assumption is not stated here.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A [unit-root autoregressive process](../../../time-series.md#unit-root-autoregressive-process) retains shocks permanently, whereas a [causal time series](../../../time-series.md#causal-time-series) with $|\phi|<1$ reverts towards its mean. Testing the unit root determines whether stationary autoregressive analysis is appropriate or [differencing](../../../time-series.md#differencing) is needed. For the model without an intercept or trend, use the [Dickey–Fuller test](../../../time-series.md#dickey-fuller-test) against the lower-sided alternative $\phi<1$ near the null. Put

$$
\widehat\phi=\frac{\sum_{t=2}^nX_{t-1}X_t}{\sum_{t=2}^nX_{t-1}^2},\qquad
\widehat\sigma^2=\frac1{n-2}\sum_{t=2}^n(X_t-\widehat\phi X_{t-1})^2,
\qquad T_n=\frac{(\widehat\phi-1)\sqrt{\sum_{t=2}^nX_{t-1}^2}}{\widehat\sigma}.
$$

This is the ordinary regression statistic for a zero coefficient when $\Delta X_t$ is regressed on $X_{t-1}$, but its null [probability distribution](../../../probability-theory.md#probability-distribution) is not the usual Student law. Under the standard unit-root initialization $X_1=o_P(\sqrt n)$ and innovations independent of the starting value,

$$
T_n\Rightarrow D=\frac{\int_0^1 W(u)\,dW(u)}{\sqrt{\int_0^1W(u)^2\,du}}
=\frac{W(1)^2-1}{2\sqrt{\int_0^1W(u)^2\,du}},
$$

where $W$ is standard [Brownian motion](../../../brownian-motion.md). If $d_\alpha$ is the lower $\alpha$-quantile of $D$, the **asymptotic level-$\alpha$ critical region** is

$$
\boxed{T_n<d_\alpha.}
$$

The deterministic terms and null initialization must match the critical-value table. For exact finite-sample [size of a statistical test](../../../statistical-modelling.md#size-of-a-statistical-test), calibrate the statistic from its Gaussian [random walk](../../../markov-process.md#random-walk) null with the specified initial condition and noise scale; for a zero starting value its distribution is scale-free. The printed two-sided recurrence alone specifies neither an initial law nor a universal finite-sample critical value. Ordinary normal quantiles do not give the intended [size of a statistical test](../../../statistical-modelling.md#size-of-a-statistical-test).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For a stationary linear autoregression, [causal time series](../../../time-series.md#causal-time-series) means that the observation uses only current and past driving noise:

$$
Y_t=\sum_{j\geq0}\psi_j\varepsilon_{t-j},\qquad \sum_{j\geq0}|\psi_j|^2<\infty.
$$

This is a convergent in the sense of [mean-square convergence](../../../convergence-of-random-variables.md#convergence-in-l2) [infinite moving-average representation](../../../time-series.md#infinite-moving-average-representation). The stronger usual stable-filter definition requires absolute summability; the argument below also handles the square-summable definition. Let $\Phi(z)=1-\sum_{k=1}^p\phi_kz^k$ and $\Psi(z)=\sum_{j\geq0}\psi_jz^j$. Substituting the filter into the recurrence and comparing coefficients of the orthogonal noise gives $\psi_0=1$ and $\psi_j=\sum_{k=1}^{\min(p,j)}\phi_k\psi_{j-k}$. Hence

$$
\Phi(z)\Psi(z)=1\qquad(|z|<1).
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) ensures that $\Psi$ is an [analytic function](../../../complex-analysis.md#space-of-holomorphic-functions) in this disk. Thus $\Phi$ has no zero strictly inside it. A boundary zero is also impossible: a zero of multiplicity $m\geq1$ at $z_0=e^{i\omega_0}$ makes $|1/\Phi(re^{i\omega})|^2$ at least a constant times $[(1-r)^2+(\omega-\omega_0)^2]^{-m}$ near that point. Its integral over $\omega$ diverges as $r\uparrow1$. On the other hand, [orthogonality of complex exponentials](../../../fourier-analysis.md#orthogonality-of-complex-exponentials) gives

$$
\frac1{2\pi}\int_{-\pi}^{\pi}|\Psi(re^{i\omega})|^2\,d\omega
=\sum_{j\geq0}|\psi_j|^2r^{2j}\leq\sum_{j\geq0}|\psi_j|^2<\infty,
$$

a contradiction. Therefore the [causality root criterion for an autoregressive model](../../../time-series.md#causality-root-criterion-for-an-autoregressive-model) is

$$
\boxed{\Phi(z)=0\ \Longrightarrow\ |z|>1.}
$$

Under absolute summability, the shorter boundary argument is continuity of $\Psi$ on the closed disk and the identity $\Phi\Psi=1$ there.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

By the [causality root criterion for an autoregressive model](../../../time-series.md#causality-root-criterion-for-an-autoregressive-model), choose $r>1$ smaller than the modulus of every root of $\Phi$. The function $\Psi=1/\Phi$ is an [analytic function](../../../complex-analysis.md#space-of-holomorphic-functions) on and inside $|z|=r$. Writing $M=\max_{|z|=r}|1/\Phi(z)|$, the [Cauchy estimate](../../../analysis.md#cauchy-estimate) gives $|\psi_j|\leq Mr^{-j}$. For $h\geq0$, [independence](../../../random-variable.md#independent-random-variables) of the noise in the [infinite moving-average representation](../../../time-series.md#infinite-moving-average-representation) gives

$$
\gamma(h)=\sigma^2\sum_{j\geq0}\psi_j\psi_{j+h},\qquad
|\gamma(h)|\leq\frac{\sigma^2M^2}{1-r^{-2}}r^{-h}.
$$

The [autocovariance](../../../time-series.md#autocovariance) is symmetric in the lag. Thus **exponential decay holds** with

$$
\boxed{s=r^{-1}\in(0,1),\qquad C=\frac{\sigma^2M^2}{1-r^{-2}}.}
$$

This is [exponential autocovariance decay of a causal autoregression](../../../time-series.md#exponential-autocovariance-decay-of-a-causal-autoregression). If $\Phi$ is constant, there are no roots and any $r>1$ works.

## 2

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [weakly stationary process](../../../time-series.md#weakly-stationary-process) has finite [second moments](../../../probability-theory.md#second-moment), a constant [expected value](../../../probability-theory.md#expected-value) $\mu$, and [covariance](../../../variance.md#covariance) depending only on the time difference:

$$
\mathbb EX_t=\mu,\qquad\operatorname{Cov}(X_{t+h},X_t)=\gamma(h).
$$

A [strictly stationary process](../../../time-series.md#strictly-stationary-process), also called strongly stationary, has every finite-dimensional [probability distribution](../../../probability-theory.md#probability-distribution) invariant under a common shift: for every finite choice of times and every shift $h$, $(X_{t_1+h},\ldots,X_{t_m+h})$ and $(X_{t_1},\ldots,X_{t_m})$ have the same law. [strict stationarity](../../../time-series.md#strictly-stationary-process) with finite [second moments](../../../probability-theory.md#second-moment) implies [weak stationarity](../../../time-series.md#weakly-stationary-process). [weak stationarity](../../../time-series.md#weakly-stationary-process) alone does not determine the full joint law, and [strict stationarity](../../../time-series.md#strictly-stationary-process) alone does not guarantee finite moments.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Two useful features of [autoregressive conditional heteroscedasticity](../../../time-series.md#autoregressive-conditional-heteroscedasticity) are **persistent changes in conditional scale** and **excess unconditional [kurtosis](../../../probability-theory.md#kurtosis)**. Its time-varying [conditional variance](../../../variance.md#conditional-variance) can explain [volatility clustering](../../../time-series.md#volatility-clustering), where large absolute returns occur in groups even when signed returns have little [autocorrelation](../../../time-series.md#autocorrelation). A homoscedastic [autoregressive moving-average model](../../../time-series.md#autoregressive-moving-average-model) has a fixed innovation [variance](../../../variance.md).

Also, a conditional [normal distribution](../../../probability-theory.md#normal-distribution) with a random scale is a [Gaussian scale mixture](../../../statistical-modelling.md#gaussian-scale-mixture). Its unconditional [kurtosis](../../../probability-theory.md#kurtosis) can exceed $3$, or its [fourth moment](../../../probability-theory.md#fourth-moment) can be infinite. A Gaussian [autoregressive moving-average model](../../../time-series.md#autoregressive-moving-average-model) remains jointly Gaussian and cannot reproduce this effect. In the particular [lag-two ARCH process](../../../time-series.md#lag-two-arch-process), persistence of the squared scale occurs within each parity subsequence; the two parity subsequences are independent.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

First justify the dependence structure rather than assume that adjacent squares behave like an ordinary lag-one ARCH model. Write $Z_t=X_t^2$. Iterating its nonnegative recurrence gives

$$
Z_t=\alpha_0\sum_{k=0}^{m-1}\alpha_2^k\prod_{j=0}^k\varepsilon_{t-2j}^2
+\alpha_2^m\left(\prod_{j=0}^{m-1}\varepsilon_{t-2j}^2\right)Z_{t-2m}.
$$

The product coefficient has [expected value](../../../probability-theory.md#expected-value) $\alpha_2^m$, so it tends to zero in probability. The stationary $Z_{t-2m}$ are a tight family; consequently the remainder tends to zero in probability, without needing [independence](../../../random-variable.md#independent-random-variables) between that remainder's factors. The increasing partial sums therefore give the representation

$$
Z_t=\alpha_0\sum_{k\geq0}\alpha_2^k\prod_{j=0}^k\varepsilon_{t-2j}^2\quad\text{almost surely}.
$$

This proves the [parity decomposition of a lag-two ARCH process](../../../time-series.md#parity-decomposition-of-a-lag-two-arch-process): even and odd observations are functions of disjoint noise families. It also shows that the positive scale $\sigma_t$ is a function of past noise, independent of $\varepsilon_t$. The [conditional expectation](../../../measure-theory.md#conditional-expectation) of $X_t$ given past noise is zero, and the second-moment recursion is $m_2=\alpha_0+\alpha_2m_2$. [independence](../../../random-variable.md#independent-random-variables) of the parity families gives the adjacent-square [covariance](../../../variance.md#covariance). Thus

$$
\boxed{\mathbb EX_t=0,\qquad m_2=\mathbb EX_t^2=\frac{\alpha_0}{1-\alpha_2},\qquad
\operatorname{Cov}(X_t^2,X_{t+1}^2)=0.}
$$

To establish finiteness of the [fourth moment](../../../probability-theory.md#fourth-moment) before using its recursion, note that the $L^2$ norm of the $k$th term in the positive series for $Z_t$ is $\alpha_0\sqrt3(\alpha_2\sqrt3)^k$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) in [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space) makes the series square-integrable when $3\alpha_2^2<1$. [independence](../../../random-variable.md#independent-random-variables) of the current noise and past scale then yields

$$
m_4=3\mathbb E(\alpha_0+\alpha_2X_{t-2}^2)^2
=3\alpha_0^2+6\alpha_0\alpha_2m_2+3\alpha_2^2m_4,
$$

and hence

$$
\boxed{\mathbb EX_t^4=\frac{3\alpha_0^2(1+\alpha_2)}{(1-\alpha_2)(1-3\alpha_2^2)}\quad\text{if }3\alpha_2^2<1.}
$$

If $3\alpha_2^2\geq1$, a finite $m_4$ would make $(1-3\alpha_2^2)m_4=3\alpha_0^2+6\alpha_0\alpha_2m_2>0$, which is impossible. Its [fourth moment](../../../probability-theory.md#fourth-moment) is then infinite. The adjacent-square product remains integrable by parity [independence](../../../random-variable.md#independent-random-variables), even in that case.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The useful [autoregressive model](../../../time-series.md#autoregressive-model) is for the squares, not for signed observations. Put $Y_t=X_t^2$ and

$$
u_t=(\varepsilon_t^2-1)(\alpha_0+\alpha_2Y_{t-2}).
$$

Then

$$
\boxed{Y_t=\alpha_0+\alpha_2Y_{t-2}+u_t.}
$$

The errors form a [martingale difference sequence](../../../martingale.md#martingale-difference-sequence) relative to the noise history, because the current standardized noise is independent of the past. When the [fourth moment](../../../probability-theory.md#fourth-moment) is finite they have finite [variance](../../../variance.md) and are uncorrelated across distinct times, although their [conditional variance](../../../variance.md#conditional-variance) depends on the regressor. In centered form, $Y_t-m_2=\alpha_2(Y_{t-2}-m_2)+u_t$.

For [ordinary least squares](../../../statistical-modelling.md#ordinary-least-squares), use the $n-2$ response-regressor pairs $y_t=X_t^2$, $r_t=X_{t-2}^2$, $t=3,\ldots,n$. With their separate means $\bar y$ and $\bar r$, minimize $\sum_{t=3}^n(y_t-a-br_t)^2$. If the regressor sum of squares is positive, the estimators are

$$
\boxed{\widehat\alpha_2=\frac{\sum_{t=3}^n(r_t-\bar r)(y_t-\bar y)}{\sum_{t=3}^n(r_t-\bar r)^2},\qquad
\widehat\alpha_0=\bar y-\widehat\alpha_2\bar r.}
$$

The two means use the matched pairs; replacing them indiscriminately by a single full-sample mean is not the exact least-squares formula. The noise-series representation supplies an [ergodic stationary process](../../../time-series.md#ergodic-stationary-process). If $3\alpha_2^2<1$, finite regressor [second moments](../../../probability-theory.md#second-moment) and the error's zero [conditional expectation](../../../measure-theory.md#conditional-expectation) justify the usual population regression and [statistical consistency](../../../statistical-inference.md#consistency-statistics) argument. The observations still define a finite-sample least-squares fit outside that moment range, but the ordinary finite-[variance](../../../variance.md) justification must not be claimed there. If parameter constraints are required, minimize the same criterion subject to $a>0$ and $0<b<1$, rather than assert that unconstrained estimates automatically satisfy them.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/i">i</h4>

↑ **Parent:** [E](#2/e)

<h5 id="2/e/i/solution">Solution</h5>

↑ **Parent:** [I](#2/e/i)

**The [covariance](../../../variance.md#covariance) is zero.** Let $\mathcal F_t=\sigma(\varepsilon_s:s\leq t)$. The stationary noise-series representation makes $f(X_t)$ measurable with respect to $\mathcal F_t$, whereas the [martingale difference sequence](../../../martingale.md#martingale-difference-sequence) property gives $\mathbb E[X_{t+h}\mid\mathcal F_{t+h-1}]=0$. The [law of total expectation](../../../measure-theory.md#law-of-total-expectation) therefore gives

$$
\mathbb E[X_{t+h}f(X_t)]
=\mathbb E\!\left[f(X_t)\mathbb E(X_{t+h}\mid\mathcal F_{t+h-1})\right]=0.
$$

Since $\mathbb EX_{t+h}=0$, this is the required [covariance](../../../variance.md#covariance). All products are integrable by the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality), using finite [second moments](../../../probability-theory.md#second-moment) of $X$ and the stipulated square integrability of $f(X_t)$.

<h4 id="2/e/ii">ii</h4>

↑ **Parent:** [E](#2/e)

<h5 id="2/e/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/e/ii)

**This [covariance](../../../variance.md#covariance) is also zero, but symmetry is essential to the proof.** Write $\varepsilon_t=\eta_t|\varepsilon_t|$, where $\eta_t$ is an independent fair sign. The [normal distribution](../../../probability-theory.md#normal-distribution) makes that sign independent of its magnitude and of every other driving variable. Conditional on the magnitudes and all noise except this sign, changing $\eta_t$ flips $X_t$ and leaves $X_t^2$ unchanged. Every future conditional scale uses only squared past observations, so $X_{t+h}$ is unchanged for $h>0$.

Thus $f(X_{t+h})$ is independent of the remaining fair sign in $X_t$. Averaging that sign gives $\mathbb E[X_tf(X_{t+h})]=0$, and hence

$$
\boxed{\operatorname{Cov}(X_t,f(X_{t+h}))=0.}
$$

The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) again guarantees integrability. For odd $h$, the [parity decomposition of a lag-two ARCH process](../../../time-series.md#parity-decomposition-of-a-lag-two-arch-process) also gives [independence](../../../random-variable.md#independent-random-variables) directly. For even $h$, the [sign symmetry of an ARCH process](../../../time-series.md#sign-symmetry-of-an-arch-process) supplies the argument; the [martingale difference sequence](../../../martingale.md#martingale-difference-sequence) property alone would not justify this reversed [covariance](../../../variance.md#covariance).

## 3

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a centered [weakly stationary process](../../../time-series.md#weakly-stationary-process) with $\gamma(0)>0$, the [autocorrelation function](../../../time-series.md#autocorrelation) is

$$
\boxed{\rho(h)=\gamma(h)/\gamma(0).}
$$

For $h\geq2$, let $P$ be [orthogonal projection](../../../hilbert-space.md#orthogonal-projection) in [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space) onto the linear span of $X_{t-1},\ldots,X_{t-h+1}$. The lag-$h$ [partial autocorrelation function](../../../time-series.md#partial-autocorrelation-function) is the [correlation coefficient](../../../variance.md#pearson-correlation-coefficient) of $X_t-PX_t$ and $X_{t-h}-PX_{t-h}$. It removes the linear contribution of the intervening observations. At lag one it is just $\rho(1)$. For nonsingular prediction [covariance](../../../variance.md#covariance) matrices, it is equivalently the last coefficient $a_{hh}$ in the order-$h$ linear predictor of $X_t$ from $X_{t-1},\ldots,X_{t-h}$. Equal residual variances, by stationarity, identify that coefficient with the residual correlation. If a residual has zero [variance](../../../variance.md), this correlation is undefined; the nondegeneracy condition matters.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Use the [sample autocorrelation function](../../../time-series.md#sample-autocorrelation-function) and [sample partial autocorrelation function](../../../time-series.md#sample-partial-autocorrelation-function) to look for approximate cutoffs. For a minimal causal [autoregressive model](../../../time-series.md#autoregressive-model) of order $p$, the [partial autocorrelation function](../../../time-series.md#partial-autocorrelation-function) is zero beyond $p$, while the [autocorrelation function](../../../time-series.md#autocorrelation) usually tails off, possibly with damped oscillation. For an invertible [moving-average model](../../../time-series.md#moving-average-model) of order $q$, the [autocorrelation function](../../../time-series.md#autocorrelation) is zero beyond $q$, while the [partial autocorrelation function](../../../time-series.md#partial-autocorrelation-function) tails off. In a mixed [autoregressive moving-average model](../../../time-series.md#autoregressive-moving-average-model), both generally tail off.

Thus the last visibly nonzero partial correlation suggests an autoregressive order, and the last visibly nonzero autocorrelation suggests a moving-average order. Finite samples do not produce exact zeros. Approximate white-noise reference bands can help flag clearly nonzero lags, but they are not universal [confidence intervals](../../../statistical-inference.md#confidence-interval) for arbitrary correlated processes. Fit a few suggested orders and check residual [autocorrelation](../../../time-series.md#autocorrelation), rather than treating these plots as a proof of the model order. This is [order identification by autocorrelation cutoffs](../../../time-series.md#order-identification-by-autocorrelation-cutoffs).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For the [moving-average process of order one](../../../time-series.md#moving-average-process-of-order-one), $\gamma(0)=\sigma^2(1+\theta_1^2)$, $\gamma(1)=\sigma^2\theta_1$, and $\gamma(2)=0$. Regressing each endpoint on the single intervening observation leaves residual [covariance](../../../variance.md#covariance) $\gamma(2)-\gamma(1)^2/\gamma(0)$ and residual [variance](../../../variance.md) $\gamma(0)-\gamma(1)^2/\gamma(0)$. Therefore its lag-two [partial autocorrelation function](../../../time-series.md#partial-autocorrelation-function) is

$$
\alpha(2)=\frac{\rho(2)-\rho(1)^2}{1-\rho(1)^2}
=\boxed{-\frac{\theta_1^2}{1+\theta_1^2+\theta_1^4}.}
$$

The denominator is positive. In particular, the moving-average autocorrelation cutoff at lag one does not make the lag-two partial correlation zero unless $\theta_1=0$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Use [cycles-per-time spectral density](../../../time-series.md#cycles-per-time-spectral-density), with frequency $\omega\in[-1/2,1/2]$. The [spectral representation theorem for a stationary time series](../../../time-series.md#spectral-representation-theorem-for-a-stationary-time-series) gives the centered [white noise](../../../time-series.md#white-noise) representation

$$
\varepsilon_t=\int_{-1/2}^{1/2}e^{2\pi it\omega}\,dZ_\varepsilon(\omega),\qquad
\mathbb E|dZ_\varepsilon(\omega)|^2=\sigma^2\,d\omega,
$$

where disjoint increments are orthogonal. Put $\theta_0=1$. Since the filter is finite, substitute each noise representation and interchange the finite sum with the integral:

$$
X_t=\int_{-1/2}^{1/2}e^{2\pi it\omega}\Theta(e^{-2\pi i\omega})\,dZ_\varepsilon(\omega).
$$

The new orthogonal increment measure is $dZ_X=\Theta(e^{-2\pi i\omega})dZ_\varepsilon$. Its [variance](../../../variance.md) measure is therefore $\sigma^2|\Theta(e^{-2\pi i\omega})|^2d\omega$. The coefficients are real, so conjugation changes the sign of the exponent without changing the modulus. Hence

$$
\boxed{f_X(\omega)=\sigma^2|\Theta(e^{2\pi i\omega})|^2.}
$$

With angular frequency $\lambda=2\pi\omega$, the [spectral density of a stationary process](../../../time-series.md#spectral-density-of-a-stationary-process) instead contains the factor $1/(2\pi)$. The convention explains its absence here. Invertibility is not needed for this finite-filter spectral calculation.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The [autocovariance](../../../time-series.md#autocovariance) vanishes beyond lag $q$. For an ordinary consecutive sum, [variance of a sum](../../../variance.md#variance-of-a-sum) gives

$$
\operatorname{Var}\!\left(\frac1{\sqrt n}\sum_{t=1}^nX_t\right)
=\sum_{|h|<n}\left(1-\frac{|h|}{n}\right)\gamma(h)
\longrightarrow\sum_{h\in\mathbb Z}\gamma(h).
$$

The last sum is finite. For $h\geq0$, $\gamma(h)=\sigma^2\sum_{j=0}^{q-h}\theta_j\theta_{j+h}$. Counting all coefficient pairs gives

$$
\boxed{\lim_{n\to\infty}\operatorname{Var}\!\left(\frac1{\sqrt n}\sum_{t=1}^nX_t\right)
=\sigma^2\left(\sum_{j=0}^q\theta_j\right)^2=\sigma^2\Theta(1)^2.}
$$

For the odd-indexed sample the lag-$h$ [autocovariance](../../../time-series.md#autocovariance) is $\gamma(2h)$, so the same finite-sum argument gives $\sum_h\gamma(2h)$. Only coefficient pairs of the same parity contribute. If $E=\sum_{j\ {\rm even}}\theta_j$ and $O=\sum_{j\ {\rm odd}}\theta_j$, the **odd-subsample limit** is

$$
\boxed{\lim_{n\to\infty}\operatorname{Var}\!\left(\frac1{\sqrt n}\sum_{t=1}^nX_{2t-1}\right)
=\sigma^2(E^2+O^2)=\frac{\sigma^2}{2}\bigl[\Theta(1)^2+\Theta(-1)^2\bigr].}
$$

This is the [odd-subsample long-run variance of a moving average](../../../time-series.md#odd-subsample-long-run-variance-of-a-moving-average). Equivalently it is $[f_X(0)+f_X(1/2)]/2$ in the cycles convention. Under the printed invertibility assumption and positive noise [variance](../../../variance.md), the polynomial is nonzero at both $1$ and $-1$, so both limits are positive. The same formulas also hold without invertibility, when cancellations can make a limit zero.

## 4

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The generalized [quantile function](../../../probability-theory.md#quantile-function) is

$$
\boxed{F^{-1}(u)=\inf\{x\in\mathbb R:F(x)\geq u\},\qquad0<u<1.}
$$

The tail limits of a [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function) make the defining set nonempty and its infimum finite. Monotonicity and right continuity imply $F^{-1}(u)\leq x$ exactly when $u\leq F(x)$. To see the direction involving the infimum, let points in the defining set decrease towards it; right continuity gives $F(F^{-1}(u))\geq u$, so every larger $x$ also qualifies. Consequently, for a [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) variable $U$,

$$
\mathbb P(F^{-1}(U)\leq x)=\mathbb P(U\leq F(x))=F(x).
$$

The probability-zero endpoints $U=0,1$ can be assigned arbitrary outputs. This proves [inverse transform sampling](../../../probability-theory.md#inverse-transform-sampling) even for distributions with atoms or flat portions; continuity or strict monotonicity of $F$ is not required.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Choose a proposal [probability density function](../../../continuous-probability-distribution.md#probability-density-function) $q$ positive wherever $|h|f$ is nonzero, up to null sets, and draw [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables) $Y_1,\ldots,Y_n$ from $q$. The ordinary [importance sampling](../../../probability-and-statistics.md#importance-sampling) estimator is

$$
\boxed{\widehat\mu_{\rm IS}=\frac1n\sum_{i=1}^n\frac{h(Y_i)f(Y_i)}{q(Y_i)}.}
$$

The [support condition for importance sampling](../../../probability-and-statistics.md#support-condition-for-importance-sampling) and absolute integrability give $\mathbb E_q[h(Y)f(Y)/q(Y)]=\int hf=\mu$, so this is an [unbiased estimator](../../../statistical-modelling.md#unbiased-estimator). Its [variance](../../../variance.md), possibly infinite, is

$$
\operatorname{Var}(\widehat\mu_{\rm IS})=\frac1n\left[\int\frac{h(x)^2f(x)^2}{q(x)}\,dx-\mu^2\right].
$$

Let $A=\int|h|f$. If $A>0$, the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) yields

$$
A^2=\left(\int\frac{|h|f}{\sqrt q}\sqrt q\right)^2\leq\int\frac{h^2f^2}{q}.
$$

Equality holds for $q$ proportional to $|h|f$. Thus the [minimum-variance importance distribution](../../../probability-and-statistics.md#minimum-variance-importance-distribution) and the minimum [variance](../../../variance.md) are

$$
\boxed{q_*(x)=\frac{|h(x)|f(x)}{A},\qquad \operatorname{Var}(\widehat\mu_{\rm IS})_{\min}=\frac{A^2-\mu^2}{n}.}
$$

For a constant-sign integrand this is zero [variance](../../../variance.md). If $A=0$, the integrand vanishes almost everywhere and the zero estimator already has zero [variance](../../../variance.md). Requiring the proposal to cover all of the target's support, including where $h=0$, can exclude $q_*$; in that stricter class, $(1-\epsilon)q_*+\epsilon f$ approaches the same infimum as $\epsilon\downarrow0$. This distinguishes coverage of the integral from coverage of every target event.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

Integrating the [Weibull distribution](../../../probability-theory.md#weibull-distribution) density gives $F(x)=1-\exp(-x^\alpha/\beta)$ for $x>0$. [Inverse transform sampling](../../../probability-theory.md#inverse-transform-sampling) therefore gives

$$
\boxed{X=[-\beta\log(1-U_1)]^{1/\alpha}.}
$$

Replacing $1-U_1$ by $U_1$ produces the same [probability distribution](../../../probability-theory.md#probability-distribution). Both uniforms belong to $(0,1)$ with probability one. Here the conventional Weibull scale is $\beta^{1/\alpha}$, rather than $\beta$.

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

The [Box-Muller transform](../../../probability-and-statistics.md#box-muller-transform) uses independent uniforms to set

$$
R=\sqrt{-2\log U_2},\qquad A=2\pi U_3,\qquad
\boxed{X_1=R\cos A,\quad X_2=R\sin A.}
$$

The radius has the unit [Rayleigh distribution](../../../continuous-probability-distribution.md#rayleigh-distribution), with density $re^{-r^2/2}$ for $r>0$, and the angle is independently uniform on $[0,2\pi)$. Their joint density is $(2\pi)^{-1}re^{-r^2/2}$. The Cartesian change of variables has absolute [Jacobian determinant](../../../calculus.md#jacobian-determinant) $r$, so the joint density of $(X_1,X_2)$ is

$$
\frac1{2\pi}e^{-(x_1^2+x_2^2)/2}
=\left(\frac1{\sqrt{2\pi}}e^{-x_1^2/2}\right)
\left(\frac1{\sqrt{2\pi}}e^{-x_2^2/2}\right).
$$

The factorization proves that the outputs are [independent random variables](../../../random-variable.md#independent-random-variables), each with a [standard normal distribution](../../../probability-theory.md#standard-normal-distribution).

<h4 id="4/c/iii">iii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/c/iii)

Recognize the integrand as a [Gaussian scale mixture](../../../statistical-modelling.md#gaussian-scale-mixture). If $R$ has the unit [Rayleigh distribution](../../../continuous-probability-distribution.md#rayleigh-distribution) and $Z$ is an independent [standard normal distribution](../../../probability-theory.md#standard-normal-distribution) variable, then the conditional density of $RZ$ given $R=r$ is $(\sqrt{2\pi}r)^{-1}e^{-x^2/(2r^2)}$. Multiplying by the radius density gives

$$
\int_0^\infty\frac1{\sqrt{2\pi}r}e^{-x^2/(2r^2)}\,r e^{-r^2/2}\,dr
=\frac1{\sqrt{2\pi}}\int_0^\infty e^{-(x^2+r^4)/(2r^2)}\,dr=g(x).
$$

Thus use $U_1$ for the independent radius and $U_2,U_3$ for the normal output of the [Box-Muller transform](../../../probability-and-statistics.md#box-muller-transform):

$$
\boxed{X=\sqrt{-2\log U_1}\,\sqrt{-2\log U_2}\cos(2\pi U_3).}
$$

The mixture argument also proves that $g$ integrates to one, by the [Tonelli theorem](../../../measure-theory.md#tonelli-theorem). As a check, $R^2$ is exponential of rate $1/2$, so the [characteristic function](../../../probability-theory.md#characteristic-function) of $RZ$ is $\mathbb E e^{-t^2R^2/2}=1/(1+t^2)$. This is the [Rayleigh-normal scale mixture](../../../statistical-modelling.md#rayleigh-normal-scale-mixture), with [Laplace distribution](../../../continuous-probability-distribution.md#laplace-distribution) density $e^{-|x|}/2$.

## 5

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Let $P$ be the [transition kernel](../../../markov-process.md#markov-kernel) of the [Markov chain](../../../markov-process.md#markov-chain). It is [phi-irreducible](../../../markov-process.md#phi-irreducibility) if there is a nonzero [sigma-finite measure](../../../measure-theory.md#sigma-finite-measure) $\varphi$ such that, for every measurable $A$ and every starting state $x$,

$$
\boxed{\varphi(A)>0\quad\Longrightarrow\quad\sum_{n=1}^\infty P^n(x,A)>0.}
$$

Equivalently, there is positive probability of eventually reaching every set of positive reference measure. For a finite state space with counting measure, this becomes ordinary [irreducible Markov chain](../../../markov-process.md#irreducible-markov-chain) accessibility. On a continuous space, requiring access to each individual point would usually be inappropriate; positive-measure sets play that role. Irreducibility requires positive probability, rather than probability one, and does not itself assert recurrence or a finite mean return time.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

A convenient general-state-space ergodic theorem is the following. For a [positive Harris recurrent Markov chain](../../../markov-process.md#positive-harris-recurrent-markov-chain) with invariant [probability measure](../../../probability-theory.md#probability-measure) $\pi$, and a measurable function $h$ with $\pi|h|<\infty$,

$$
\boxed{\frac1n\sum_{t=1}^nh(X_t)\longrightarrow\pi h\quad\text{almost surely}.}
$$

Here $\pi h=\int h\,d\pi$ is the stationary [expected value](../../../probability-theory.md#expected-value). [Harris recurrence](../../../markov-process.md#harris-recurrent-markov-chain) means that every set of positive irreducibility measure is visited almost surely from every state; positive recurrence supplies an invariant probability rather than only an infinite invariant measure. The [ergodic theorem for a positive Harris recurrent Markov chain](../../../markov-process.md#ergodic-theorem-for-a-positive-harris-recurrent-markov-chain) holds from any starting state under these Harris hypotheses. [aperiodicity](../../../markov-process.md#aperiodic-markov-chain) is not necessary just for averages.

A useful sufficient form of the [central limit theorem for a geometrically ergodic Markov chain](../../../statistical-inference.md#central-limit-theorem-for-a-geometrically-ergodic-markov-chain) adds [aperiodicity](../../../markov-process.md#aperiodic-markov-chain), [geometric ergodicity](../../../statistical-inference.md#geometric-ergodicity), and $\pi(|h|^{2+\delta})<\infty$ for some $\delta>0$. It gives

$$
\boxed{\sqrt n\left(\frac1n\sum_{t=1}^nh(X_t)-\pi h\right)\Rightarrow N(0,v_h),\qquad
v_h=\gamma_h(0)+2\sum_{k=1}^\infty\gamma_h(k).}
$$

These are sufficient hypotheses, not a claim that irreducibility alone ensures a [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem). The [Markov chain Monte Carlo asymptotic variance](../../../statistical-inference.md#markov-chain-monte-carlo-asymptotic-variance) uses stationary covariances $\gamma_h(k)=\operatorname{Cov}_\pi(h(X_0),h(X_k))$, with $\gamma_h(0)=\operatorname{Var}_\pi h$. The series is absolutely convergent under the stated sufficient assumptions. If $\gamma_h(0)>0$, write $\rho_h(k)=\gamma_h(k)/\gamma_h(0)$ and $v_h=\gamma_h(0)\tau_{\rm int}$, where the [integrated autocorrelation time](../../../statistical-inference.md#integrated-autocorrelation-time) is $\tau_{\rm int}=1+2\sum_{k\geq1}\rho_h(k)$. When $v_h>0$, the [effective sample size of a Markov chain](../../../statistical-inference.md#effective-sample-size-of-a-markov-chain) is approximately $n/\tau_{\rm int}$. Negative correlations can reduce the asymptotic [variance](../../../variance.md); a zero asymptotic [variance](../../../variance.md) gives a degenerate normal limit. For constant $h$, [variance](../../../variance.md) is zero and the autocorrelation normalization is undefined.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

First require a proper target: $0<Z=\int_{\mathbb R^d}\pi(x)\,dx<\infty$ and $\bar\pi=\pi/Z$. The [Metropolis–Hastings algorithm](../../../statistical-inference.md#metropolis-hastings-algorithm) uses the [Metropolis–Hastings acceptance probability](../../../statistical-inference.md#metropolis-hastings-acceptance-probability)

$$
a(x,y)=\min\!\left\{1,\frac{\pi(y)q(x\mid y)}{\pi(x)q(y\mid x)}\right\}.
$$

Sufficient general conditions are [phi-irreducibility](../../../markov-process.md#phi-irreducibility), [aperiodicity](../../../markov-process.md#aperiodic-markov-chain), and a [drift-minorisation condition](../../../statistical-inference.md#drift-minorisation-condition) establishing [geometric ergodicity](../../../statistical-inference.md#geometric-ergodicity) of the resulting chain, together with a stationary $(2+\delta)$th moment for the observable being averaged. These imply the [central limit theorem for a geometrically ergodic Markov chain](../../../statistical-inference.md#central-limit-theorem-for-a-geometrically-ergodic-markov-chain). The observable's moment condition must be included: conditions on the sampler alone cannot give the theorem for every arbitrary function.

A concrete stronger condition, directly in terms of the proposal, is

$$
\boxed{q(y\mid x)\geq\epsilon\bar\pi(y)\quad\text{for all }x,y\text{ in the target support},\qquad\epsilon>0.}
$$

Together with a bounded observable, this is an especially simple sufficient answer. The accepted proposal density is $\min\{q(y\mid x),\bar\pi(y)q(x\mid y)/\bar\pi(x)\}$, so it is at least $\epsilon\bar\pi(y)$. The kernel satisfies a global [minorization condition](../../../statistical-inference.md#minorization-condition) with the target, hence [uniform geometric ergodicity](../../../statistical-inference.md#uniform-geometric-ergodicity), positive [Harris recurrence](../../../markov-process.md#harris-recurrent-markov-chain), and [aperiodicity](../../../markov-process.md#aperiodic-markov-chain). An independent proposal whose importance weight $\bar\pi(y)/q(y)$ is uniformly bounded is one example. No claim of these properties follows merely from writing down a positive proposal.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/1">1</h4>

↑ **Parent:** [D](#5/d)

<h5 id="5/d/1/solution">Solution</h5>

↑ **Parent:** [1](#5/d/1)

The algorithm is a [Random-scan Gibbs sampler](../../../statistical-inference.md#random-scan-gibbs-sampler). Start at a point where the target is positive, with a proper normalizing integral and well-defined [full conditional distributions](../../../probability-theory.md#full-conditional-distribution). Its state is the entire coordinate vector. Choosing the initial point fixes the initial law; it need not already be the invariant law. The transition rule below preserves the target irrespective of this choice.

<h4 id="5/d/2">2</h4>

↑ **Parent:** [D](#5/d)

<h5 id="5/d/2/solution">Solution</h5>

↑ **Parent:** [2](#5/d/2)

At each transition, choose a coordinate uniformly and independently of the previous coordinate choices. Draw a fresh value from that coordinate's [full conditional distribution](../../../probability-theory.md#full-conditional-distribution) given the current remaining coordinates, and keep all other coordinates fixed. This supplies the random-selection and conditional-draw operations lost in the TeX transcription. The update depends only on the current vector and fresh randomness, which proves the [Markov property](../../../markov-process.md#markov-property). The printed mathematical requests are the kernel and its [detailed balance](../../../markov-process.md#detailed-balance), answered in the following two subsections.

<h4 id="5/d/3">3</h4>

↑ **Parent:** [D](#5/d)

<h5 id="5/d/3/i">i</h5>

↑ **Parent:** [3](#5/d/3)

<h6 id="5/d/3/i/solution">Solution</h6>

↑ **Parent:** [I](#5/d/3/i)

For the [Random-scan Gibbs sampler](../../../statistical-inference.md#random-scan-gibbs-sampler), the correct [transition kernel](../../../markov-process.md#markov-kernel) is a measure, since a one-coordinate update is singular with respect to full-dimensional [Lebesgue measure](../../../measure-theory.md#lebesgue-measure) when $p>1$. Write $x_{-i}$ for all coordinates except $i$. Then

$$
\boxed{P(x,dx')=\frac1p\sum_{i=1}^p\pi_i(x_i'\mid x_{-i})\,dx_i'\prod_{j\ne i}\delta_{x_j}(dx_j').}
$$

Each [Dirac measure](../../../measure-theory.md#dirac-measure) fixes an unupdated coordinate. Equivalently, $P(x,A)=p^{-1}\sum_i\int\mathbf1_A(x_{-i},z)\pi_i(z\mid x_{-i})\,dz$, with $z$ placed in coordinate $i$. Replacing this kernel by an ordinary density on the whole product space would omit those fixed-coordinate constraints.

<h5 id="5/d/3/ii">ii</h5>

↑ **Parent:** [3](#5/d/3)

<h6 id="5/d/3/ii/solution">Solution</h6>

↑ **Parent:** [Ii](#5/d/3/ii)

Let $\bar\pi$ be the normalized target and $\bar\pi_{-i}$ its [marginal distribution](../../../probability-theory.md#marginal-distribution). A coordinate-$i$ kernel $P_i$ leaves $x_{-i}=x'_{-i}$ and has the joint old-new measure

$$
\bar\pi(dx)P_i(x,dx')=
\bar\pi_{-i}(dx_{-i})\,
\pi_i(x_i\mid x_{-i})\,dx_i\,
\pi_i(x_i'\mid x_{-i})\,dx_i'\,
\delta_{x_{-i}}(dx'_{-i}).
$$

This is symmetric in the old and new state: the common remaining coordinates are fixed and the two conditional factors exchange places. Thus each coordinate kernel satisfies [detailed balance](../../../markov-process.md#detailed-balance). Averaging them with the fixed weights $1/p$ proves

$$
\boxed{\bar\pi(dx)P(x,dx')=\bar\pi(dx')P(x',dx).}
$$

Integrating out the old state proves invariance of $\bar\pi$. The common normalization cancels, so detailed balance can also be written with the unnormalized target. This establishes [detailed balance of a random-scan Gibbs sampler](../../../statistical-inference.md#detailed-balance-of-a-random-scan-gibbs-sampler) and a [reversible Markov chain](../../../markov-process.md#reversible-markov-chain). Fresh independent random choices make the update a [Markov chain](../../../markov-process.md#markov-chain), as explained above; invariance is not an assertion that an arbitrarily initialized chain starts in stationarity.

## 6

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/a">a</h4>

↑ **Parent:** [I](#6/i)

<h5 id="6/i/a/solution">Solution</h5>

↑ **Parent:** [A](#6/i/a)

Use the [Bayes' theorem](../../../probability-theory.md#bayes-theorem) to multiply the [Ising model](../../../statistical-physics.md#ising-model) prior by the conditionally independent normal likelihood factors. For fixed observed $x$, the [posterior distribution](../../../statistical-inference.md#bayesian-posterior) is

$$
\boxed{\pi(s\mid x)\propto
\exp\!\left[-J\sum_{\{i,j\}\in\mathcal N}s_is_j
-\frac12\sum_{k\in D}\left\{x_k-\left(\sum_{j\in\mathcal N_k}s_j\right)^7\right\}^2\right],\qquad s\in\{-1,1\}^D.}
$$

There is no boundary wraparound: the neighbor sets use only actual horizontal and vertical edges inside the square. Each unordered edge is counted once. In particular, the prior retains the printed minus sign in front of $J$, and the likelihood retains the seventh power. The finite state space and finite observed values make every posterior weight positive and finite, with a finite positive normalizing sum.

<h4 id="6/i/b">b</h4>

↑ **Parent:** [I](#6/i)

<h5 id="6/i/b/solution">Solution</h5>

↑ **Parent:** [B](#6/i/b)

The prior factors involving $s_i$ are $\exp(-Js_is_j)$ for $j\in\mathcal N_i$. A likelihood factor centered at $k$ depends on $s_i$ precisely when $i\in\mathcal N_k$, equivalently $k\in\mathcal N_i$. Those factors are

$$
\exp\!\left[-\frac12\left\{x_k-\left(\sum_{j\in\mathcal N_k}s_j\right)^7\right\}^2\right],\qquad k\in\mathcal N_i.
$$

**Only incident prior edges and likelihoods centered at neighboring sites are affected.** In particular, the likelihood centered at $i$ does not depend on $s_i$: its mean involves only the neighbors of $i$. These are the [local likelihood factors in a hidden spin field](../../../statistical-inference.md#local-likelihood-factors-in-a-hidden-spin-field). The resulting conditional dependence can extend two lattice steps, beyond the nearest-neighbor prior interactions. For $K=1$, both collections are empty.

<h4 id="6/i/c">c</h4>

↑ **Parent:** [I](#6/i)

<h5 id="6/i/c/solution">Solution</h5>

↑ **Parent:** [C](#6/i/c)

For $k\in\mathcal N_i$, put $a_k^{(i)}=\sum_{j\in\mathcal N_k\setminus\{i\}}s_j$ and $H_i=\sum_{j\in\mathcal N_i}s_j$. Removing all factors independent of $s_i$ from the [posterior distribution](../../../statistical-inference.md#bayesian-posterior) gives, for $u\in\{-1,1\}$,

$$
w_i(u)=\exp\!\left[-JuH_i-\frac12\sum_{k\in\mathcal N_i}\{x_k-(a_k^{(i)}+u)^7\}^2\right],\qquad
\boxed{\pi_i(u\mid s_{-i},x)=\frac{w_i(u)}{w_i(+1)+w_i(-1)}.}
$$

A stable implementation uses the difference of the log weights. The conditional [log odds](../../../statistical-modelling.md#log-odds) are

$$
L_i=-2JH_i-\frac12\sum_{k\in\mathcal N_i}
\left[\{x_k-(a_k^{(i)}+1)^7\}^2-\{x_k-(a_k^{(i)}-1)^7\}^2\right],
$$

so $\pi_i(+1\mid s_{-i},x)=1/(1+e^{-L_i})$, a [logistic function](../../../statistical-learning.md#logistic-function). For very large $|L_i|$, evaluate this logistic expression using the sign of $L_i$ to avoid exponential overflow.

For [Gibbs sampling for a finite hidden spin field](../../../statistical-inference.md#gibbs-sampling-for-a-finite-hidden-spin-field), initialize any spin configuration. At every step choose $i\in D$ uniformly, draw a fresh uniform variable, set spin $i$ to $+1$ with the probability above and to $-1$ otherwise, and leave all remaining spins fixed. This [Random-scan Gibbs sampler](../../../statistical-inference.md#random-scan-gibbs-sampler) has the stated [posterior distribution](../../../statistical-inference.md#bayesian-posterior) invariant by [detailed balance of a random-scan Gibbs sampler](../../../statistical-inference.md#detailed-balance-of-a-random-scan-gibbs-sampler). All [conditional probabilities](../../../probability-theory.md#conditional-probability) are strictly between zero and one. For the one-site case, the [conditional probabilities](../../../probability-theory.md#conditional-probability) are both $1/2$.

<h4 id="6/i/d">d</h4>

↑ **Parent:** [I](#6/i)

<h5 id="6/i/d/solution">Solution</h5>

↑ **Parent:** [D](#6/i/d)

Apply the [Monte Carlo estimator](../../../probability-and-statistics.md#monte-carlo-estimator) to the observable $h(s)=\exp(\sum_{i\in D}\sqrt{2+s_i})$:

$$
\boxed{\widehat\theta_T=\frac1T\sum_{t=1}^T\exp\!\left(\sum_{i\in D}\sqrt{2+S_i^{(t)}}\right).}
$$

The theoretical justification is the [ergodic theorem for a positive Harris recurrent Markov chain](../../../markov-process.md#ergodic-theorem-for-a-positive-harris-recurrent-markov-chain), not an independent-sample law of large numbers. The [Markov chain](../../../markov-process.md#markov-chain) has finite state space, is irreducible, and has the strictly positive [posterior distribution](../../../statistical-inference.md#bayesian-posterior) as invariant law, so it is positive recurrent and Harris recurrent with counting measure. The observable is bounded: $e^{K^2}\leq h(s)\leq e^{\sqrt3K^2}$. Thus the estimator converges almost surely to the posterior [expected value](../../../probability-theory.md#expected-value) from any initial configuration.

Each state also has positive self-transition probability, so the chain is an [aperiodic Markov chain](../../../markov-process.md#aperiodic-markov-chain). Finiteness then gives geometric convergence and the relevant [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem); serial dependence determines the [Markov chain Monte Carlo asymptotic variance](../../../statistical-inference.md#markov-chain-monte-carlo-asymptotic-variance) if error bars are required. A fixed finite burn-in can be discarded without changing consistency, but [independence](../../../random-variable.md#independent-random-variables) of the retained states should not be assumed.

<h4 id="6/i/e">e</h4>

↑ **Parent:** [I](#6/i)

<h5 id="6/i/e/solution">Solution</h5>

↑ **Parent:** [E](#6/i/e)

Fix any configurations $s$ and $s'$. List the sites where they differ and update those sites in turn to their target signs. Every specified site has positive probability $1/K^2$ of being selected. At every intermediate configuration, both values of its [full conditional distribution](../../../probability-theory.md#full-conditional-distribution) have positive probability, since all weights $w_i(\pm1)$ are finite and strictly positive. The finite prescribed sequence therefore has positive probability and reaches $s'$.

Thus **every configuration is accessible from every other configuration**, so the sampler is an [irreducible Markov chain](../../../markov-process.md#irreducible-markov-chain), or equivalently [phi-irreducible](../../../markov-process.md#phi-irreducibility) with counting measure. If $s=s'$, a single update that keeps its selected spin unchanged also has positive probability. This simultaneously proves positive self-transition probability and [aperiodicity](../../../markov-process.md#aperiodic-markov-chain), including $K=1$. The sign of finite $J$ does not alter the accessibility argument.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
