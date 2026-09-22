# Paper 38

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper38.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper38.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [Solution](#4/solution)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Condition first on the count in the [random sum of independent claims](../../../actuarial-statistics.md#random-sum-of-independent-claims). For $N=k$, [independence](../../../random-variable.md#independent-random-variables) of the summands and independence from $N$ give

$$
\mathbb E[e^{uS}\mid N=k]=\prod_{j=1}^k\mathbb E[e^{uX_j}]=M_X(u)^k.
$$

The empty product is one when $k=0$. Taking [expected values](../../../probability-theory.md#expected-value) proves the [random-sum transform identity](../../../actuarial-statistics.md#random-sum-transform-identity):

$$
\boxed{M_S(u)=\sum_{k=0}^{\infty}\mathbb P(N=k)M_X(u)^k=G_N(M_X(u)).}
$$

For positive claim sizes this composition is always finite for $u\le0$, and is an identity of [Laplace transforms of nonnegative random variables](../../../probability-theory.md#laplace-transform-of-a-nonnegative-random-variable) after writing $u=-s$. For positive $u$, it holds wherever the composed series is finite; no positive [exponential moment](../../../probability-theory.md#exponential-moment) is implied merely by positivity of the summands.

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write $\lambda=\sum_i\lambda_i$, and suppose first that $\lambda>0$. Let $T_i$ be policy $i$'s aggregate, and $M_i$ the [moment-generating function](../../../probability-theory.md#moment-generating-function) of its claim sizes. The [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) count has [probability generating function](../../../probability-theory.md#probability-generating-function) $G_i(z)=\exp(\lambda_i(z-1))$, so the [random-sum transform identity](../../../actuarial-statistics.md#random-sum-transform-identity) and [independence](../../../random-variable.md#independent-random-variables) of the policies give

$$
M_T(u)=\prod_i\exp(\lambda_i(M_i(u)-1))
=\exp\left[\lambda\left(\sum_i\frac{\lambda_i}{\lambda}M_i(u)-1\right)\right].
$$

The expression in the weighted sum is the [moment-generating function](../../../probability-theory.md#moment-generating-function) of a [mixture distribution](../../../probability-theory.md#mixture-distribution) with claim [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function)

$$
F_*(x)=\sum_i\frac{\lambda_i}{\lambda}F_i(x).
$$

Thus **the aggregate has a [compound Poisson distribution](../../../actuarial-statistics.md#compound-poisson-distribution) with intensity $\lambda$ and severity law $F_*$**. This identification remains valid without positive [exponential moments](../../../probability-theory.md#exponential-moment), using the same calculation for [Laplace transforms of nonnegative random variables](../../../probability-theory.md#laplace-transform-of-a-nonnegative-random-variable) and their uniqueness. It is the [Poisson superposition of insurance portfolios](../../../actuarial-statistics.md#poisson-superposition-of-insurance-portfolios).

For common unit-rate [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) severities, the merged count $K$ is [Poisson distributed](../../../discrete-probability-distribution.md#poisson-distribution) with mean $\lambda$. Because each severity is strictly positive, $T=0$ exactly when $K=0$, giving

$$
\boxed{a=e^{-\lambda}.}
$$

For $k\ge1$, the sum of $k$ unit-rate [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) claims has [Erlang distribution](../../../continuous-probability-distribution.md#erlang-distribution) density $x^{k-1}e^{-x}/(k-1)!$. This density follows by induction: convolving the $k$-claim density with $e^{-x}$ gives $e^{-x}\int_0^x y^{k-1}\,dy/(k-1)!=e^{-x}x^k/k!$. Conditional on a positive aggregate, the count weights are

$$
\mathbb P(K=k\mid K>0)=\frac{e^{-\lambda}\lambda^k/k!}{1-e^{-\lambda}}=\frac{\lambda^k}{(e^\lambda-1)k!}.
$$

Therefore the [hurdle decomposition of a positive random sum](../../../actuarial-statistics.md#hurdle-decomposition-of-a-positive-random-sum) has positive-component [probability density function](../../../continuous-probability-distribution.md#probability-density-function)

$$
\boxed{\widetilde f_T(x)=\sum_{k=1}^{\infty}\frac{\lambda^k}{(e^\lambda-1)k!}\frac{x^{k-1}e^{-x}}{(k-1)!},\qquad x>0.}
$$

Each density integrates to one and the weights sum to one. Hence $F_T(x)=a+(1-a)\widetilde F_T(x)$ for $x\ge0$, where $\widetilde F_T$ is the conditional [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function) given $T>0$. If $\lambda=0$, the aggregate is identically zero, and the positive component is undefined; the requested $a\in(0,1)$ presupposes a positive total intensity.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The original PDF specifies a [geometric distribution](../../../discrete-probability-distribution.md#geometric-distribution) on $\{0,1,\ldots\}$, with probabilities $pq^k$. Its [probability generating function](../../../probability-theory.md#probability-generating-function) is $p/(1-qz)$. By [independence](../../../random-variable.md#independent-random-variables), the total original claim count $K=\sum_iN_i$ has

$$
G_K(z)=\left(\frac p{1-qz}\right)^n,
\qquad
\mathbb P(K=k)=\binom{n+k-1}{k}p^nq^k,\quad k\ge0.
$$

The coefficient follows from the [negative binomial series](../../../real-analysis.md#negative-binomial-series). Thus **one representation uses independent unit-rate [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) steps and a [negative binomial distribution](../../../discrete-probability-distribution.md#negative-binomial-distribution) count $K$**.

There is a second useful [random sum of independent claims](../../../actuarial-statistics.md#random-sum-of-independent-claims) representation. For one policy, the [random-sum transform identity](../../../actuarial-statistics.md#random-sum-transform-identity) gives

$$
M_{T_i}(u)=\frac{p}{1-q/(1-u)}=\frac{p(1-u)}{p-u}=p+q\frac p{p-u},\qquad u<p.
$$

This is the [mixture distribution](../../../probability-theory.md#mixture-distribution) of zero with probability $p$ and a rate-$p$ [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) with probability $q$. Consequently

$$
\boxed{T\overset d=\sum_{j=1}^B Y_j,\qquad B\sim\operatorname{Binomial}(n,q),\quad Y_j\sim\operatorname{Exp}(p),}
$$

with the [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) count independent of the independent steps. Equality follows by multiplying the [moment-generating functions](../../../probability-theory.md#moment-generating-function). This is a [negative-binomial sum of exponential claims](../../../actuarial-statistics.md#negative-binomial-sum-of-exponential-claims).

When $n=2$, the three values of $B$ give

$$
\mathcal L(T)=p^2\delta_0+2pq\operatorname{Exp}(p)+q^2\operatorname{Erlang}(2,p).
$$

Thus the zero mass is $\boxed{b=p^2}$, and the conditional positive [probability density function](../../../continuous-probability-distribution.md#probability-density-function) is

$$
\boxed{\widetilde f_T(x)=\frac{p^2e^{-px}}{1-p^2}(2q+q^2x),\qquad x>0.}
$$

Its integral is $(2pq+q^2)/(1-p^2)=1$. Equivalently the positive-component [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function) is

$$
\widetilde F_T(x)=1-e^{-px}\left(1+\frac{pq^2x}{1-p^2}\right),\qquad x\ge0,
$$

so $F_T(x)=p^2+(1-p^2)\widetilde F_T(x)$. For $x<0$, $F_T(x)=0$.

## 2

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let $P(z)$, $F(z)$ and $G(z)$ be the [probability generating functions](../../../probability-theory.md#probability-generating-function) of $N$, one severity, and $S$, respectively. Positivity of the severities gives $F(0)=0$ and $g_0=p_0$; the [random-sum transform identity](../../../actuarial-statistics.md#random-sum-transform-identity) gives $G=P\circ F$. The count recurrence in the [Panjer claim-count class](../../../actuarial-statistics.md#panjer-claim-count-class) implies

$$
P'(z)=\sum_{n\ge1}np_nz^{n-1}
=\sum_{n\ge1}(an+b)p_{n-1}z^{n-1}
=azP'(z)+(a+b)P(z).
$$

Use the [chain rule](../../../calculus.md#chain-rule) and substitute $F(z)$ to obtain

$$
(1-aF(z))G'(z)=(a+b)F'(z)G(z).
$$

Equating the coefficient of $z^{r-1}$ gives

$$
r g_r-a\sum_{j=1}^r(r-j)f_jg_{r-j}
=(a+b)\sum_{j=1}^rj f_jg_{r-j}.
$$

The factor multiplying $f_jg_{r-j}$ after rearrangement is $a(r-j)+(a+b)j=ar+bj$. Therefore the [Panjer recursion](../../../actuarial-statistics.md#panjer-recursion) is

$$
\boxed{g_0=p_0,\qquad g_r=\sum_{j=1}^r\left(a+\frac{bj}{r}\right)f_jg_{r-j}\quad(r\ge1).}
$$

These power-series calculations are valid inside the convergence discs of the [probability generating functions](../../../probability-theory.md#probability-generating-function), and hence justify the coefficient identities without assumptions about positive [exponential moments](../../../probability-theory.md#exponential-moment).

For a [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) count, $p_n/p_{n-1}=\lambda/n$, so $a=0$ and $b=\lambda$. The aggregate recursion becomes

$$
\boxed{g_0=e^{-\lambda},\qquad g_r=\frac\lambda r\sum_{j=1}^rj f_jg_{r-j}.}
$$

To obtain a [moment](../../../probability-theory.md#moment) recursion, write $\mu_j=\mathbb E X^j$, $m_j=\mathbb E S^j$, and $m_0=1$. For nonnegative measurable $h$, conditioning on $N=n$ and using exchangeability of the severities gives

$$
\begin{aligned}
\mathbb E[S h(S)]
&=\sum_{n\ge1}p_n n\,\mathbb E\left[X_1h\left(X_1+\sum_{j=2}^nX_j\right)\right]\\
&=\lambda\sum_{m\ge0}p_m\,\mathbb E\left[Xh\left(X+\sum_{j=1}^mX_j\right)\right]
=\lambda\mathbb E[Xh(X+S)],
\end{aligned}
$$

where $X$ on the right is independent of $S$. The second equality uses $np_n=\lambda p_{n-1}$, the [Poisson size-bias identity](../../../discrete-probability-distribution.md#poisson-size-bias-identity). Choosing $h(s)=s^{k-1}$, applying the [binomial theorem](../../../combinatorics.md#binomial-theorem), and using [independence](../../../random-variable.md#independent-random-variables) proves the [raw moment recursion for a compound Poisson distribution](../../../actuarial-statistics.md#raw-moment-recursion-for-a-compound-poisson-distribution):

$$
\boxed{m_k=\lambda\sum_{j=0}^{k-1}\binom{k-1}{j}\mu_{j+1}m_{k-1-j},\qquad k\ge1.}
$$

For any particular $k$, a finite severity $k$th [moment](../../../probability-theory.md#moment) suffices: $(\sum_{i=1}^nX_i)^k\le n^{k-1}\sum_{i=1}^nX_i^k$, and the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) has finite [moments](../../../probability-theory.md#moment) of every order. No positive [moment-generating function](../../../probability-theory.md#moment-generating-function) domain is required.

The first three iterations give

$$
m_1=\lambda\mu_1,\qquad
m_2=\lambda\mu_2+\lambda^2\mu_1^2,\qquad
m_3=\lambda\mu_3+3\lambda^2\mu_1\mu_2+\lambda^3\mu_1^3.
$$

Subtracting the appropriate powers of the [expected value](../../../probability-theory.md#expected-value) yields

$$
\boxed{\mathbb ES=\lambda\mu_1,\qquad
\operatorname{Var}(S)=\lambda\mu_2,\qquad
\mathbb E[(S-\mathbb ES)^3]=\lambda\mu_3.}
$$

In particular, the aggregate [variance](../../../variance.md) and third [central moment](../../../probability-theory.md#central-moment) involve the raw second and third severity [moments](../../../probability-theory.md#moment), rather than their centered counterparts.

## 3

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let $C_t$ be the cumulative claim amount and $U_t=u+ct-C_t$ the surplus in the [classical risk model](../../../actuarial-statistics.md#classical-risk-model). The supplied [adjustment coefficient](../../../actuarial-statistics.md#adjustment-coefficient) satisfies $\lambda(M_X(R)-1)=cR$. The [Compound Poisson process](../../../stochastic-process.md#compound-poisson-process) has independent increments, and the [random-sum transform identity](../../../actuarial-statistics.md#random-sum-transform-identity) gives

$$
\mathbb E[e^{R(C_t-C_s)}]=\exp((t-s)\lambda(M_X(R)-1)).
$$

It follows that $Z_t=\exp(R(C_t-ct))$ is a nonnegative [martingale](../../../martingale.md) with $Z_0=1$: conditional on the past, the multiplicative increment has [expected value](../../../probability-theory.md#expected-value) one. This is the [exponential surplus martingale](../../../actuarial-statistics.md#exponential-surplus-martingale).

Let $\tau=\inf\{t\ge0:U_t<0\}$ be the ruin [stopping time](../../../martingale.md#stopping-time). Surplus decreases only at claim arrivals, so on $\{\tau\le t\}$ the deficit at ruin gives $C_\tau-c\tau>u$ and $Z_\tau>e^{Ru}$. The [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) at the bounded [stopping time](../../../martingale.md#stopping-time) $\tau\wedge t$ yields

$$
1=\mathbb E Z_{\tau\wedge t}\ge\mathbb E[Z_\tau\mathbf1_{\{\tau\le t\}}]
\ge e^{Ru}\mathbb P(\tau\le t).
$$

As $t$ increases without bound, the events $\{\tau\le t\}$ increase to eventual ruin. Hence the [ultimate ruin probability](../../../actuarial-statistics.md#ultimate-ruin-probability) satisfies the [Lundberg inequality](../../../actuarial-statistics.md#lundberg-inequality)

$$
\boxed{\psi(u)=\mathbb P(\tau<\infty)\le e^{-Ru},\qquad u\ge0.}
$$

The proof uses only bounded-time stopping; it does not presume that the [martingale](../../../martingale.md) can be stopped with equality of [expected values](../../../probability-theory.md#expected-value) at an unbounded ruin time.

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a unit-rate [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution), $\mu=1$ and $M_X(r)=1/(1-r)$ for $r<1$. The [adjustment coefficient](../../../actuarial-statistics.md#adjustment-coefficient) equation is

$$
\frac r{1-r}=(1+\theta)r.
$$

Its nonzero root is

$$
\boxed{R_{\rm exp}=\frac\theta{1+\theta}.}
$$

It lies in $(0,1)$ for $\theta>0$, so the [moment-generating function](../../../probability-theory.md#moment-generating-function) is finite there and the [Lundberg inequality](../../../actuarial-statistics.md#lundberg-inequality) applies.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The severity is an equal-weight [mixture distribution](../../../probability-theory.md#mixture-distribution) of rate-$2$ and rate-$2/3$ [exponential distributions](../../../continuous-probability-distribution.md#exponential-distribution). Its [expected value](../../../probability-theory.md#expected-value) is

$$
\boxed{\mu=\frac12\frac12+\frac12\frac32=1.}
$$

The [moment-generating function](../../../probability-theory.md#moment-generating-function), finite exactly for $r<2/3$, is

$$
M_X(r)=\frac1{2-r}+\frac1{2-3r},\qquad
M_X(r)-1=\frac{r(4-3r)}{(2-r)(2-3r)}.
$$

Canceling the nonzero $r$ in the [adjustment coefficient](../../../actuarial-statistics.md#adjustment-coefficient) equation and multiplying by the positive denominator on $0<r<2/3$ gives

$$
4-3r=(1+\theta)(4-8r+3r^2).
$$

Thus the required [polynomial](../../../polynomial.md) is

$$
P(r)=3(1+\theta)r^2-(8\theta+5)r+4\theta.
$$

Since $P(0)=4\theta>0$, $P(2/3)=-2<0$, and the leading coefficient is positive, one root lies in $(0,2/3)$ and the other exceeds $2/3$. Only the smaller root is in the [moment-generating function](../../../probability-theory.md#moment-generating-function) domain. Consequently

$$
\boxed{R_{\rm mix}=\frac{8\theta+5-\sqrt{16\theta^2+32\theta+25}}{6(1+\theta)}
=\frac{8\theta}{8\theta+5+\sqrt{16\theta^2+32\theta+25}}.}
$$

The rationalized expression avoids subtraction of nearly equal numbers when $\theta$ is small.

The erroneously chosen same-mean [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) gives $R_{\rm exp}=\theta/(1+\theta)$. Direct substitution shows $P(R_{\rm exp})=-\theta<0$, so $R_{\rm exp}$ lies strictly between the two polynomial roots, and in particular $R_{\rm mix}<R_{\rm exp}$. Therefore

$$
\boxed{e^{-R_{\rm exp}u}<e^{-R_{\rm mix}u}\quad(u>0),}
$$

while both bounds equal one at $u=0$. **The exponential misspecification produces a smaller claimed upper bound.** The [Lundberg inequality](../../../actuarial-statistics.md#lundberg-inequality) certifies $e^{-R_{\rm mix}u}$ for the actual mixture; it does not certify the smaller expression computed from the wrong severity law.

## 4

↑ **Parent:** [Paper 38](paper-38.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The PDF gives an [inverse-gamma distribution](../../../continuous-probability-distribution.md#inverse-gamma-distribution) with shape $k$ and scale $\theta$, and a [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) prior with shape $\alpha$ and rate $\lambda$. Write $\mu(\theta)=\theta/(k-1)$. The supplied conditional [moments](../../../probability-theory.md#moment), together with $\mathbb E\theta=\alpha/\lambda$ and $\mathbb E\theta^2=\alpha(\alpha+1)/\lambda^2$, give the three structural quantities of the [Bühlmann model](../../../actuarial-statistics.md#buhlmann-model):

$$
\begin{aligned}
m&=\mathbb E\mu(\theta)=\frac\alpha{\lambda(k-1)},\\
v&=\operatorname{Var}(\mu(\theta))=\frac\alpha{\lambda^2(k-1)^2},\\
s^2&=\mathbb E[\operatorname{Var}(X_i\mid\theta)]
=\frac{\alpha(\alpha+1)}{\lambda^2(k-1)^2(k-2)}.
\end{aligned}
$$

Here $v$ is the [variance of hypothetical means](../../../actuarial-statistics.md#variance-of-hypothetical-means) and $s^2$ the [expected process variance](../../../actuarial-statistics.md#expected-process-variance). The [law of total covariance](../../../variance.md#law-of-total-covariance) and [conditional independence](../../../random-variable.md#conditional-independence) of different years imply

$$
\mathbb E X_i=m,\qquad
\operatorname{Cov}(\mu(\theta),X_i)=v,\qquad
\operatorname{Cov}(X_i,X_j)=v+s^2\mathbf1_{\{i=j\}}.
$$

All these quantities are finite because $k>2$.

For any coefficients $c_i$, minimizing the [mean squared error](../../../statistical-modelling.md#mean-squared-error) over the intercept first gives $c_0=m(1-\sum_i c_i)$. Let $Y=\mu(\theta)-m$ and $W_i=X_i-m$. Expanding the remaining [mean squared error](../../../statistical-modelling.md#mean-squared-error) gives

$$
\mathbb E\left[(Y-\sum_i c_iW_i)^2\right]
=v-2v\sum_i c_i+s^2\sum_i c_i^2+v\left(\sum_i c_i\right)^2.
$$

Its [normal equations](../../../statistical-modelling.md#normal-equation) are $s^2c_i+v\sum_jc_j=v$ for every $i$. Since $s^2>0$, subtracting any two equations shows that all $c_i$ agree. The quadratic part is strictly positive for every nonzero coefficient change, so the solution is the unique global minimizer. Solving gives

$$
\boxed{c_i=\frac v{s^2+nv}=\frac{k-2}{n(k-2)+\alpha+1}\quad(1\le i\le n),\qquad
c_0=\frac{\alpha(\alpha+1)}{\lambda(k-1)[n(k-2)+\alpha+1]}.}
$$

A [credibility estimate](../../../actuarial-statistics.md#credibility-estimate) combines individual experience with the collective [expected value](../../../probability-theory.md#expected-value), using an experience weight $Z\in[0,1]$. In this equal-exposure setting, the [Bühlmann credibility premium](../../../actuarial-statistics.md#buhlmann-credibility-premium) is

$$
\boxed{\widehat\mu_{\rm lin}=(1-Z)m+Z\overline X,\qquad
Z=\frac{nv}{s^2+nv}=\frac{n(k-2)}{n(k-2)+\alpha+1}.}
$$

Thus the computed coefficients give exactly a [credibility estimate](../../../actuarial-statistics.md#credibility-estimate), with a fixed [credibility factor](../../../actuarial-statistics.md#credibility-factor) determined by known parameters and the number of observed years. This is [Bühlmann credibility for inverse-gamma observations](../../../actuarial-statistics.md#buhlmann-credibility-for-inverse-gamma-observations).

For the final Bayesian calculation, the [likelihood function](../../../statistical-modelling.md#likelihood-function) in $\theta$ is proportional to $\theta^{nk}\exp(-\theta\sum_i x_i^{-1})$. Multiplication by the [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) prior gives the [Gamma prior for an inverse-gamma scale](../../../continuous-probability-distribution.md#gamma-prior-for-an-inverse-gamma-scale) update

$$
\theta\mid x_1,\ldots,x_n\sim\operatorname{Gamma}\left(\alpha+nk,\text{ rate }\lambda+\sum_i x_i^{-1}\right).
$$

Under [quadratic loss](../../../statistical-inference.md#squared-error-loss), the conditional risk of an estimate $d$ is $\operatorname{Var}(\mu(\theta)\mid x)+(d-\mathbb E[\mu(\theta)\mid x])^2$. Its minimizer is therefore the [posterior mean](../../../statistical-inference.md#posterior-mean):

$$
\boxed{\widehat\mu_{\rm Bayes}=\frac{\alpha+nk}{(k-1)(\lambda+\sum_i x_i^{-1})}.}
$$

**This is not a fixed-weight arithmetic-mean [credibility estimate](../../../actuarial-statistics.md#credibility-estimate).** For $n=2$, the observations $(1,3)$ and $(2,2)$ have the same [sample mean](../../../variance.md#sample-mean), but reciprocal sums $4/3$ and $1$, hence different [posterior means](../../../statistical-inference.md#posterior-mean). For any $n>2$, append the same positive observations to these two samples. For $n=1$, the estimate is $Cx/(1+\lambda x)$, with $C=(\alpha+k)/(k-1)$; its second [derivative](../../../calculus.md#derivative) is $-2C\lambda/(1+\lambda x)^3\ne0$, so it is not affine either. Symmetry in the observations would force equal slopes in any affine representation, so these examples also exclude a general fixed-coefficient linear representation.

One can express the [posterior mean](../../../statistical-inference.md#posterior-mean) as a broader data-dependent blend. With $A=\sum_i x_i^{-1}$ and [harmonic mean](../../../arithmetic.md#harmonic-mean) $H=n/A$, it is

$$
\widehat\mu_{\rm Bayes}=(1-Z_B)m+Z_B\frac{kH}{k-1},\qquad Z_B=\frac A{\lambda+A}.
$$

This weights a harmonic-mean-based experience estimate, and the weight itself depends on the observations. It is not the [credibility estimate](../../../actuarial-statistics.md#credibility-estimate) based on $\overline X$ and the fixed [Bühlmann credibility factor](../../../actuarial-statistics.md#credibility-factor) derived above.

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The ratio of [expected process variance](../../../actuarial-statistics.md#expected-process-variance) to [variance of hypothetical means](../../../actuarial-statistics.md#variance-of-hypothetical-means) is $K=s^2/v=(\alpha+1)/(k-2)$, and the [credibility factor](../../../actuarial-statistics.md#credibility-factor) is $Z=n/(n+K)$. Holding $\alpha,\lambda$ fixed, an increase in $k$ decreases $K$. Hence **the [credibility factor](../../../actuarial-statistics.md#credibility-factor) increases**, approaching one as $k$ tends to infinity. Extending the formula to real $k>2$ makes the sign explicit:

$$
\frac{\partial Z}{\partial k}=\frac{n(\alpha+1)}{[n(k-2)+\alpha+1]^2}>0.
$$

For the integer values in the model this establishes the same strict monotonicity. The collective claim [expected value](../../../probability-theory.md#expected-value) $m=\alpha/[\lambda(k-1)]$ also changes, but the conclusion concerns the relative weight of experience: conditional noise declines faster than the variation of the risk means.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Set $h=\mathbb E\theta>0$ and $w=\operatorname{Var}(\theta)>0$. Keeping $h$ fixed in the [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) family gives $\alpha=h^2/w$ and $\lambda=h/w$. The ratio of [expected process variance](../../../actuarial-statistics.md#expected-process-variance) to [variance of hypothetical means](../../../actuarial-statistics.md#variance-of-hypothetical-means) becomes

$$
K=\frac{h^2+w}{w(k-2)}=\frac{1+h^2/w}{k-2},\qquad
Z=\frac{n(k-2)}{n(k-2)+1+h^2/w}.
$$

As the prior [variance](../../../variance.md) $w$ decreases, $K$ increases, so **the [credibility factor](../../../actuarial-statistics.md#credibility-factor) decreases**. In the limit $w\downarrow0$, $Z\downarrow0$: the risk parameter is already essentially known from the prior, leaving little need to use the noisy [sample mean](../../../variance.md#sample-mean). The population claim [expected value](../../../probability-theory.md#expected-value) $h/(k-1)$ remains fixed throughout this comparison.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
