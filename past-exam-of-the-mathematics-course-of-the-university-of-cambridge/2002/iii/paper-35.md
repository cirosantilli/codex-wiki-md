# Paper 35

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper35.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper35.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)

## 1

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Condition on the [claim count](../../../actuarial-statistics.md#claim-count). The empty [random sum of independent claims](../../../actuarial-statistics.md#random-sum-of-independent-claims) is zero, and independence gives $\mathbb E[e^{tS}\mid N=n]=M_X(t)^n$. Therefore the [random-sum transform identity](../../../actuarial-statistics.md#random-sum-transform-identity) is

$$
\boxed{M_S(t)=\sum_{n=0}^{\infty}\mathbb P(N=n)M_X(t)^n=G_N(M_X(t)),}
$$

wherever the composition is finite. This follows directly from the [law of total expectation](../../../measure-theory.md#law-of-total-expectation), rather than replacing the random count by its mean.

Put $q=1-p$. For the specified [negative binomial distribution](../../../discrete-probability-distribution.md#negative-binomial-distribution), the [negative binomial series](../../../real-analysis.md#negative-binomial-series) gives $G_N(z)=[p/(1-qz)]^k$. A rate-$\lambda$ [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) has [moment-generating function](../../../probability-theory.md#moment-generating-function) $M_X(t)=\lambda/(\lambda-t)$. Hence

$$
M_S(t)=\left(\frac{p(\lambda-t)}{p\lambda-t}\right)^k
=\left(p+q\frac{p\lambda}{p\lambda-t}\right)^k,\qquad t<p\lambda.
$$

The last expression is exactly the [moment-generating function](../../../probability-theory.md#moment-generating-function) of a [compound binomial distribution](../../../actuarial-statistics.md#compound-binomial-distribution) with independent count and severities

$$
\boxed{\widetilde N\sim\operatorname{Binomial}(k,1-p),\qquad\widetilde X_j\sim\operatorname{Exp}(p\lambda).}
$$

The [moment-generating function](../../../probability-theory.md#moment-generating-function) exists in a neighborhood of zero, so its uniqueness identifies the distributions. In particular, the new [claim sizes](../../../actuarial-statistics.md#claim-size) have mean $1/(p\lambda)$, not $1/\lambda$, and both aggregate distributions have an atom $p^k$ at zero. This is the [negative-binomial sum of exponential claims](../../../actuarial-statistics.md#negative-binomial-sum-of-exponential-claims) representation with the severity rate explicitly retained.

Conditional on $N=n\ge1$, the aggregate has [Erlang distribution](../../../continuous-probability-distribution.md#erlang-distribution) with density $\lambda^n s^{n-1}e^{-\lambda s}/(n-1)!$ on $s>0$. Repeated [integration by parts](../../../calculus.md#integration-by-parts) of its tail gives

$$
\mathbb P(S>x\mid N=n)=e^{-\lambda x}\sum_{j=0}^{n-1}\frac{(\lambda x)^j}{j!}.
$$

Indeed, after substituting $v=\lambda s$, the integral $\int_{\lambda x}^{\infty}e^{-v}v^{n-1}\,dv/(n-1)!$ reduces recursively to the corresponding integral with exponent $n-2$, terminating at $e^{-\lambda x}$. Applying the [law of total probability](../../../probability-theory.md#law-of-total-probability) yields the original infinite [mixture distribution](../../../probability-theory.md#mixture-distribution) tail

$$
\mathbb P(S>x)=\sum_{n=1}^{\infty}p_n e^{-\lambda x}\sum_{j=0}^{n-1}\frac{(\lambda x)^j}{j!},\qquad x>0.
$$

Applying the same argument to the [compound binomial distribution](../../../actuarial-statistics.md#compound-binomial-distribution) gives instead the [finite Erlang-mixture tail for a negative-binomial exponential aggregate](../../../actuarial-statistics.md#finite-erlang-mixture-tail-for-a-negative-binomial-exponential-aggregate):

$$
\boxed{\mathbb P(\widetilde S>x)=\sum_{n=1}^{k}\binom{k}{n}q^n p^{k-n}e^{-p\lambda x}\sum_{j=0}^{n-1}\frac{(p\lambda x)^j}{j!}.}
$$

The two tails are equal. **The binomial representation replaces an infinite sum by a finite exact calculation**, eliminating the need to choose a claim-count truncation and control its omitted tail. The inner sums can be evaluated recursively, using $a_{j+1}=a_j(p\lambda x)/(j+1)$ for their exponential-weighted terms.

## 2

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Write the surplus in the [classical risk model](../../../actuarial-statistics.md#classical-risk-model) as $U_t=u+ct-\sum_{j=1}^{N_t}X_j$, with premium rate $c=(1+\rho)\lambda\mu$. The [adjustment coefficient](../../../actuarial-statistics.md#adjustment-coefficient) is the positive solution of

$$
\lambda\bigl(M_X(R)-1\bigr)=cR.
$$

For the [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) of mean $\mu$, $M_X(r)=(1-\mu r)^{-1}$ for $r<1/\mu$. Cancelling the nonzero root $R$ in its equation gives $\lambda\mu/(1-\mu R)=c$, and hence

$$
\boxed{R=\frac{\rho}{(1+\rho)\mu}.}
$$

It is strictly between zero and $1/\mu$, as required by the transform domain.

The [ultimate ruin probability](../../../actuarial-statistics.md#ultimate-ruin-probability) is $\psi(u)=\mathbb P(\inf_{t\ge0}U_t<0)$. The [Lundberg inequality](../../../actuarial-statistics.md#lundberg-inequality) states

$$
\boxed{\psi(u)\le e^{-Ru}.}
$$

Ruin can occur only at a claim arrival. Thus the event defining the [finite-claim ruin probability](../../../actuarial-statistics.md#finite-claim-ruin-probability) $\psi_n(u)$ is contained in the ultimate ruin event, giving $\psi_n(u)\le\psi(u)\le e^{-Ru}$ for every $n\ge1$ and $u>0$.

For the explicit calculations, take $\mu=1$, put $d=1+\rho=c/\lambda$ and $h=d+1=2+\rho$, and let $T$ be the first arrival time. It has rate-$\lambda$ [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution), independent of the severity. Ruin on the first claim is the event $X_1>u+cT$, so

$$
\boxed{\psi_1(u)=\mathbb E[e^{-(u+cT)}]=e^{-u}\frac{\lambda}{\lambda+c}=\frac{e^{-u}}h.}
$$

For ruin by the second claim, condition on whether the first claim ruins the insurer or leaves capital $u+cT-x$. The independent future arrivals and severities have the same law as a fresh [classical risk model](../../../actuarial-statistics.md#classical-risk-model). Therefore

$$
\begin{aligned}
\psi_2(u)&=\psi_1(u)+\int_0^\infty\lambda e^{-\lambda t}\int_0^{u+ct}e^{-x}\psi_1(u+ct-x)\,dx\,dt\\
&=\frac{e^{-u}}h+\frac{e^{-u}}h\int_0^\infty\lambda e^{-(\lambda+c)t}(u+ct)\,dt\\
&=\boxed{e^{-u}\left(\frac1h+\frac{u}{h^2}+\frac{d}{h^3}\right).}
\end{aligned}
$$

The two terms in the first line refer to disjoint ruin events, so there is no double counting.

For a direct check of the [Lundberg inequality](../../../actuarial-statistics.md#lundberg-inequality), now $R=1-1/d$. The ratio $\psi_1(u)/e^{-Ru}=h^{-1}e^{-u/d}$ is less than one. For the second [finite-claim ruin probability](../../../actuarial-statistics.md#finite-claim-ruin-probability), put $A=h^{-1}+dh^{-3}$ and $B=h^{-2}$. Its ratio is $e^{-u/d}(A+Bu)$. Since

$$
A-dB=\frac{2d+1}{h^3}>0,\qquad 1-A=\frac{d(h^2-1)}{h^3}>0,
$$

the derivative of this ratio is $e^{-u/d}[B-(A+Bu)/d]<0$ for $u\ge0$, and its value at zero is $A<1$. This verifies both required bounds directly from the calculated probabilities.

## 3

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

In the [Bühlmann model](../../../actuarial-statistics.md#buhlmann-model), one policy has a random risk parameter $\Theta$. Conditional on $\Theta$, its annual observations $X_i$ are [independent and identically distributed random variables](../../../random-variable.md#independent-and-identically-distributed-random-variables), with mean $m(\Theta)$ and variance $v(\Theta)$. Put $m_0=\mathbb E[m(\Theta)]$, let $v=\mathbb E[v(\Theta)]$ be the [expected process variance](../../../actuarial-statistics.md#expected-process-variance), and let $a=\operatorname{Var}(m(\Theta))$ be the [variance of hypothetical means](../../../actuarial-statistics.md#variance-of-hypothetical-means). Assume the required second moments are finite.

The [Bühlmann credibility premium](../../../actuarial-statistics.md#buhlmann-credibility-premium) is the best affine estimate of $m(\Theta)$ under [mean squared error](../../../statistical-modelling.md#mean-squared-error). After choosing the intercept to make the estimate unbiased, write it as $m_0+\sum_{i=1}^n b_i(X_i-m_0)$. If $B=\sum_i b_i$, the [law of total variance](../../../probability-theory.md#law-of-total-variance) and conditional independence give its error

$$
\mathbb E\left[\left(m(\Theta)-m_0-\sum_i b_i(X_i-m_0)\right)^2\right]
=a(1-B)^2+v\sum_i b_i^2.
$$

For fixed $B$, the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) minimizes the last sum at $b_i=B/n$. Differentiating $a(1-B)^2+vB^2/n$ gives $B=na/(na+v)$. Thus the [credibility factor](../../../actuarial-statistics.md#credibility-factor) and [credibility premium](../../../actuarial-statistics.md#credibility-estimate) are

$$
\boxed{Z=\frac{na}{na+v}=\frac{n}{n+v/a},\qquad \widehat m=Z\overline X+(1-Z)m_0.}
$$

The ratio form assumes $a>0$; when $a=0$ and $v>0$, the conditional mean is constant and $Z=0$. Predicting $X_{n+1}$ rather than its conditional mean adds the constant $v$ to the error and leaves the optimal affine estimate unchanged.

Here the latent intensity has a [Pareto distribution](../../../continuous-probability-distribution.md#pareto-distribution) with shape three and lower bound one. For $r<3$, its moments are $\mathbb E[\Theta^r]=3\int_1^\infty\theta^{r-4}\,d\theta=3/(3-r)$. Consequently

$$
m_0=\mathbb E\Theta=\frac32,\qquad v=\mathbb E\Theta=\frac32,\qquad a=\operatorname{Var}\Theta=3-\frac94=\frac34.
$$

The equality for $v$ uses the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) conditional variance $v(\Theta)=\Theta$. There are two years of experience, so $Z=1/2$ and the observed [sample mean](../../../variance.md#sample-mean) is $k/2$. The [Poisson credibility with a shape-three Pareto intensity](../../../actuarial-statistics.md#poisson-credibility-with-a-shape-three-pareto-intensity) is therefore

$$
\boxed{\widehat m_{\mathrm{cred}}=\frac12\frac{k}{2}+\frac12\frac32=\frac{k+3}{4}.}
$$

In particular it equals $2$ when $k=5$.

For the exact [Bayesian credibility](../../../actuarial-statistics.md#bayesian-credibility) estimate, the total count conditional on $\Theta=\theta$ has [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) of mean $2\theta$. Multiplication of its [likelihood](../../../statistical-modelling.md#likelihood-function) by the [prior distribution](../../../statistical-inference.md#prior-probability) density gives a [Bayesian posterior](../../../statistical-inference.md#bayesian-posterior) density proportional to $\theta^{k-4}e^{-2\theta}$ on $\theta>1$. At $k=5$, its normalizing integral and first-moment integral are

$$
\int_1^\infty\theta e^{-2\theta}\,d\theta=\frac34e^{-2},\qquad
\int_1^\infty\theta^2e^{-2\theta}\,d\theta=\frac54e^{-2}.
$$

Hence the next-year predictive [expected value](../../../probability-theory.md#expected-value) is

$$
\boxed{\mathbb E[N_3\mid N_1+N_2=5]=\mathbb E[\Theta\mid N_1+N_2=5]=\frac53\ne2.}
$$

The [Bühlmann credibility premium](../../../actuarial-statistics.md#buhlmann-credibility-premium) optimizes over affine estimates, whereas the [Bayesian posterior](../../../statistical-inference.md#bayesian-posterior) mean optimizes over all square-integrable estimates. This explains why the two [credibility estimates](../../../actuarial-statistics.md#credibility-estimate) need not agree for this nonconjugate prior.

## 4

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Mix the conditional [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) over the rate-$\nu$ [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) intensity. The [Gamma integral](../../../complex-analysis.md#gamma-integral) gives

$$
\mathbb P(N=j)=\int_0^\infty\frac{e^{-\lambda}\lambda^j}{j!}\nu e^{-\nu\lambda}\,d\lambda
=\frac{\nu}{(1+\nu)^{j+1}}=pq^j,
$$

where $p=\nu/(1+\nu)$ and $q=1/(1+\nu)$. Thus the annual [claim count](../../../actuarial-statistics.md#claim-count) has the zero-based [geometric distribution](../../../discrete-probability-distribution.md#geometric-distribution), with probabilities $\mathbb P(N=0)=p$, $\mathbb P(N=1)=pq$ and $\mathbb P(N\ge2)=q^2$.

For the intended [Markov chain](../../../markov-process.md#markov-chain) calculation, take these annual counts to be independent. Order the states by discounts $0,\alpha,\beta$. From either of the first two states, a positive count returns the policy to zero, while a zero count raises it by one level. From the top, two or more claims send it to zero, exactly one sends it to $\alpha$, and no claim keeps it at $\beta$. Hence the [transition matrix](../../../markov-process.md#stochastic-matrix) is

$$
\boxed{P=\begin{pmatrix}q&p&0\\q&0&p\\q^2&pq&p\end{pmatrix}.}
$$

Write its [stationary distribution](../../../markov-process.md#stationary-distribution) as $(\pi_0,\pi_\alpha,\pi_\beta)$. The final two balance equations give $q\pi_\beta=p\pi_\alpha$ and $\pi_\alpha=p\pi_0+pq\pi_\beta$. It follows that $\pi_\alpha=p\pi_0/[q(1+p)]$ and $\pi_\beta=p^2\pi_0/[q^2(1+p)]$. Normalizing yields the [three-level discount equilibrium with geometric annual counts](../../../actuarial-statistics.md#three-level-discount-equilibrium-with-geometric-annual-counts):

$$
\boxed{(\pi_0,\pi_\alpha,\pi_\beta)=\frac{(q^2(1+p),pq,p^2)}{1-p^2q}.}
$$

The [Markov chain](../../../markov-process.md#markov-chain) is irreducible for $0<p,q<1$ and has a self-loop, so it is aperiodic and this equilibrium is the limiting distribution. Weighting the three premiums $c,c(1-\alpha),c(1-\beta)$ gives

$$
\boxed{\mathbb E[\text{stationary premium}]=c\left[1-\frac{\alpha pq+\beta p^2}{1-p^2q}\right].}
$$

There is a necessary qualification to the temporal model: the one-year mixture alone does not specify independence between years. A [persistent claim intensity can destroy the discount Markov property](../../../actuarial-statistics.md#persistent-claim-intensity-can-destroy-the-discount-markov-property). If one fixed $\Lambda$ is drawn for the policyholder and annual counts are conditionally independent given it, then histories $0,\alpha,\beta,\beta$ and $0,0,\alpha,\beta$ both end at the top after three years but give different next-year no-claim probabilities. The first history is three zero counts, so its posterior intensity has exponential rate $\nu+3$ and next no-claim probability $(\nu+3)/(\nu+4)$. The second is a positive count followed by two zero counts; its posterior density is proportional to $(1-e^{-\lambda})e^{-(\nu+2)\lambda}$, giving next no-claim probability $(\nu+2)/(\nu+4)$. Thus the displayed matrix and premium require independent annual marginal sampling, for example a fresh intensity each year. They are not valid for a persistent unobserved policy intensity without conditioning on that intensity.

Under the persistent-intensity interpretation, one can instead condition on $\lambda$. Put $a_0=e^{-\lambda}$ and $b_1=\lambda e^{-\lambda}$. The conditional [transition matrix](../../../markov-process.md#stochastic-matrix) has rows $(1-a_0,a_0,0)$, $(1-a_0,0,a_0)$ and $(1-a_0-b_1,b_1,a_0)$. Its [stationary distribution](../../../markov-process.md#stationary-distribution) is

$$
\pi(\lambda)=\frac{(1-a_0-a_0b_1,\ a_0(1-a_0),\ a_0^2)}{1-a_0b_1}.
$$

The corresponding population limiting [expected value](../../../probability-theory.md#expected-value) of the premium is $c\int_0^\infty[1-\alpha\pi_\alpha(\lambda)-\beta\pi_\beta(\lambda)]\nu e^{-\nu\lambda}\,d\lambda$. This gives the correct alternative when the intensity persists, and makes the extra assumption behind the requested marginal matrix explicit.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Compare future premium differences, since the current premium is already fixed. From the highest discount, making no claim keeps all future premiums at $c(1-\beta)$. One submitted claim raises next year's premium to $c(1-\alpha)$; if there are no further events, the year after returns to $c(1-\beta)$. The extra premium is therefore $c(\beta-\alpha)$. Claiming saves payment of the loss itself, so the first claim is advantageous precisely when $L_1>c(\beta-\alpha)$. For the unit-rate [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) loss,

$$
\boxed{\mathbb P(\text{claim for }L_1)=e^{-c(\beta-\alpha)}.}
$$

Now condition on the first claim already having been submitted. If the second loss is not claimed, next year's discount is $\alpha$ and the following year's is $\beta$. Claiming the second loss instead makes these two discounts $0$ and $\alpha$, after which both paths are back at $\beta$. Thus the additional premium caused by this second claim is

$$
c\alpha+c(\beta-\alpha)=c\beta.
$$

This is the [incremental second-claim threshold at the highest discount level](../../../actuarial-statistics.md#incremental-second-claim-threshold-at-the-highest-discount-level): compare the second decision to the already-chosen one-claim path, not to a no-claim path. The second claim is advantageous exactly when $L_2>c\beta$. The losses are independent, so conditioning on the first claim does not change the [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) of $L_2$. Hence

$$
\boxed{\mathbb P(\text{claim for }L_2\mid\text{claimed for }L_1)=e^{-c\beta}.}
$$

Equality at a threshold has probability zero. The infinitely many premiums common to both paths cancel; all nonzero differences occur in the next two years, so no divergent sum is used. These thresholds use the undiscounted comparison in the question, with no interest rate or deductible introduced.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
