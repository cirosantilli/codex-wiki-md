<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [Metropolis–Hastings algorithm](../../../../../metropolis-hastings-algorithm.md) proposes $y\sim q(\cdot\mid x)$ and moves from the current state $x$ with acceptance [probability](../../../../../probability.md)

$$
\alpha(x,y)=\min\left\{1,\frac{\pi(y)q(x\mid y)}{\pi(x)q(y\mid x)}\right\}.
$$

On rejection it retains $x$. The target need only be known up to its normalizing constant, but it must define a proper [probability](../../../../../probability.md) distribution. The accepted off-diagonal [probability](../../../../../probability.md) flow is

$$
\pi(x)q(y\mid x)\alpha(x,y)
=\min\{\pi(x)q(y\mid x),\pi(y)q(x\mid y)\},
$$

which is symmetric in $x,y$ and proves [detailed balance](../../../../../detailed-balance.md). This permits considerable flexibility in proposals, including joint moves when a [posterior distribution](../../../../../bayesian-posterior.md) has strongly correlated parameters, but requires proposal tuning and can waste computation on rejections.

A [Gibbs sampler](../../../../../gibbs-sampler.md) instead updates a coordinate or block from its exact [full conditional distribution](../../../../../full-conditional-distribution.md), holding the other coordinates fixed. This is a special [Metropolis–Hastings algorithm](../../../../../metropolis-hastings-algorithm.md) update with acceptance [probability](../../../../../probability.md) one: the joint density factors into the unchanged marginal density and the proposed conditional density, which cancel in the acceptance ratio. The coordinate update preserves the target; composing such updates therefore preserves it too, although an entire deterministic sweep need not itself be reversible.

Use [Gibbs sampling](../../../../../gibbs-sampler.md) when the conditional laws are easy to simulate and suitably chosen blocks mix well. Scalar updates can mix poorly under strong [posterior distribution](../../../../../bayesian-posterior.md) correlation, whereas a [blocked Gibbs sampler](../../../../../blocked-gibbs-sampler.md) can alleviate that dependence. Prefer a flexible Metropolis proposal when conditional draws are difficult or a well-tuned joint proposal is more effective. Variations include random or systematic coordinate scans, [Random-walk Metropolis algorithms](../../../../../random-walk-metropolis-algorithm.md), [independence](../../../../../independent-random-variables.md) proposals, and using Metropolis updates for difficult blocks inside a Gibbs scheme. Both methods generate dependent draws; usable long-run estimates require an appropriate irreducible, aperiodic chain and assessment of mixing, not merely a formal update rule.

For the change-point calculation, put $v=\sigma^2$ and

$$
S_m(\theta,\phi)=\sum_{i=1}^m(x_i-\theta)^2+
\sum_{i=m+1}^n(x_i-\phi)^2.
$$

Multiplication of the [Gaussian](../../../../../normal-distribution.md) [likelihood function](../../../../../likelihood-function.md) by the specified [prior distribution](../../../../../prior-probability.md) gives the formal [posterior distribution](../../../../../bayesian-posterior.md) kernel, with respect to $d\theta\,d\phi\,dv$ and counting measure on $m$,

$$
\boxed{\widetilde\pi(\theta,\phi,v,m\mid x)
\propto\frac1n\,v^{-n/2-1}
\exp\left[-\frac{S_m(\theta,\phi)}{2v}\right],\qquad v>0,\ 1\le m\le n.}
$$

There is an [empty component under an improper prior](../../../../../empty-component-under-an-improper-prior.md) at $m=n$. The sum $S_n$ is independent of $\phi$, whose [prior distribution](../../../../../prior-probability.md) is flat on all of $\mathbb R$. For every fixed finite $\theta$ and $v>0$, the kernel is a strictly positive constant in $\phi$, hence

$$
\int_{\mathbb R}\widetilde\pi(\theta,\phi,v,n\mid x)\,d\phi=\infty.
$$

The configuration has positive [prior probability](../../../../../prior-probability.md) $1/n$. Integrating over, for example, a bounded interval of $\theta$ and $1\le v\le2$ already makes the joint normalization infinite. Thus **the printed [prior distribution](../../../../../prior-probability.md) does not produce a [posterior probability](../../../../../posterior-probability.md) distribution**. This failure is present for every data set, not just for a special arrangement of observations.

The formal full conditionals expose exactly where the requested sampler breaks. For $m<n$, completing the two mean squares gives

$$
\theta\mid\phi,v,m,x\sim N\left(\overline x_{1:m},\frac vm\right),\qquad
\phi\mid\theta,v,m,x\sim N\left(\overline x_{m+1:n},\frac v{n-m}\right).
$$

