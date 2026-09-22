# Paper 43

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper43.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper43.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Write $P(z)=\mathbb E[z^N]$, $F(z)=\mathbb E[z^{X_1}]$ and $G(z)=\mathbb E[z^{S_N}]$ for the three [probability generating functions](../../../probability-theory.md#probability-generating-function). Since both the claim count and every claim size are positive, $P(0)=F(0)=G(0)=0$. Conditioning on the count and using [independence](../../../random-variable.md#independent-random-variables) gives the [random-sum transform identity](../../../actuarial-statistics.md#random-sum-transform-identity)

$$
G(z)=\sum_{n\ge1}p_n F(z)^n=P(F(z)).
$$

The crucial point is that the count recurrence begins at $n=2$. Multiplying it by $n z^{n-1}$ and summing, we obtain

$$
\begin{aligned}
P'(z)-p_1
&=\sum_{n\ge2}(an+b)p_{n-1}z^{n-1}\\
&=\sum_{m\ge1}(a(m+1)+b)p_mz^m\\
&=azP'(z)+(a+b)P(z).
\end{aligned}
$$

Consequently $(1-az)P'(z)=(a+b)P(z)+p_1$. The [chain rule](../../../calculus.md#chain-rule) applied to the aggregate [probability generating function](../../../probability-theory.md#probability-generating-function) therefore gives

$$
(1-aF(z))G'(z)=\big((a+b)G(z)+p_1\big)F'(z).
$$

These identities hold inside the unit disk, or as identities of [formal power series](../../../commutative-algebra.md#formal-power-series). Since $F(0)=0$, every coefficient of the composition depends on only finitely many count probabilities.

Compare the coefficient of $z^{k-1}$. The product $FG'$ contributes $\sum_{j=1}^{k-1}(k-j)f_jg_{k-j}$, and $F'G$ contributes $\sum_{j=1}^{k-1}j f_jg_{k-j}$. Hence

$$
k g_k=p_1 k f_k+\sum_{j=1}^{k-1}\big(a(k-j)+(a+b)j\big)f_jg_{k-j}.
$$

The required [aggregate recursion for zero-truncated Panjer counts](../../../probability-theory.md#aggregate-recursion-for-zero-truncated-panjer-counts) is **initialized by $g_0=0$ and $g_1=p_1f_1$**, and for every $k\ge1$ it is

$$
\boxed{g_k=p_1f_k+\sum_{j=1}^{k-1}\left(a+\frac{bj}{k}\right)f_jg_{k-j}.}
$$

The empty sum at $k=1$ is zero. Every term on the right is known or has a smaller aggregate index. Omitting $p_1f_k$ would incorrectly apply the usual [Panjer recursion](../../../actuarial-statistics.md#panjer-recursion) with a zero initial value, producing zero for every aggregate probability.

For the [zero-truncated Poisson distribution](../../../discrete-probability-distribution.md#zero-truncated-poisson-distribution), $p_n/p_{n-1}=\lambda/n$ for $n\ge2$, so $a=0$, $b=\lambda$ and $p_1=\lambda/(e^\lambda-1)$, with $\lambda>0$. Thus

$$
\boxed{g_k=\frac{\lambda}{e^\lambda-1}f_k+\frac{\lambda}{k}\sum_{j=1}^{k-1}j f_jg_{k-j},\qquad k\ge1.}
$$

As a direct [probability generating function](../../../probability-theory.md#probability-generating-function) check, $P(z)=(e^{\lambda z}-1)/(e^\lambda-1)$ and therefore $G(z)=(e^{\lambda F(z)}-1)/(e^\lambda-1)$; differentiation reproduces this recursion.

## 2

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The claim-size [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) has [expected value](../../../probability-theory.md#expected-value) $\mu>0$ and [moment-generating function](../../../probability-theory.md#moment-generating-function)

$$
M_X(t)=\int_0^\infty e^{tx}\frac1\mu e^{-x/\mu}\,dx=\frac1{1-\mu t},\qquad t<1/\mu.
$$

Conditional on $N_i=k$, [independence](../../../random-variable.md#independent-random-variables) makes the aggregate [moment-generating function](../../../probability-theory.md#moment-generating-function) equal to $M_X(t)^k$. Averaging over the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) of the count gives

$$
\begin{aligned}
M_{S_i}(t)
&=\sum_{k\ge0}e^{-\lambda_i}\frac{\lambda_i^k}{k!}M_X(t)^k\\
&=\exp\big(\lambda_i(M_X(t)-1)\big)
=\boxed{\exp\left(\frac{\lambda_i\mu t}{1-\mu t}\right)}.
\end{aligned}
$$

Put $\Lambda=\sum_{i=1}^n\lambda_i$. For fixed intensities, [independence](../../../random-variable.md#independent-random-variables) between risks gives

$$
M_S(t)=\prod_{i=1}^n M_{S_i}(t)
=\exp\big(\Lambda(M_X(t)-1)\big).
$$

This is precisely the transform of a [compound Poisson distribution](../../../actuarial-statistics.md#compound-poisson-distribution). Indeed the [addition of independent Poisson random variables](../../../discrete-probability-distribution.md#addition-of-independent-poisson-random-variables) makes the total count [Poisson distributed](../../../discrete-probability-distribution.md#poisson-distribution) with parameter $\Lambda$, and every claim in the pooled portfolio has the same [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution). Thus **the portfolio aggregate is compound Poisson with intensity $\sum_i\lambda_i$ and exponential claim sizes of mean $\mu$.**

Now regard the individual intensities as independent [gamma distributed](../../../continuous-probability-distribution.md#gamma-distribution) quantities, with shape $m\ge1$ and rate $\alpha$. Their [moment-generating functions](../../../probability-theory.md#moment-generating-function) are $(\alpha/(\alpha-t))^m$ for $t<\alpha$. Multiplying these transforms proves [additivity of independent gamma distributions with a common rate](../../../continuous-probability-distribution.md#additivity-of-independent-gamma-distributions-with-a-common-rate):

$$
\boxed{\Lambda\sim\operatorname{Gamma}(nm,\text{rate }\alpha),\qquad f_\Lambda(\ell)=\frac{\alpha^{nm}}{\Gamma(nm)}\ell^{nm-1}e^{-\alpha\ell},\quad \ell>0.}
$$

Conditional on the individual intensities, the total count $N$ has [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) with parameter $\Lambda$. Because this conditional law depends only on their sum, it is also the law of $N$ conditional on $\Lambda$. Integrating its [probability mass function](../../../probability-theory.md#probability-mass-function) against the [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) density yields

$$
\begin{aligned}
\mathbb P(N=k)
&=\frac{\alpha^{nm}}{k!\,\Gamma(nm)}\int_0^\infty \ell^{nm+k-1}e^{-(\alpha+1)\ell}\,d\ell\\
&=\frac{\Gamma(nm+k)}{k!\,\Gamma(nm)}\frac{\alpha^{nm}}{(\alpha+1)^{nm+k}}\\
&=\boxed{\binom{nm+k-1}{k}\left(\frac{\alpha}{\alpha+1}\right)^{nm}\left(\frac1{\alpha+1}\right)^k},\qquad k\ge0.
\end{aligned}
$$

Thus **the total count has a [negative binomial distribution](../../../discrete-probability-distribution.md#negative-binomial-distribution) with shape $nm$ and success probability $\alpha/(\alpha+1)$**, using the convention that counts failures before the specified number of successes. Its [probability generating function](../../../probability-theory.md#probability-generating-function) is $(\alpha/(\alpha+1-z))^{nm}$.

Conditional on $\Lambda$, the claim sizes retain their common [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) and the amount $S$ has a [compound Poisson distribution](../../../actuarial-statistics.md#compound-poisson-distribution) of intensity $\Lambda$. Therefore **the unconditional amount has a [compound mixed Poisson distribution](../../../actuarial-statistics.md#compound-mixed-poisson-distribution) with gamma mixing intensity of shape $nm$ and rate $\alpha$**. To make the mixture explicit, average the conditional aggregate [moment-generating function](../../../probability-theory.md#moment-generating-function):

$$
\begin{aligned}
M_S(t)
&=\mathbb E\exp\big(\Lambda(M_X(t)-1)\big)\\
&=\left(\frac{\alpha}{\alpha-(M_X(t)-1)}\right)^{nm}
=\boxed{\left(\frac{\alpha(1-\mu t)}{\alpha-(\alpha+1)\mu t}\right)^{nm}},
\qquad t<\frac{\alpha}{(\alpha+1)\mu}.
\end{aligned}
$$

The displayed domain ensures both the severity transform and the intensity transform are finite. The mixing distribution describes the Poisson intensity, not the claim sizes. In particular, the aggregate has an atom at zero of mass $\mathbb P(N=0)=(\alpha/(\alpha+1))^{nm}$.

## 3

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

In the [classical risk model](../../../actuarial-statistics.md#classical-risk-model), the insurer's surplus is

$$
U(t)=u+ct-C(t),\qquad C(t)=\sum_{j=1}^{N(t)}X_j,
$$

where $u\ge0$ is initial capital, $N(t)$ is a [Poisson process](../../../probability-theory.md#poisson-process) of rate $\lambda>0$, and the claim sizes are positive [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables) with [expected value](../../../probability-theory.md#expected-value) $\mu$, independent of the claim-arrival process. Premium flows in at constant rate $c$. A positive [relative safety loading](../../../actuarial-statistics.md#relative-safety-loading) $\theta$ means

$$
\boxed{c=(1+\theta)\lambda\mu,\qquad\theta>0,}
$$

so premium income exceeds the expected claim cost per unit time. The ruin [stopping time](../../../martingale.md#stopping-time) is $\tau=\inf\{t\ge0:U(t)<0\}$, with $\tau=\infty$ if ruin never occurs, and the [ultimate ruin probability](../../../actuarial-statistics.md#ultimate-ruin-probability) is $\psi(u)=\mathbb P(\tau<\infty)$.

Assume the stated positive [adjustment coefficient](../../../actuarial-statistics.md#adjustment-coefficient) $R$ exists and that the claim [moment-generating function](../../../probability-theory.md#moment-generating-function) is finite at $R$. The [Lundberg inequality](../../../actuarial-statistics.md#lundberg-inequality) is

$$
\boxed{\psi(u)\le e^{-Ru},\qquad u\ge0.}
$$

Here is a proof, including the stopping argument. By conditioning on the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) of $N(t)$, the [random-sum transform identity](../../../actuarial-statistics.md#random-sum-transform-identity) gives

$$
\mathbb E e^{rC(t)}=\exp\big(\lambda t(M(r)-1)\big).
$$

The [adjustment coefficient](../../../actuarial-statistics.md#adjustment-coefficient) equation is $\lambda(M(R)-1)=cR$. Consequently the [exponential surplus martingale](../../../actuarial-statistics.md#exponential-surplus-martingale)

$$
Z_t=\exp\big(R(C(t)-ct)\big),\qquad Z_0=1,
$$

has [expected value](../../../probability-theory.md#expected-value) one at every finite time. More strongly, the claim process has [independent increments](../../../stochastic-process.md#independent-increments), so for $s\le t$,

$$
\begin{aligned}
\mathbb E[Z_t\mid\mathcal F_s]
&=Z_s\,\mathbb E\exp\big(R(C(t)-C(s)-c(t-s))\big)\\
&=Z_s\exp\big((t-s)(\lambda(M(R)-1)-cR)\big)=Z_s.
\end{aligned}
$$

Thus $Z$ is a nonnegative [continuous-time martingale](../../../martingale.md#continuous-time-martingale) for the filtration generated by arrivals and claim sizes. For a fixed finite horizon $T$, the [optional stopping theorem](../../../martingale.md#optional-sampling-theorem-for-a-supermartingale) at the bounded [stopping time](../../../martingale.md#stopping-time) $\tau\wedge T$ gives $\mathbb E Z_{\tau\wedge T}=1$. This bounded use is legitimate: the stopped values belong to the closed [martingale](../../../martingale.md) on $[0,T]$ given by conditional expectations of the integrable variable $Z_T$.

On $\{\tau\le T\}$, the surplus is negative, and therefore $C(\tau)-c\tau=u-U(\tau)>u$. By nonnegativity on the complementary event,

$$
1=\mathbb E Z_{\tau\wedge T}
\ge \mathbb E\big[Z_\tau\mathbf1_{\{\tau\le T\}}\big]
\ge e^{Ru}\mathbb P(\tau\le T).
$$

The ruin events increase to $\{\tau<\infty\}$ as $T$ increases, so continuity of [probability](../../../probability-theory.md#probability) gives the claimed [Lundberg inequality](../../../actuarial-statistics.md#lundberg-inequality). No expectation identity at the unbounded [stopping time](../../../martingale.md#stopping-time) $\tau$ is needed. Positive loading by itself does not guarantee a positive [adjustment coefficient](../../../actuarial-statistics.md#adjustment-coefficient) for every claim law; the existence assumption is used here.

For the [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) of claim sizes, $M(r)=1/(1-\mu r)$ for $r<1/\mu$. Substitution in the [adjustment coefficient](../../../actuarial-statistics.md#adjustment-coefficient) equation gives

$$
\frac{\mu r}{1-\mu r}=(1+\theta)\mu r.
$$

Discard the zero root and divide by $\mu r$. The unique positive solution is

$$
\boxed{R=\frac{\theta}{(1+\theta)\mu}},
$$

which lies strictly inside the finite-transform domain.

For deterministic claim sizes, the claim [moment-generating function](../../../probability-theory.md#moment-generating-function) is $e^{\mu r}$. Define $h(r)=e^{\mu r}-1-(1+\theta)\mu r$. It satisfies $h(0)=0$, $h'(0)=-\theta\mu<0$, $h''(r)=\mu^2e^{\mu r}>0$, and $h(r)\to\infty$ as $r\to\infty$. Thus its strict [convexity](../../../real-analysis.md#convex-function) gives exactly one positive zero $R_\mu$, with $h(r)<0$ for $0<r<R_\mu$.

Put $x=\mu R=\theta/(1+\theta)\in(0,1)$. Since $-\log(1-x)>x$, we have $e^x<1/(1-x)$. Hence

$$
h(R)=e^{\mu R}-1-(1+\theta)\mu R
<\frac1{1-\mu R}-1-(1+\theta)\mu R=0.
$$

It follows that

$$
\boxed{R<R_\mu,\qquad e^{-R_\mu u}<e^{-Ru}\quad(u>0).}
$$

Thus **the deterministic-claim [Lundberg inequality](../../../actuarial-statistics.md#lundberg-inequality) provides a smaller upper bound at positive capital**; at zero capital both bounds equal one. This is a special case of [deterministic claims maximize the adjustment coefficient at fixed mean and loading](../../../actuarial-statistics.md#deterministic-claims-maximize-the-adjustment-coefficient-at-fixed-mean-and-loading): fixing the mean and loading, variability lowers the exponential decay coefficient relative to deterministic claims. The ordering of these upper bounds alone is not a proof that the actual [ultimate ruin probabilities](../../../actuarial-statistics.md#ultimate-ruin-probability) are ordered.

## 4

↑ **Parent:** [Paper 43](paper-43.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $M=\sum_{i=1}^n m_i$ be the total exposure, and define the [prior distribution](../../../statistical-inference.md#prior-probability) [expected value](../../../probability-theory.md#expected-value), prior [variance](../../../variance.md) and average binomial noise by

$$
\eta=\mathbb E\theta,\qquad v=\operatorname{Var}(\theta),\qquad w=\mathbb E[\theta(1-\theta)].
$$

Since the [prior distribution](../../../statistical-inference.md#prior-probability) has a [probability density function](../../../continuous-probability-distribution.md#probability-density-function) on $(0,1)$, $v>0$ and $w>0$. All relevant [moments](../../../probability-theory.md#moment) exist because the parameter and observations are bounded. The [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) gives

$$
\mathbb E[X_i\mid\theta]=\theta,\qquad
\operatorname{Var}(X_i\mid\theta)=\frac{\theta(1-\theta)}{m_i}.
$$

The [law of total expectation](../../../measure-theory.md#law-of-total-expectation), [law of total variance](../../../probability-theory.md#law-of-total-variance) and [law of total covariance](../../../variance.md#law-of-total-covariance) consequently yield

$$
\mathbb E X_i=\eta,\quad
\operatorname{Var}(X_i)=v+\frac{w}{m_i},\quad
\operatorname{Cov}(X_i,X_j)=v\ (i\ne j),\quad
\operatorname{Cov}(\theta,X_i)=v.
$$

In particular, [conditional independence](../../../random-variable.md#conditional-independence) of the annual observations does not imply unconditional [independence](../../../random-variable.md#independent-random-variables): they share the uncertain parameter.

To derive the optimal [credibility estimate](../../../actuarial-statistics.md#credibility-estimate) among [affine functions](../../../vector-space.md#affine-function) of the observations, put $A=\sum_i a_i$ and write $X_i=\theta+\varepsilon_i$. The conditional errors have zero [conditional expectation](../../../measure-theory.md#conditional-expectation), [conditional variance](../../../variance.md#conditional-variance) $\theta(1-\theta)/m_i$, and zero pairwise conditional [covariances](../../../variance.md#covariance). They are also uncorrelated with every integrable function of $\theta$. Therefore the joint [mean squared error](../../../statistical-modelling.md#mean-squared-error) is

$$
\begin{aligned}
L(a_0,a_1,\ldots,a_n)
&=\mathbb E\left[\big((1-A)\theta-a_0-\sum_i a_i\varepsilon_i\big)^2\right]\\
&=((1-A)\eta-a_0)^2+v(1-A)^2+w\sum_i\frac{a_i^2}{m_i}.
\end{aligned}
$$

For fixed slopes, the first term is uniquely minimized by $a_0=(1-A)\eta$. For fixed sum $A$, the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) gives

$$
A^2=\left(\sum_i\frac{a_i}{\sqrt{m_i}}\sqrt{m_i}\right)^2
\le M\sum_i\frac{a_i^2}{m_i},
$$

with equality exactly when $a_i=A m_i/M$. Thus the remaining optimization is the strictly convex quadratic

$$
v(1-A)^2+\frac{w}{M}A^2.
$$

Its derivative vanishes at $A=Mv/(Mv+w)$. Consequently the [Bühlmann–Straub credibility estimate](../../../actuarial-statistics.md#buhlmann-straub-credibility-estimate) is

$$
\boxed{\widehat\theta=Z\frac{\sum_i m_iX_i}{M}+(1-Z)\eta,\qquad
Z=\frac{Mv}{Mv+w}=\frac{M}{M+w/v}.}
$$

The individual coefficients are $a_i=Zm_i/M$ and $a_0=(1-Z)\eta$. The strict quadratic minimizations establish global optimality and uniqueness, not just necessary equations. Here $v$ is the [variance of hypothetical means](../../../actuarial-statistics.md#variance-of-hypothetical-means), $w$ is the [expected process variance](../../../actuarial-statistics.md#expected-process-variance), and $Z$ is the [Bühlmann–Straub credibility factor](../../../actuarial-statistics.md#buhlmann-straub-credibility-factor). More exposure gives more weight to the observed claim fraction. Since $0<Z<1$, the estimate remains between the observed pooled fraction and the prior [expected value](../../../probability-theory.md#expected-value). If one separately permits a degenerate prior, $v=0$ leads to the constant estimate $\eta$, interpreted as $Z=0$.

For the [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) prior on $(0,1)$,

$$
\eta=\frac12,\qquad v=\frac1{12},\qquad
w=\int_0^1\theta(1-\theta)\,d\theta=\frac16.
$$

With two years, put $M=m_1+m_2$ and $s=Y_1+Y_2=m_1X_1+m_2X_2$. Then $Z=M/(M+2)$ and

$$
\boxed{\widehat\theta=\frac{s+1}{M+2}
=\frac{m_1X_1+m_2X_2+1}{m_1+m_2+2}.}
$$

To compare with the [Bayes estimator under squared error loss](../../../statistical-inference.md#bayes-estimator-under-squared-error-loss), use [conditional independence](../../../random-variable.md#conditional-independence) to multiply the two binomial [likelihood functions](../../../statistical-modelling.md#likelihood-function). Terms independent of $\theta$ cancel on normalization, and the uniform prior makes the [posterior density](../../../statistical-inference.md#posterior-density) proportional to $\theta^s(1-\theta)^{M-s}$. Hence [Beta-binomial conjugacy](../../../statistical-inference.md#beta-binomial-conjugacy) gives

$$
\theta\mid(Y_1,Y_2)\sim\operatorname{Beta}(s+1,M-s+1),\qquad
\mathbb E[\theta\mid Y_1,Y_2]=\frac{s+1}{M+2}.
$$

Finally, for an arbitrary reported value $d$, conditional [quadratic loss](../../../statistical-inference.md#squared-error-loss) decomposes as

$$
\mathbb E[(\theta-d)^2\mid Y_1,Y_2]
=\operatorname{Var}(\theta\mid Y_1,Y_2)
+\big(d-\mathbb E[\theta\mid Y_1,Y_2]\big)^2.
$$

The unique minimum is the [posterior mean](../../../statistical-inference.md#posterior-mean). Therefore **the affine [credibility estimate](../../../actuarial-statistics.md#credibility-estimate) and the exact Bayesian estimate coincide** in this case. The agreement illustrates [exact beta-binomial credibility with unequal exposures](../../../actuarial-statistics.md#exact-beta-binomial-credibility-with-unequal-exposures); for a general [prior distribution](../../../statistical-inference.md#prior-probability), minimizing over [affine functions](../../../vector-space.md#affine-function) of the observations need not recover the unrestricted [posterior mean](../../../statistical-inference.md#posterior-mean).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
