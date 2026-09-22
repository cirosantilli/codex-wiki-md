# Paper 33

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper33.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper33.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Write $C=\int_{\mathbb R}f(x)\,dx$, so $0<C<\infty$. The finite envelope condition means that $f\leq Mg$ almost everywhere; in particular, the proposal must cover the support of the target.

For each [independent](../../../random-variable.md#independent-random-variables) proposal $Y\sim g$, generate an [independent](../../../random-variable.md#independent-random-variables) $U\sim\operatorname{Unif}(0,1)$ and accept $Y$ precisely when

$$
\boxed{U\leq\frac{f(Y)}{Mg(Y)}.}
$$

Discard a rejected proposal and continue. The ratio is in $[0,1]$ and is needed only where $g(Y)>0$. Neither evaluation of $C$ nor prior knowledge of the normalized target is required.

To prove the output law, for any measurable set $D$ the joint [probability](../../../probability-theory.md#probability) of acceptance and a proposal in $D$ is

$$
\mathbb P(Y\in D,\mathrm{accept})
=\int_Dg(y)\frac{f(y)}{Mg(y)}\,dy
=\frac1M\int_Df(y)\,dy.
$$

Dividing by the total acceptance [probability](../../../probability-theory.md#probability) $C/M$ gives $\int_D f(y)/C\,dy$, the target [probability](../../../probability-theory.md#probability). [Independent](../../../random-variable.md#independent-random-variables) proposal-uniform pairs give [independent](../../../random-variable.md#independent-random-variables) accepted observations. With a finite proposal list there can be no accepted value; with continued [independent](../../../random-variable.md#independent-random-variables) trials, acceptance eventually occurs almost surely because $C/M>0$.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

The [acceptance mass for an unnormalized rejection envelope](../../../probability-and-statistics.md#acceptance-mass-for-an-unnormalized-rejection-envelope) follows by integrating the proposal-specific acceptance [probability](../../../probability-theory.md#probability):

$$
\boxed{p_{\rm acc}=\mathbb E_g\!\left[\frac{f(Y)}{Mg(Y)}\right]
=\frac CM.}
$$

The inequality $f\leq Mg$ also gives $C\leq M$, so this is a valid [probability](../../../probability-theory.md#probability). It is the same at every [independent](../../../random-variable.md#independent-random-variables) trial.

If $J_i$ indicates acceptance of the $i$th proposal, then $J_1,\ldots,J_n$ are [independent](../../../random-variable.md#independent-random-variables) [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution) variables with parameter $C/M$. Hence the accepted count $K=\sum_iJ_i$ satisfies

$$
K\sim\operatorname{Bin}\!\left(n,\frac CM\right),
\qquad
\boxed{\mathbb EK=\frac{nC}{M}=\frac nM\int_{\mathbb R}f(y)\,dy.}
$$

Its [variance](../../../variance.md) is $np_{\rm acc}(1-p_{\rm acc})$. Conditional on any acceptance pattern, the accepted values have [independent](../../../random-variable.md#independent-random-variables) target [probability density function](../../../continuous-probability-distribution.md#probability-density-function) $h$; mixing over patterns retains this product law conditional on their count.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For [normal rejection sampling with an exponential envelope](../../../probability-and-statistics.md#normal-rejection-sampling-with-an-exponential-envelope), complete the square in the [probability density function](../../../continuous-probability-distribution.md#probability-density-function) ratio:

$$
\frac{h(x)}{g(x)}
=\frac{\sqrt{2/\pi}}{\lambda}
\exp\!\left(-\frac{x^2}{2}+\lambda x\right)
=\frac{\sqrt{2/\pi}}{\lambda}e^{\lambda^2/2}
e^{-(x-\lambda)^2/2}.
$$

The maximum occurs at $x=\lambda$, which lies in the support because $\lambda>0$. Thus

$$
\boxed{M(\lambda)=\frac{\sqrt{2/\pi}}{\lambda}e^{\lambda^2/2}
=\sqrt{\frac{2e^{\lambda^2}}{\pi\lambda^2}}.}
$$

The PDF exponent is $e^{\lambda^2}$ inside the square root; this distinction is lost in the converted TeX.

The acceptance rule simplifies to

$$
U\leq e^{-(Y-\lambda)^2/2},
\qquad Y\sim\operatorname{Exp}(\lambda).
$$

An exponential proposal can be generated as $Y=-\lambda^{-1}\log V$ from an [independent](../../../random-variable.md#independent-random-variables) [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) value $V$. Since the target is normalized, the overall acceptance [probability](../../../probability-theory.md#probability) is $1/M(\lambda)$. To maximize it,

$$
\frac{d}{d\lambda}\log M=\lambda-\lambda^{-1},
\qquad
\frac{d^2}{d\lambda^2}\log M=1+\lambda^{-2}>0.
$$

Therefore **the optimal rate is $\lambda=1$**, with acceptance [probability](../../../probability-theory.md#probability) $\sqrt{\pi/(2e)}$.

Finally, give each accepted [half-normal distribution](../../../probability-theory.md#half-normal-distribution) value $Y$ an [independent](../../../random-variable.md#independent-random-variables) fair sign $R\in\{-1,1\}$ and output $Z=RY$. On each half-line its [probability density function](../../../continuous-probability-distribution.md#probability-density-function) is half the reflected [half-normal distribution](../../../probability-theory.md#half-normal-distribution) [probability density function](../../../continuous-probability-distribution.md#probability-density-function):

$$
p_Z(z)=\frac12h(|z|)=\frac1{\sqrt{2\pi}}e^{-z^2/2}.
$$

Consequently **$Z\sim N(0,1)$**. The sign must be drawn independently; rejection itself does not supply it.

## 2

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

For the [Metropolis–Hastings algorithm](../../../statistical-inference.md#metropolis-hastings-algorithm), start at a point $x$ with positive target [probability density function](../../../continuous-probability-distribution.md#probability-density-function). Draw $Y$ from a proposal [probability density function](../../../continuous-probability-distribution.md#probability-density-function) $q(y\mid x)$, generate an [independent](../../../random-variable.md#independent-random-variables) [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) value $U$, and set the next state to $Y$ if

$$
U\leq\alpha(x,Y),\qquad
\boxed{\alpha(x,y)=\min\!\left\{1,\frac{\pi(y)q(x\mid y)}{\pi(x)q(y\mid x)}\right\}.}
$$

Otherwise retain $x$, including that repeated state in the sample. Where a proposed forward move is possible but its reverse [probability density function](../../../continuous-probability-distribution.md#probability-density-function) vanishes, its acceptance [probability](../../../probability-theory.md#probability) is zero. Unknown [normalizing constants](../../../continuous-probability-distribution.md#normalizing-constant) in $\pi$ cancel.

For distinct states, the accepted [probability](../../../probability-theory.md#probability) flow is

$$
\pi(x)q(y\mid x)\alpha(x,y)
=\min\{\pi(x)q(y\mid x),\pi(y)q(x\mid y)\},
$$

which is symmetric in $x,y$. This [detailed balance](../../../markov-process.md#detailed-balance) identity, together with the holding [probability](../../../probability-theory.md#probability), proves that $\pi$ is invariant. Under appropriate irreducibility and aperiodicity conditions the chain converges to $\pi$; successive states are generally dependent.

The [Gibbs sampler](../../../statistical-inference.md#gibbs-sampler) updates coordinates from their [full conditional distributions](../../../probability-theory.md#full-conditional-distribution). In a systematic sweep, draw successively

$$
X_j^{(r)}\sim
\pi\!\left(\,\cdot\mid X_1^{(r)},\ldots,X_{j-1}^{(r)},
X_{j+1}^{(r-1)},\ldots,X_k^{(r-1)}\right),
\quad j=1,\ldots,k.
$$

Each update preserves the target joint law: integrating the old coordinate against its conditional [probability density function](../../../continuous-probability-distribution.md#probability-density-function) and replacing it by an [independent](../../../random-variable.md#independent-random-variables) draw from that same conditional leaves the joint [probability density function](../../../continuous-probability-distribution.md#probability-density-function) unchanged. The composition of the coordinate updates therefore also preserves $\pi$. A [Gibbs sampler](../../../statistical-inference.md#gibbs-sampler) coordinate move can be regarded as a [Metropolis–Hastings algorithm](../../../statistical-inference.md#metropolis-hastings-algorithm) move with acceptance [probability](../../../probability-theory.md#probability) one. Systematic sweeps preserve [stationarity](../../../time-series.md#stationary-process) but need not themselves be reversible. Initialization away from [stationarity](../../../time-series.md#stationary-process) requires convergence before treating the draws as approximately target-distributed, and dependence must be accounted for in [Monte Carlo method](../../../probability-and-statistics.md#monte-carlo-method) error estimates.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Assume $\sigma_1,\sigma_2>0$ and $|\rho|<1$, as required for the displayed nonsingular [probability density function](../../../continuous-probability-distribution.md#probability-density-function). Put $z_j=(x_j-\mu_j)/\sigma_j$. Its quadratic exponent is

$$
Q(x)=\frac{z_1^2-2\rho z_1z_2+z_2^2}{1-\rho^2}
=\frac{(z_1-\rho z_2)^2}{1-\rho^2}+z_2^2.
$$

Holding $x_2$ fixed and normalizing the term depending on $x_1$ gives

$$
\boxed{X_1\mid X_2=x_2\sim
N\!\left(\mu_1+\rho\frac{\sigma_1}{\sigma_2}(x_2-\mu_2),
\sigma_1^2(1-\rho^2)\right).}
$$

The analogous completion of the square gives

$$
\boxed{X_2\mid X_1=x_1\sim
N\!\left(\mu_2+\rho\frac{\sigma_2}{\sigma_1}(x_1-\mu_1),
\sigma_2^2(1-\rho^2)\right).}
$$

Using [independent](../../../random-variable.md#independent-random-variables) draws $\eta_{1,r},\eta_{2,r}$ from the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution), a sweep is

$$
X_1^{(r)}=\mu_1+\rho\frac{\sigma_1}{\sigma_2}(X_2^{(r-1)}-\mu_2)
+\sigma_1\sqrt{1-\rho^2}\,\eta_{1,r},
$$



$$
X_2^{(r)}=\mu_2+\rho\frac{\sigma_2}{\sigma_1}(X_1^{(r)}-\mu_1)
+\sigma_2\sqrt{1-\rho^2}\,\eta_{2,r}.
$$

Use the newly drawn first coordinate in the second update. Recording the pairs after each sweep gives the dependent sample.

The [Gaussian Gibbs sweep autocorrelation](../../../statistical-inference.md#gaussian-gibbs-sweep-autocorrelation) makes the dependence explicit. In standardized coordinates, substitution yields

$$
Z_{2,r}=\rho^2Z_{2,r-1}
+\sqrt{1-\rho^2}(\rho\eta_{1,r}+\eta_{2,r}).
$$

The new noise has [variance](../../../variance.md) $1-\rho^4$, so the stationary [variance](../../../variance.md) is one and the lag-$h$ sweep [autocorrelation](../../../time-series.md#autocorrelation) is $\rho^{2h}$. Thus the sampler converges geometrically for $|\rho|<1$, but becomes slow near perfect [correlation](../../../variance.md#pearson-correlation-coefficient). When $\rho=0$, complete sweeps yield [independent](../../../random-variable.md#independent-random-variables) pairs. The singular cases $|\rho|=1$ do not have the stipulated two-dimensional [probability density function](../../../continuous-probability-distribution.md#probability-density-function).

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

Here the proposal is $Y=x+\eta$ with $\eta\sim N_2(0,I_2)$. Its [probability density function](../../../continuous-probability-distribution.md#probability-density-function) depends only on $\|y-x\|^2$, so $q(y\mid x)=q(x\mid y)$. The determinant and [normalizing constant](../../../continuous-probability-distribution.md#normalizing-constant) of the target also cancel. With $Q$ as in the preceding entry,

$$
\boxed{\alpha(x,y)=\min\{1,e^{-[Q(y)-Q(x)]/2}\}.}
$$

Equivalently, writing $u_j=(y_j-\mu_j)/\sigma_j$ and $z_j=(x_j-\mu_j)/\sigma_j$,

$$
\alpha(x,y)=\min\!\left\{1,
\exp\!\left[-\frac{
u_1^2-2\rho u_1u_2+u_2^2-z_1^2+2\rho z_1z_2-z_2^2
}{2(1-\rho^2)}\right]\right\}.
$$

One can also compute the exponent without subtracting two large [quadratic forms](../../../linear-algebra.md#quadratic-form):

$$
\log\frac{\pi(x+\eta)}{\pi(x)}
=-\eta^\top\Sigma^{-1}(x-\mu)-\frac12\eta^\top\Sigma^{-1}\eta.
$$

Generate two [independent](../../../random-variable.md#independent-random-variables) [standard normal distribution](../../../probability-theory.md#standard-normal-distribution) proposal increments, compute this log ratio, and accept when $\log U\leq\min(0,\log(\pi(Y)/\pi(x)))$. Retain the previous pair on rejection. [Detailed balance](../../../markov-process.md#detailed-balance) gives the correct [invariant distribution](../../../markov-process.md#stationary-distribution), and the everywhere-positive [Gaussian](../../../probability-theory.md#normal-distribution) proposal makes this [Random-walk Metropolis algorithm](../../../statistical-inference.md#random-walk-metropolis-algorithm) chain irreducible; a rejection [probability](../../../probability-theory.md#probability) provides a holding step. The resulting target-distributed pairs are dependent, with proposal scale and target anisotropy controlling how quickly they mix.

## 3

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Write $\sigma_\varepsilon^2$ for the driving [white noise](../../../time-series.md#white-noise) [variance](../../../variance.md) and $\Theta(z)=1+\sum_{\ell=1}^q\theta_\ell z^\ell$. The [autoregressive polynomial](../../../time-series.md#autoregressive-polynomial) factors as

$$
\Phi(z)=1-\frac56z+\frac16z^2
=(1-z/2)(1-z/3).
$$

The [discrete Gaussian white noise](../../../time-series.md#discrete-gaussian-white-noise) values are [independent](../../../random-variable.md#independent-random-variables). The roots of $\Phi$ are outside the [unit disc](../../../topology.md#unit-disc), so expanding $\Theta(z)/\Phi(z)$ gives an absolutely summable [causal time-series representation](../../../time-series.md#causal-time-series-representation). Hence $x_t$ is a centered [Gaussian](../../../probability-theory.md#normal-distribution) process formed from driving [white noise](../../../time-series.md#white-noise) values at times at most $t$. In particular, for $k>q$, every driving [white noise](../../../time-series.md#white-noise) value $\varepsilon_{t-\ell}$ with $\ell\leq q$ is [independent](../../../random-variable.md#independent-random-variables) of $x_{t-k}$. The [autocovariance tail recurrence of a causal ARMA process](../../../time-series.md#autocovariance-tail-recurrence-of-a-causal-arma-process) follows by taking [covariance](../../../variance.md#covariance) of the recursion with $x_{t-k}$:

$$
\boxed{\gamma_k-\frac56\gamma_{k-1}+\frac16\gamma_{k-2}=0\qquad(k>q).}
$$

The roots of the [characteristic polynomial](../../../linear-operator-theory.md#characteristic-polynomial) of this tail recurrence are $1/2$ and $1/3$. Let $k_0=\max(q-1,0)$. There exist constants $c,d$ such that

$$
\gamma_k=c\,2^{-k}+d\,3^{-k}\qquad(k\geq k_0).
$$

For example, put $a=6\gamma_{k_0+1}-2\gamma_{k_0}$ and $b=3\gamma_{k_0}-6\gamma_{k_0+1}$; then $c=2^{k_0}a$ and $d=3^{k_0}b$ reproduce the two starting values and therefore the whole recurrence. Choose $C$ strictly larger than $|c|+|d|$ and all the finitely many values $2^k|\gamma_k|$ with $0\leq k<k_0$. Symmetry $\gamma_{-k}=\gamma_k$ now gives

$$
\boxed{|\gamma_k|<C\,2^{-|k|}\quad(k\in\mathbb Z).}
$$

For negative $k$ this is stronger than the requested bound with $2^{-k}$. It also proves $\sum_{k\geq1}k|\gamma_k|<\infty$.

For the Fourier calculation, take $D=2m+1$ positive and $T=DN$ positive. The supplied equal-norm trigonometric identities require $j\not\equiv0\pmod D$; the usual intended range is $1\leq j\leq m$. Because $D$ is odd, $2j\not\equiv0\pmod D$ at every such nonzero frequency. The [geometric series](../../../real-analysis.md#geometric-series) of $e^{i\omega t}$ and $e^{2i\omega t}$ over $T$ terms vanish. They imply

$$
\sum_{t=1}^T c_ts_t=0,\qquad
\sum_{t=1}^T c_t^2=\sum_{t=1}^Ts_t^2=T/2,
\qquad c_t=\cos(\omega t),\quad s_t=\sin(\omega t).
$$

Other integer values of $j$ reduce modulo $D$; folding a negative frequency changes the sine coefficient only by a sign. The permitted zero frequency is handled below.

Grouping the double [expectation](../../../probability-theory.md#expected-value) sum according to the time lag yields

$$
\mathbb E(AB)
=\frac1{\pi T}\sum_{t,u=1}^T\gamma_{u-t}c_ts_u
=\frac1{\pi T}\left[
\gamma_0\sum_{t=1}^Tc_ts_t+
\sum_{k=1}^{T-1}\gamma_k
\left(\sum_{t=1}^{T-k}c_ts_{t+k}+\sum_{t=k+1}^Tc_ts_{t-k}\right)\right].
$$

Replace the two truncated sums for lag $k$ by full sums. Their total is

$$
\sum_{t=1}^Tc_t(s_{t+k}+s_{t-k})
=2\cos(\omega k)\sum_{t=1}^Tc_ts_t=0.
$$

Each replacement adds at most $k$ terms, each of absolute value at most one. This gives the [finite-record Fourier covariance bound](../../../time-series.md#finite-record-fourier-covariance-bound):

$$
\boxed{|\mathbb E(AB)|\leq\frac1{\pi T}\sum_{k=1}^{T-1}2k|\gamma_k|
=O(T^{-1})\longrightarrow0.}
$$

Both coefficients have [expected value](../../../probability-theory.md#expected-value) zero, so this [expectation](../../../probability-theory.md#expected-value) is their [covariance](../../../variance.md#covariance).

For each finite $T$, $(A,B)$ has a [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution) because it is a [linear transformation](../../../vector-space.md#linear-map) of the [Gaussian](../../../probability-theory.md#normal-distribution) observation vector. If the [variances](../../../variance.md) converge to $v_A,v_B$, its [characteristic function](../../../probability-theory.md#characteristic-function) converges to

$$
\exp\!\left[-\frac12(v_Au^2+v_Bv^2)\right],
$$

since the cross-covariance tends to zero. This is the [characteristic function](../../../probability-theory.md#characteristic-function) of two [independent](../../../random-variable.md#independent-random-variables) centered normal variables; zero limiting [variances](../../../variance.md) are allowed.

We can calculate the [variance](../../../variance.md) limits rather than merely assume their existence. Grouping the cosine [covariance](../../../variance.md#covariance) sum gives

$$
\mathbb EA^2=\frac1{\pi T}
\left[\gamma_0\sum_tc_t^2+
2\sum_{k=1}^{T-1}\gamma_k\sum_{t=1}^{T-k}c_tc_{t+k}\right].
$$

Over a full record, $\sum_{t=1}^Tc_tc_{t+k}=(T/2)\cos(\omega k)$. Truncation changes this by at most $k$. The same statements hold for the sine products. Consequently

$$
\mathbb EA^2=
\frac{\gamma_0}{2\pi}+\frac1\pi\sum_{k=1}^{T-1}\gamma_k\cos(k\omega)+R_{A,T},
\qquad
|R_{A,T}|\leq\frac2{\pi T}\sum_{k=1}^{T-1}k|\gamma_k|,
$$

and the identical main term and bound apply to $\mathbb EB^2$. Absolute summability now gives

$$
\boxed{\lim\mathbb EA^2=\lim\mathbb EB^2
=\frac{\gamma_0+2\sum_{k\geq1}\gamma_k\cos(k\omega)}{2\pi}.}
$$

Specify the spectral convention to identify this limit. Let

$$
f_2(\omega)=\frac1{2\pi}\sum_{k\in\mathbb Z}\gamma_ke^{-ik\omega},
\qquad
s(\omega)=2f_2(\omega)=
\frac{\gamma_0+2\sum_{k\geq1}\gamma_k\cos(k\omega)}{\pi}.
$$

Here $f_2$ is the two-sided [probability density function](../../../continuous-probability-distribution.md#probability-density-function) on $[-\pi,\pi]$, and $s$ is the one-sided [probability density function](../../../continuous-probability-distribution.md#probability-density-function) on $[0,\pi]$, satisfying $\gamma_k=\int_0^\pi s(\omega)\cos(k\omega)\,d\omega$. Thus each [variance](../../../variance.md) limit is $f_2(\omega)=s(\omega)/2$. For this particular model, the filter representation also gives

$$
s(\omega)=\frac{\sigma_\varepsilon^2}{\pi}
\frac{|\Theta(e^{-i\omega})|^2}
{|1-e^{-i\omega}/2|^2\,|1-e^{-i\omega}/3|^2}.
$$

For the specified squared-sum estimator, an exact [expectation](../../../probability-theory.md#expected-value) calculation uses $c_tc_u+s_ts_u=\cos(\omega(t-u))$:

$$
\mathbb EI(\omega)=
\frac1\pi\left[\gamma_0+
2\sum_{k=1}^{T-1}\left(1-\frac kT\right)\gamma_k\cos(k\omega)\right].
$$

The missing tail and the $k/T$ terms vanish; indeed the bias is $O(T^{-1})$ by the exponential [covariance](../../../variance.md#covariance) bound. Therefore **$I(\omega)$ is asymptotically unbiased for the one-sided [probability density function](../../../continuous-probability-distribution.md#probability-density-function) $s(\omega)$**. Under the common two-sided convention its limit in [expectation](../../../probability-theory.md#expected-value) is $2f_2(\omega)$, so $I(\omega)/2$ is the appropriately normalized estimator.

At an interior frequency with $s(\omega)>0$, the joint [Gaussian](../../../probability-theory.md#normal-distribution) limit gives the [exponential limit of a one-sided periodogram](../../../time-series.md#exponential-limit-of-a-one-sided-periodogram):

$$
\boxed{\frac{I(\omega)}{s(\omega)}
\xrightarrow{d}\frac{\chi_2^2}{2}=\operatorname{Exp}(1).}
$$

Moreover, for a centered [Gaussian](../../../probability-theory.md#normal-distribution) pair,

$$
\operatorname{Var}(A^2+B^2)
=2(\operatorname{Var}A)^2+2(\operatorname{Var}B)^2
+4\operatorname{Cov}(A,B)^2
\longrightarrow s(\omega)^2.
$$

The nondegenerate exponential limiting law rules out [convergence in probability](../../../convergence-of-random-variables.md#convergence-in-probability) to $s(\omega)$. Thus **the unsmoothed [periodogram](../../../time-series.md#periodogram) is not [consistent](../../../statistical-inference.md#consistency-statistics) at frequencies with positive spectrum**, despite its asymptotic unbiasedness. If $s(\omega)=0$, the nonnegative estimator has [expectation](../../../probability-theory.md#expected-value) tending to zero and is [consistent](../../../statistical-inference.md#consistency-statistics) there by [Markov's inequality](../../../probability-inequality.md#markov-inequality). Smoothing an increasing number of nearby ordinates while shrinking the frequency bandwidth can remove the positive-spectrum [variance](../../../variance.md) obstruction.

For $j\equiv0\pmod D$, the sine coefficient is identically zero and the cosine coefficient is the normalized sum of the observations. The corrected limits are

$$
\mathbb EB^2=0,\qquad
\mathbb EA^2\longrightarrow
\frac{\gamma_0+2\sum_{k\geq1}\gamma_k}{\pi}=s(0).
$$

The joint limit is $(N(0,s(0)),0)$, [independent](../../../random-variable.md#independent-random-variables) in the degenerate sense. The exact [expectation](../../../probability-theory.md#expected-value) formula for $I$ still applies and tends to $s(0)$, but now $I(0)/s(0)\xrightarrow{d}\chi_1^2$ when $s(0)>0$, with limiting [variance](../../../variance.md) $2s(0)^2$. The estimator is again inconsistent. This covers the zero frequency allowed by the printed inequality on $j$.

<a id="3/image-normalized-one-sided-periodograms-remain-dispersed-as-the-record-length-increases"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-33-periodogram.png)

**[Figure 1](#3/image-normalized-one-sided-periodograms-remain-dispersed-as-the-record-length-increases). Normalized one-sided periodograms remain dispersed as the record length increases**.

The figure uses the allowed cancellation $\Theta=\Phi$, so the observations reduce to [white noise](../../../time-series.md#white-noise). Orthogonal Fourier projections give the exponential law exactly at each plotted record length; increasing the record does not narrow the individual [periodogram](../../../time-series.md#periodogram) ordinate.

## 4

↑ **Parent:** [Paper 33](paper-33.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For the [three-coordinate state realization of an ARMA(1,1) process](../../../time-series.md#three-coordinate-state-realization-of-an-arma-1-1-process), the observation row and transition [matrix](../../../vector-space.md#matrix) are

$$
\boxed{F=(\phi,1,\theta),\qquad
G=\begin{pmatrix}\phi&1&\theta\\0&0&0\\0&1&0\end{pmatrix}.}
$$

The first row of $GS_{t-1}$ is $x_{t-1}$ by the previous-time recursion; the second row is zero until the new [white noise](../../../time-series.md#white-noise) value is added; and the third row copies $\varepsilon_{t-1}$. Hence the state equation has noise [covariance](../../../variance.md#covariance)

$$
Q=\operatorname{Cov}(w_t)
=\begin{pmatrix}0&0&0\\0&\sigma^2&0\\0&0&0\end{pmatrix}.
$$

We use the causal state model, in which the new driving noise is independent of the previous state. The [Gaussian filtering with exact observations](../../../control-theory.md#gaussian-filtering-with-exact-observations) form of the [Kalman filter](../../../control-theory.md#kalman-filter) alternates prediction through the state equation with conditioning on the next observation. Given the posterior [expected value](../../../probability-theory.md#expected-value) and [covariance](../../../variance.md#covariance) at time $t-1$, [independence](../../../random-variable.md#independent-random-variables) of the new [white noise](../../../time-series.md#white-noise) value gives predictive [expected value](../../../probability-theory.md#expected-value) $a_t=G\widehat S_{t-1}$ and predictive [covariance](../../../variance.md#covariance)

$$
R_t=GP_{t-1}G^\top+Q.
$$

Project through the observation row to get

$$
\widehat x_t=Fa_t,\qquad
\boxed{V_t=FR_tF^\top=FGP_{t-1}G^\top F^\top+\sigma^2.}
$$

The residual $v_t=x_t-\widehat x_t$ is the [innovation](../../../time-series.md#innovation-process). Conditioning the joint [Gaussian](../../../probability-theory.md#normal-distribution) state-observation vector adjusts the [expected value](../../../probability-theory.md#expected-value) according to this residual and reduces the [covariance](../../../variance.md#covariance). In this exact-observation model, the updates can be written

$$
K_t=\frac{R_tF^\top}{V_t},\qquad
\widehat S_t=a_t+K_tv_t,\qquad
P_t=R_t-\frac{R_tF^\top FR_t}{V_t}.
$$

Thus $F\widehat S_t=x_t$ and $FP_tF^\top=0$: the observed [linear combination](../../../vector-space.md#linear-combination) of the state is now known exactly, though other state combinations remain uncertain.

The PDF's stated prediction [variance](../../../variance.md) omits $FQF^\top=\sigma^2$. This omission cannot be used in a valid [likelihood](../../../statistical-modelling.md#likelihood-function): for the AR(1) specialization below it would give zero prediction [variance](../../../variance.md) after the first observation. The required [likelihood](../../../statistical-modelling.md#likelihood-function) calculation uses the corrected [innovation](../../../time-series.md#innovation-process) [variance](../../../variance.md) just derived.

For [stationary initialization of an ARMA(1,1) state](../../../time-series.md#stationary-initialization-of-an-arma-1-1-state) with $|\phi|<1$, take $\widehat S_0=0$ and the unconditional stationary [covariance](../../../variance.md#covariance). The causal coefficients are $1$ at lag zero and $(\phi+\theta)\phi^{j-1}$ at lags $j\geq1$, giving

$$
\gamma_0=\operatorname{Var}(x_t)
=\sigma^2\left[1+\frac{(\phi+\theta)^2}{1-\phi^2}\right]
=\frac{\sigma^2(1+\theta^2+2\phi\theta)}{1-\phi^2}.
$$

Since $S_0=(x_{-1},\varepsilon_0,\varepsilon_{-1})^\top$, the cross-covariance with $\varepsilon_0$ is zero and that with $\varepsilon_{-1}$ is $\sigma^2$. Therefore

$$
\boxed{P_0=
\begin{pmatrix}
\gamma_0&0&\sigma^2\\
0&\sigma^2&0\\
\sigma^2&0&\sigma^2
\end{pmatrix}.}
$$

Direct substitution verifies $P_0=GP_0G^\top+Q$. If prior state information is available, instead use its conditional [expected value](../../../probability-theory.md#expected-value) and [covariance](../../../variance.md#covariance). A diffuse initialization is another option when the initial state is genuinely unknown, but it changes the finite-sample [likelihood](../../../statistical-modelling.md#likelihood-function) and should not silently replace the stationary initial law.

By the [Gaussian](../../../probability-theory.md#normal-distribution) prediction step,

$$
x_t\mid x_1,\ldots,x_{t-1}\sim N(\widehat x_t,V_t).
$$

The [chain rule for probabilities](../../../probability-theory.md#chain-rule-for-probabilities) for the joint [probability density function](../../../continuous-probability-distribution.md#probability-density-function) therefore gives

$$
L(\phi,\theta,\sigma^2)
=\prod_{t=1}^T(2\pi V_t)^{-1/2}
\exp\!\left[-\frac{(x_t-\widehat x_t)^2}{2V_t}\right].
$$

Taking minus twice its logarithm shows that **[maximum likelihood estimation](../../../statistical-modelling.md#maximum-likelihood-estimation) is equivalent to minimizing**

$$
\boxed{\sum_{t=1}^T\left[\log(2\pi)+\log V_t+
\frac{(x_t-\widehat x_t)^2}{V_t}\right],}
$$

with each $V_t$ and $\widehat x_t$ evaluated at the candidate parameters and the specified initialization. The corrected $+\sigma^2$ is essential in every $V_t$.

For the stationary causal AR(1) case, $\theta=0$ and $|\phi|<1$. The first observation is $N(0,\sigma^2/(1-\phi^2))$, whereas each later conditional observation is $\phi x_{t-1}+\varepsilon_t$. Hence

$$
\boxed{V_1=\frac{\sigma^2}{1-\phi^2},
\qquad V_t=\sigma^2\quad(2\leq t\leq T).}
$$

This also gives a direct counterexample to the uncorrected PDF [variance](../../../variance.md): with $\theta=0$, $FG=\phi F$ and $FP_{t-1}F^\top=0$ after observing $x_{t-1}$, so its printed expression would give $V_t=0$ for $t\geq2$.

To compare the [conditional and stationary AR1 likelihood estimators](../../../time-series.md#conditional-and-stationary-ar1-likelihood-estimators), put

$$
Q_T(\phi)=(1-\phi^2)x_1^2+
\sum_{t=2}^T(x_t-\phi x_{t-1})^2.
$$

Then its negative twice log-likelihood is

$$
T\log(2\pi)+T\log\sigma^2-\log(1-\phi^2)+
\frac{Q_T(\phi)}{\sigma^2}.
$$

For fixed $\phi$, $\widehat{\sigma^2}=Q_T(\phi)/T$. Writing

$$
C_T=\sum_{t=2}^Tx_{t-1}^2,\qquad
D_T=\sum_{t=2}^Tx_tx_{t-1},
$$

the exact interior score equation is

$$
0=\frac{\phi}{1-\phi^2}+
\frac{\phi(C_T-x_1^2)-D_T}{\sigma^2}.
$$

The stationary initial contribution is order one for a fixed interior parameter, while $C_T$ is order $T$. Discarding this lower-order contribution gives

$$
\boxed{\widehat\phi\approx
\frac{D_T}{C_T}
=\frac{\sum_{t=2}^Tx_tx_{t-1}}{\sum_{t=2}^Tx_{t-1}^2}.}
$$

Conditioning on $x_1$ makes this ratio the exact unconstrained [conditional maximum likelihood](../../../statistical-modelling.md#conditional-maximum-likelihood) estimate. Under the stationary initial law it is only the leading approximation: at an interior optimum,

$$
\widehat\phi-\frac{D_T}{C_T}
=\frac{\widehat\phi}{C_T}
\left(x_1^2-\frac{\widehat{\sigma^2}}{1-\widehat\phi^2}\right)
=O_{\mathbb P}(T^{-1}).
$$

This approximation presumes a nondegenerate sample denominator and a true coefficient fixed away from the unit-root boundary; a finite-sample constrained optimum must respect $|\phi|<1$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