The [variance](../../../../../variance-split.md) kernel is that of $\operatorname{IG}(n/2,S_m/2)$ when $S_m>0$, and the discrete conditional probabilities are proportional to $e^{-S_m/(2v)}$. At $m=n$ the conditional kernel for $\phi$ is constant and cannot be normalized; it is not a [normal distribution](../../../../../normal-distribution.md) with an infinite [variance](../../../../../variance-split.md). Therefore **no valid [Gibbs sampler](../../../../../gibbs-sampler.md), and no value of $P(m=n\mid x)$, exists for the model as printed**. A chain that simply substitutes an arbitrary distribution for this missing conditional would be sampling a different model.

Here is a fully specified proper-prior repair retaining the no-change configuration. Choose fixed hyperparameters

$$
\theta\sim N(\mu_\theta,t_\theta),\quad
\phi\sim N(\mu_\phi,t_\phi),\quad
v\sim\operatorname{IG}(a_0,b_0),\quad m\sim\operatorname{Uniform}\{1,\ldots,n\},
$$

independently, with $t_\theta,t_\phi,a_0,b_0>0$. Its [Gaussian change-point posterior with proper priors](../../../../../gaussian-change-point-posterior-with-proper-priors.md) is

$$
\pi_{\mathrm{proper}}\propto\frac1n
v^{-(a_0+n/2+1)}\exp\left[-\frac{b_0+S_m/2}{v}
-\frac{(\theta-\mu_\theta)^2}{2t_\theta}
-\frac{(\phi-\mu_\phi)^2}{2t_\phi}\right].
$$

It is normalizable even for degenerate data: the [likelihood function](../../../../../likelihood-function.md) is at most $(2\pi)^{-n/2}v^{-n/2}$, and its integral against the [variance](../../../../../variance-split.md) [prior distribution](../../../../../prior-probability.md) is bounded by

$$
(2\pi)^{-n/2}b_0^{-n/2}
\frac{\Gamma(a_0+n/2)}{\Gamma(a_0)}<\infty.
$$

The normal mean priors integrate to one, and the normalizing constant is positive. This proves [posterior propriety](../../../../../posterior-propriety.md) for the repaired model.

Completing the conditional squares gives the [Gaussian change-point Gibbs updates](../../../../../gaussian-change-point-gibbs-updates.md). Define

$$
V_\theta=\left(\frac mv+\frac1{t_\theta}\right)^{-1},\qquad
M_\theta=V_\theta\left(\frac{\sum_{i\le m}x_i}{v}+\frac{\mu_\theta}{t_\theta}\right),
$$



$$
V_\phi=\left(\frac{n-m}{v}+\frac1{t_\phi}\right)^{-1},\qquad
M_\phi=V_\phi\left(\frac{\sum_{i>m}x_i}{v}+\frac{\mu_\phi}{t_\phi}\right).
$$

The four updates are

$$
\boxed{\begin{aligned}
\theta\mid\cdots&\sim N(M_\theta,V_\theta),\\
\phi\mid\cdots&\sim N(M_\phi,V_\phi),\\
v\mid\cdots&\sim\operatorname{IG}(a_0+n/2,b_0+S_m(\theta,\phi)/2),\\
\mathbb P(m=k\mid\theta,\phi,v,x)&=
\frac{e^{-S_k(\theta,\phi)/(2v)}}{\sum_{j=1}^ne^{-S_j(\theta,\phi)/(2v)}}.
\end{aligned}}
$$

At $m=n$, $M_\phi=\mu_\phi,V_\phi=t_\phi$, giving its proper [prior distribution](../../../../../prior-probability.md) unchanged. Starting from any finite means, positive [variance](../../../../../variance-split.md) and allowed $m$, cycle through these four updates using the latest values. The sum-of-squares terms can be evaluated from cumulative data sums; normalize the discrete log weights after subtracting their maximum to avoid numerical underflow. The proper positive conditionals allow movement among all split values and throughout the continuous parameter support.

Under this specified repair, $P(m=n\mid x)$ is the [posterior probability](../../../../../posterior-probability.md) of no change within the observed sequence: all $n$ data points belong to the first mean regime. For $N$ retained draws after initialization has ceased to affect the estimates, its [Markov chain Monte Carlo](../../../../../markov-chain-monte-carlo.md) [estimator](../../../../../estimator.md) is

$$
\boxed{\widehat P(m=n\mid x)=\frac1N\sum_{r=1}^N\mathbf1_{\{m^{(r)}=n\}}.}
$$

Alternatively average the displayed conditional [probability](../../../../../probability.md) of $m=n$ at the sampled continuous parameters, giving an estimate by [Rao-Blackwellization](../../../../../rao-blackwellization.md). Autocorrelation must be accounted for in its Monte Carlo uncertainty. These are probabilities and [estimators](../../../../../estimator.md) for the explicitly repaired model; the original unnormalizable kernel supplies neither.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
