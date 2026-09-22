# Paper 43

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper43.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2005/Paper43.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)

## 1

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Condition on the [claim count](../../../actuarial-statistics.md#claim-count), defining the empty sum to be zero. [Independence](../../../random-variable.md#independent-random-variables) gives $\mathbb E[S\mid N=k]=k\mathbb E X_1$. By the [law of total expectation](../../../measure-theory.md#law-of-total-expectation),

$$
\boxed{\mathbb ES=\mathbb EN\,\mathbb EX_1.}
$$

For nonnegative claims this also follows from [Tonelli theorem](../../../measure-theory.md#tonelli-theorem); for signed claims finite $\mathbb EN$ and $\mathbb E|X_1|$ ensure [integrability](../../../measure-theory.md#integrability). [Conditional independence](../../../random-variable.md#conditional-independence) likewise gives

$$
\mathbb E[e^{tS}\mid N=k]=\prod_{j=1}^k\mathbb E[e^{tX_j}]=M_{X_1}(t)^k,
\qquad
\boxed{M_S(t)=G_N(M_{X_1}(t)).}
$$

This [random-sum transform identity](../../../actuarial-statistics.md#random-sum-transform-identity) holds wherever the composed series is finite, or as an extended nonnegative [expectation](../../../probability-theory.md#expected-value). It is not permission to use an algebraic continuation outside the convergence domain.

For the zero-based [geometric distribution](../../../discrete-probability-distribution.md#geometric-distribution), summing the [geometric series](../../../real-analysis.md#geometric-series) gives

$$
G_N(z)=\frac p{1-qz},\qquad \mathbb EN=G_N'(1)=\frac qp.
$$

The [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) of mean $\mu$ has $M_{X_1}(t)=(1-\mu t)^{-1}$ for $t<1/\mu$. Therefore

$$
\boxed{\mathbb ES=\frac{q\mu}p,\qquad
M_S(t)=\frac p{1-q/(1-\mu t)}
=\frac{p(1-\mu t)}{p-\mu t}\quad(t<p/\mu).}
$$

The stricter bound $t<p/\mu$ is necessary: the [geometric series](../../../real-analysis.md#geometric-series) requires $qM_{X_1}(t)<1$. At and above $p/\mu$ that series diverges; at and above $1/\mu$ even one claim has an infinite transform. Thus the displayed rational expression represents the [moment-generating function](../../../probability-theory.md#moment-generating-function) only on its stated domain.

Since all claims are strictly positive, $S=0$ exactly when $N=0$, so $\mathbb P(S=0)=p$. Splitting the transform gives

$$
M_S(t)=p+q\frac{p/\mu}{p/\mu-t}.
$$

Uniqueness of the [moment-generating function](../../../probability-theory.md#moment-generating-function) identifies a [mixture distribution](../../../probability-theory.md#mixture-distribution) with a zero atom of weight $p$ and an exponential positive component of weight $q$ and rate $p/\mu$. In particular,

$$
\boxed{\mathbb P(S=0)=p,\qquad f_S(x)=\frac{qp}{\mu}e^{-px/\mu}\quad(x>0).}
$$

The density integrates to $q$, not one. One can also verify it directly: conditional on $N=k\geq1$, the sum has [Erlang distribution](../../../continuous-probability-distribution.md#erlang-distribution) density $x^{k-1}e^{-x/\mu}/[\mu^k(k-1)!]$. Multiplying by $pq^k$ and summing over $k$ gives $(pq/\mu)e^{-x/\mu}e^{qx/\mu}$, the same density. This is the [zero-based geometric sum of exponential variables](../../../actuarial-statistics.md#zero-based-geometric-sum-of-exponential-variables).

Under [excess of loss reinsurance](../../../actuarial-statistics.md#excess-of-loss-reinsurance), the ceded amount for each claim is $(X_j-M)_+$, and the monthly reduction is their [random sum](../../../random-variable.md#random-sum). The [tail integral formula for moments](../../../probability-theory.md#tail-integral-formula-for-moments) gives

$$
\mathbb E(X_1-M)_+=\int_M^\infty\mathbb P(X_1>x)\,dx
=\mu e^{-M/\mu}.
$$

Conditioning on $N$ again yields

$$
\boxed{\mathbb E\sum_{j=1}^N(X_j-M)_+=\frac{q\mu}p e^{-M/\mu}.}
$$

The retained payment is $\sum_{j=1}^N\min(X_j,M)$; it is generally not $\min(S,M)$.

Under [aggregate stop loss reinsurance](../../../actuarial-statistics.md#aggregate-stop-loss-reinsurance), the reduction is $(S-\widetilde M)_+$. The aggregate tail is $\mathbb P(S>x)=q e^{-px/\mu}$ for $x\geq0$, so

$$
\mathbb E(S-\widetilde M)_+=\int_{\widetilde M}^\infty q e^{-px/\mu}\,dx
=\frac{q\mu}p e^{-p\widetilde M/\mu}.
$$

The prefactor is positive. Equality with the per-claim recovery is equivalent to $p\widetilde M=M$, giving the unique [reinsurance retention](../../../actuarial-statistics.md#reinsurance-retention)

$$
\boxed{\widetilde M=\frac Mp.}
$$

This is the relation for [equal expected recoveries from excess of loss and stop loss](../../../actuarial-statistics.md#equal-expected-recoveries-from-excess-of-loss-and-stop-loss); since $p<1$, the aggregate [reinsurance retention](../../../actuarial-statistics.md#reinsurance-retention) exceeds the individual [reinsurance retention](../../../actuarial-statistics.md#reinsurance-retention). These are reductions in claim payouts, before any reinsurance premium is deducted.

## 2

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Write $M(t)=\mathbb Ee^{tX}$, with $M(0)=1$, and differentiate $\kappa(t)=\log M(t)$:

$$
\begin{aligned}
\kappa'(t)&=\frac{M'(t)}{M(t)},\\
\kappa''(t)&=\frac{M''(t)}{M(t)}-\frac{M'(t)^2}{M(t)^2},\\
\kappa'''(t)&=\frac{M'''(t)}{M(t)}-\frac{3M'(t)M''(t)}{M(t)^2}
 +\frac{2M'(t)^3}{M(t)^3}.
\end{aligned}
$$

Using $M^{(j)}(0)=\mathbb EX^j$ and $\mu=\mathbb EX$ gives

$$
\boxed{\kappa_1=\mu,\qquad\kappa_2=\mathbb EX^2-\mu^2=\operatorname{Var}X,\qquad
\kappa_3=\mathbb EX^3-3\mu\mathbb EX^2+2\mu^3=\mathbb E(X-\mu)^3.}
$$

Thus the first three [cumulants](../../../probability-theory.md#cumulant) are the mean, [variance](../../../variance.md) and third [central moment](../../../probability-theory.md#central-moment). A finite [moment-generating function](../../../probability-theory.md#moment-generating-function) near zero justifies these differentiations. For positive claims with only three finite ordinary [moments](../../../probability-theory.md#moment), the same calculations are valid as left [derivatives](../../../calculus.md#derivative) at zero of the logarithm of the [Laplace transform of a nonnegative random variable](../../../probability-theory.md#laplace-transform-of-a-nonnegative-random-variable); positive [exponential moments](../../../probability-theory.md#exponential-moment) are not needed for the resulting [moment](../../../probability-theory.md#moment) identities.

For the independent [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) count, the [random-sum transform identity](../../../actuarial-statistics.md#random-sum-transform-identity) gives

$$
M_S(t)=\exp\{\lambda(M_{X_1}(t)-1)\},\qquad
\kappa_S(t)=\lambda(M_{X_1}(t)-1).
$$

Consequently the [compound Poisson distribution](../../../actuarial-statistics.md#compound-poisson-distribution) has

$$
\kappa_{S,1}=\lambda m_1,\qquad
\kappa_{S,2}=\lambda m_2,\qquad
\kappa_{S,3}=\lambda m_3.
$$

These are raw severity [moments](../../../probability-theory.md#moment), not severity [cumulants](../../../probability-theory.md#cumulant).

The printed gamma density uses rate $\nu$, not scale. Direct integration against $e^{ty}$ gives

$$
M_Y(t)=\left(\frac\nu{\nu-t}\right)^\alpha\quad(t<\nu),\qquad
\kappa_V(t)=kt-\alpha\log(1-t/\nu).
$$

Therefore the required matching equations for the [shifted gamma distribution](../../../continuous-probability-distribution.md#shifted-gamma-distribution) are

$$
k+\frac\alpha\nu=\lambda m_1,\qquad
\frac\alpha{\nu^2}=\lambda m_2,\qquad
\frac{2\alpha}{\nu^3}=\lambda m_3.
$$

For $\lambda>0$ and nonzero positive claims with finite $m_3$, these equations give positive $\alpha,\nu$ and the unique solution

$$
\boxed{\nu=\frac{2m_2}{m_3},\qquad
\alpha=\frac{4\lambda m_2^3}{m_3^2},\qquad
k=\lambda m_1-\frac{2\lambda m_2^2}{m_3}.}
$$

This is the [three-cumulant shifted gamma approximation](../../../actuarial-statistics.md#three-cumulant-shifted-gamma-approximation). In particular, its [skewness](../../../probability-theory.md#skewness) $2/\sqrt\alpha$ equals $m_3/(\sqrt\lambda\,m_2^{3/2})$, the [skewness](../../../probability-theory.md#skewness) of $S$.

The competing [normal approximation to a compound Poisson aggregate](../../../actuarial-statistics.md#normal-approximation-to-a-compound-poisson-aggregate) is

$$
\boxed{S\approx\mathcal N(\lambda m_1,\lambda m_2),\qquad
\mathbb P(S\leq x)\approx\Phi\!\left(\frac{x-\lambda m_1}{\sqrt{\lambda m_2}}\right).}
$$

To justify its large-count limit, let $\varphi_X$ be the claim [characteristic function](../../../probability-theory.md#characteristic-function). For fixed severity law with $m_2<\infty$, its expansion is $\varphi_X(u)=1+im_1u-m_2u^2/2+o(u^2)$. The [characteristic function](../../../probability-theory.md#characteristic-function) of $(S-\lambda m_1)/\sqrt{\lambda m_2}$ is

$$
\exp\left\{\lambda\left[\varphi_X\left(\frac t{\sqrt{\lambda m_2}}\right)-1\right]
-\frac{it\lambda m_1}{\sqrt{\lambda m_2}}\right\}
\longrightarrow e^{-t^2/2}.
$$

Thus it converges in distribution to a standard [normal distribution](../../../probability-theory.md#normal-distribution) as $\lambda\to\infty$.

The [normal approximation](../../../convergence-of-random-variables.md#normal-approximation) is simple, uses only $m_1,m_2$, and works well in the centre when the count is large and standardized [skewness](../../../probability-theory.md#skewness) is small. It imposes symmetry, whereas positive compound-Poisson claims have positive third [cumulant](../../../probability-theory.md#cumulant). The shifted-gamma approximation reproduces that third [cumulant](../../../probability-theory.md#cumulant) and can better describe moderate right [skewness](../../../probability-theory.md#skewness). It requires a finite and reliably known third [moment](../../../probability-theory.md#moment), and matching three [cumulants](../../../probability-theory.md#cumulant) alone does not guarantee accurate extreme tails.

Neither continuous approximation reproduces the genuine atom $\mathbb P(S=0)=e^{-\lambda}$, which matters at small $\lambda$. The [normal distribution](../../../probability-theory.md#normal-distribution) also assigns [probability](../../../probability-theory.md#probability) $\Phi(-\sqrt\lambda m_1/\sqrt{m_2})$ to negative losses. The gamma approximation is bounded below by $k$, but **its fitted shift need not be nonnegative**: exponential claims of mean $\mu$ give $k=-\lambda\mu/3$, so it too can assign mass to negative losses. If $k>0$, it instead excludes some genuinely possible small losses. These support and atom discrepancies prevent either approximation from being a universal replacement for the exact aggregate law.

## 3

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For the [Poisson process](../../../probability-theory.md#poisson-process) of claims and [relative safety loading](../../../actuarial-statistics.md#relative-safety-loading) $\rho$, the premium rate in the [classical risk model](../../../actuarial-statistics.md#classical-risk-model) is $c=(1+\rho)\lambda\mu$. Dividing the [adjustment coefficient](../../../actuarial-statistics.md#adjustment-coefficient) equation $\lambda(M(r)-1)=cr$ by $\lambda$ explains why the arrival rate cancels. Interpret $r_\infty$ as the upper endpoint of the finite [moment-generating function](../../../probability-theory.md#moment-generating-function) domain, so $M(r)<\infty$ for $0\leq r<r_\infty$ and its stated divergence occurs at that endpoint.

Set $F(r)=M(r)-1-(1+\rho)\mu r$. Then

$$
F(0)=0,\qquad F'(0)=-\rho\mu<0,\qquad
F''(r)=\mathbb E[X_1^2e^{rX_1}]>0\quad(0\leq r<r_\infty).
$$

Differentiation is valid inside the finite-transform domain, and its positive neighbourhood gives finite [moments](../../../probability-theory.md#moment) of every order. Thus $F$ is [strictly convex](../../../real-analysis.md#strictly-convex-function) and negative just to the right of zero. If $r_\infty<\infty$, divergence of $M(r)$ makes $F(r)\to\infty$ at the endpoint. If $r_\infty=\infty$, choose $a>0$ with $\mathbb P(X_1\geq a)>0$; then $M(r)\geq\mathbb P(X_1\geq a)e^{ar}$, which eventually exceeds every [linear function](../../../vector-space.md#linear-function). Again $F(r)\to\infty$. The [intermediate value theorem](../../../calculus.md#intermediate-value-theorem) gives a positive zero.

There is at most one positive zero: [strict convexity](../../../real-analysis.md#strictly-convex-function) and $F(0)=0$ make the secant slope $F(r)/r$ strictly increasing for $r>0$. It starts at $-\rho\mu$ and crosses zero exactly once. Hence

$$
\boxed{\text{There is a unique }R\in(0,r_\infty)\text{ with }M(R)-1=(1+\rho)\mu R.}
$$

This proves the [secant-slope existence criterion for an adjustment coefficient](../../../actuarial-statistics.md#secant-slope-existence-criterion-for-an-adjustment-coefficient) in the present setting.

Put $m_j=\mathbb EX_1^j$. For $u>0$, the positive remainder of the [exponential series](../../../calculus.md#exponential-series) gives $e^u>1+u+u^2/2$. Apply it to $u=RX_1$ and take [expectations](../../../probability-theory.md#expected-value):

$$
(1+\rho)\mu R=M(R)-1>\mu R+\frac{m_2R^2}{2}.
$$

Dividing by $R>0$ yields

$$
\boxed{R<r_1=\frac{2\rho\mu}{m_2}.}
$$

Keeping the cubic term similarly gives

$$
\rho\mu>\frac{m_2R}{2}+\frac{m_3R^2}{6}.
$$

The [polynomial](../../../polynomial.md) $g(r)=m_3r^2+3m_2r-6\rho\mu$ is strictly increasing for $r\geq0$, is negative at zero and tends to infinity. Let $r_2$ be its unique positive zero. The last inequality says $g(R)<0$, so

$$
\boxed{R<r_2=\frac{\sqrt{9m_2^2+24\rho\mu m_3}-3m_2}{2m_3},\qquad
g(r_2)=0.}
$$

Finally, $3m_2r_1=6\rho\mu$, whence $g(r_1)=m_3r_1^2>0$. Monotonicity gives $r_2<r_1$. Thus the requested [upper bounds](../../../set.md#upper-bound-in-a-partially-ordered-set) can in fact be sharpened to the strict ordering **$0<R<r_2<r_1$**. The bounds themselves need not lie in the finite-transform domain; the argument only evaluates the actual transform at $R$ and [polynomial](../../../polynomial.md) [moments](../../../probability-theory.md#moment) elsewhere. These are [polynomial moment bounds for the adjustment coefficient](../../../actuarial-statistics.md#polynomial-moment-bounds-for-the-adjustment-coefficient).

For rate-$\alpha$ [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) claims,

$$
\mu=\frac1\alpha,\qquad m_2=\frac2{\alpha^2},\qquad m_3=\frac6{\alpha^3},\qquad
M(r)=\frac\alpha{\alpha-r}\quad(r<\alpha).
$$

The positive root satisfies $1/(\alpha-R)=(1+\rho)/\alpha$ after dividing out $R$, so

$$
\boxed{R=\frac{\alpha\rho}{1+\rho},\qquad
r_1=\alpha\rho,\qquad
r_2=\frac\alpha2\left(\sqrt{1+4\rho}-1\right).}
$$

The cubic-bound equation reduces to $r_2^2+\alpha r_2-\rho\alpha^2=0$, selecting the displayed positive root. In particular $R<\alpha$, as required by the transform domain, for every $\rho>0$.

## 4

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [credibility estimate](../../../actuarial-statistics.md#credibility-estimate) combines a risk's observed experience with collective or [prior](../../../statistical-inference.md#prior-probability) information, typically as $Z\overline X+(1-Z)m_0$. The [credibility factor](../../../actuarial-statistics.md#credibility-factor) $Z\in[0,1]$ is the weight assigned to the individual experience: more reliable or more extensive data generally increases it. [Bayesian credibility](../../../actuarial-statistics.md#bayesian-credibility) treats the risk parameter as random with a [prior distribution](../../../statistical-inference.md#prior-probability) and predicts future claims by averaging the conditional claim mean under its [posterior distribution](../../../statistical-inference.md#bayesian-posterior). Under [squared-error loss](../../../statistical-inference.md#squared-error-loss) this [posterior predictive](../../../statistical-inference.md#posterior-predictive-distribution) mean is optimal. It need not be an [affine combination](../../../geometry-and-topology.md#affine-combination) in every Bayesian model; the [Poisson-gamma conjugacy](../../../statistical-inference.md#poisson-gamma-conjugacy) calculation below yields that credibility form exactly, rather than as a best-linear approximation.

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Let $s=\sum_{j=1}^n x_j$. The conditional joint [likelihood function](../../../statistical-modelling.md#likelihood-function) of the observed counts is

$$
L(\theta;\mathbf x)=\prod_{j=1}^n\frac{e^{-\theta}\theta^{x_j}}{x_j!}
=\frac{e^{-n\theta}\theta^s}{\prod_jx_j!}.
$$

The [prior](../../../statistical-inference.md#prior-probability) is a [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) with shape two and rate $\lambda$. Multiplication by its density gives the unnormalized [posterior density](../../../statistical-inference.md#posterior-density) $\theta^{s+1}e^{-(n+\lambda)\theta}$. Normalizing with the [gamma function](../../../complex-analysis.md#gamma-function) yields

$$
\pi(\theta\mid\mathbf x)=\frac{(n+\lambda)^{s+2}}{\Gamma(s+2)}
\theta^{s+1}e^{-(n+\lambda)\theta},\qquad\theta>0.
$$

Thus [Poisson-gamma conjugacy](../../../statistical-inference.md#poisson-gamma-conjugacy) gives $\Theta\mid\mathbf x\sim\operatorname{Gamma}(s+2,n+\lambda)$. Conditional on $\Theta$ and the past data, the next count has mean $\Theta$, so the [law of total expectation](../../../measure-theory.md#law-of-total-expectation) gives

$$
\boxed{\mathbb E[X_{n+1}\mid\mathbf x]=\mathbb E[\Theta\mid\mathbf x]=\frac{s+2}{n+\lambda}.}
$$

With $\overline x=s/n$ and [prior](../../../statistical-inference.md#prior-probability) mean $m_0=2/\lambda$, this is exactly

$$
\boxed{\frac{s+2}{n+\lambda}
=Z\overline x+(1-Z)m_0,\qquad Z=\frac n{n+\lambda}.}
$$

Here $n\geq1$, $\lambda>0$, and the [credibility factor](../../../actuarial-statistics.md#credibility-factor) increases to one as the number of observed years grows. The denominator uses the [prior](../../../statistical-inference.md#prior-probability) rate $\lambda$ and total exposure $n$; it does not add two to the exposure when adding the [prior](../../../statistical-inference.md#prior-probability) shape.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Given $\Theta=\theta$, the sum of the independent yearly counts is $S_n\sim\operatorname{Poisson}(n\theta)$: their [probability generating functions](../../../probability-theory.md#probability-generating-function) multiply to $\exp(n\theta(z-1))$. Averaging this conditional law over the [prior](../../../statistical-inference.md#prior-probability) gives the [mixed Poisson distribution](../../../discrete-probability-distribution.md#mixed-poisson-distribution)

$$
\boxed{p_n(s):=\mathbb P(S_n=s)
=\frac{n^s}{s!}\int_0^\infty e^{-n\theta}\theta^s\pi(\theta)\,d\theta,\qquad s\geq0.}
$$

The likelihood for the full vector depends on $\theta$ only through $s$, so $S_n$ is a [sufficient statistic](../../../probability-and-statistics.md#sufficient-statistic); conditioning on the total or on the full observed vector gives the same [posterior](../../../statistical-inference.md#bayesian-posterior) for $\Theta$.

For an event of positive [probability](../../../probability-theory.md#probability) $p_n(s)>0$, the [posterior density](../../../statistical-inference.md#posterior-density) is proportional to $e^{-n\theta}\theta^s\pi(\theta)$. Put $I_s=\int_0^\infty e^{-n\theta}\theta^s\pi(\theta)\,d\theta$. Its mean is $I_{s+1}/I_s$. The future count has [conditional mean](../../../measure-theory.md#conditional-expectation) $\Theta$, so

$$
\begin{aligned}
\mathbb E[X_{n+1}\mid S_n=s]
&=\frac{I_{s+1}}{I_s}\\
&=\frac{(s+1)!\,p_n(s+1)/n^{s+1}}{s!\,p_n(s)/n^s}
=\boxed{\frac{(s+1)\mathbb P(S_n=s+1)}{n\mathbb P(S_n=s)}}.
\end{aligned}
$$

This is the [posterior mean from adjacent mixed Poisson probabilities](../../../discrete-probability-distribution.md#posterior-mean-from-adjacent-mixed-poisson-probabilities). Both [probabilities](../../../probability-theory.md#probability) refer to the same $n$-year exposure; the numerator is not a [probability](../../../probability-theory.md#probability) for $S_{n+1}$. For a proper [prior](../../../statistical-inference.md#prior-probability) and $n>0$, the integrals defining this [posterior mean](../../../statistical-inference.md#posterior-mean) are finite because $\theta^{s+1}e^{-n\theta}$ is bounded on $[0,\infty)$.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Insert the shape-two gamma [prior](../../../statistical-inference.md#prior-probability) into the integral from part (ii). The [gamma function](../../../complex-analysis.md#gamma-function) integral gives

$$
\begin{aligned}
p_n(s)
&=\frac{n^s\lambda^2}{s!}\int_0^\infty\theta^{s+1}e^{-(n+\lambda)\theta}\,d\theta\\
&=\frac{n^s\lambda^2\Gamma(s+2)}{s!(n+\lambda)^{s+2}}\\
&=\boxed{(s+1)\left(\frac\lambda{n+\lambda}\right)^2
\left(\frac n{n+\lambda}\right)^s},\qquad s=0,1,\ldots.
\end{aligned}
$$

Therefore $S_n$ has a [negative binomial distribution](../../../discrete-probability-distribution.md#negative-binomial-distribution) with shape two and success [probability](../../../probability-theory.md#probability) $\lambda/(n+\lambda)$, using the failures-before-two-successes convention. This is the [Poisson-gamma mixture](../../../discrete-probability-distribution.md#poisson-gamma-mixture). The identity $\sum_{s\geq0}(s+1)z^s=(1-z)^{-2}$ verifies that the [probabilities](../../../probability-theory.md#probability) sum to one.

Its adjacent [probability](../../../probability-theory.md#probability) ratio is

$$
\frac{p_n(s+1)}{p_n(s)}=\frac{s+2}{s+1}\frac n{n+\lambda}.
$$

Substituting in the [posterior](../../../statistical-inference.md#bayesian-posterior) formula gives

$$
\boxed{\mathbb E[X_{n+1}\mid S_n=s]=\frac{s+2}{n+\lambda},}
$$

exactly the estimate from part (i). The equality is required by sufficiency, and the direct computation confirms that the two negative-binomial and gamma parameter conventions have been used consistently.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2005](../../2005.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
