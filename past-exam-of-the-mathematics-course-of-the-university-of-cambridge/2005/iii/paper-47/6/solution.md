<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For minimizing an energy $F(\theta)$, [simulated annealing](../../../../../simulated-annealing.md) at temperature $T>0$ uses the [Boltzmann distribution](../../../../../boltzmann-distribution.md) $\pi_T(\theta)\propto e^{-F(\theta)/T}$. At each temperature run a [Metropolis–Hastings algorithm](../../../../../metropolis-hastings-algorithm.md) or Gibbs transition preserving that law, then reduce $T$. With a symmetric proposal, accept $\theta'$ with [probability](../../../../../probability.md) $\min\{1,e^{-[F(\theta')-F(\theta)]/T}\}$: downhill moves are accepted and uphill moves remain possible. Keep the best state encountered. As temperature decreases, equilibrium mass favors global minima, provided the target is proper and the relevant concentration hypotheses hold. An arbitrary finite cooling run does not by itself prove global convergence.

Let $s=\sum_{i=1}^m x_i$, $\bar x=s/m$ and $S=\sum_i(x_i-\bar x)^2$. For the [Poisson distribution](../../../../../poisson-distribution.md) model the observations must be nonnegative integers. Its [log-likelihood](../../../../../log-likelihood.md) is

$$
\ell_P(\lambda)=-m\lambda+s\log\lambda-\sum_i\log(x_i!).
$$

For $s>0$, differentiation gives $\ell_P'=-m+s/\lambda$ and $\ell_P''=-s/\lambda^2<0$. If $s=0$, the [likelihood](../../../../../likelihood-function.md) is decreasing and the maximizer is the boundary value zero. For the [normal distribution](../../../../../normal-distribution.md) model write $v=\sigma^2>0$, giving

$$
\ell_N(\mu,v)=-\frac m2\log(2\pi v)
-\frac{S+m(\mu-\bar x)^2}{2v}.
$$

For each $v$, this is maximized at $\mu=\bar x$, and differentiating there gives $v=S/m$. Hence

$$
\boxed{\widehat\lambda=\bar x,\qquad
\widehat\mu=\bar x,\qquad
\widehat{\sigma^2}=S/m.}
$$

The normal [variance](../../../../../variance-split.md) estimate has denominator $m$, not $m-1$. A finite positive normal maximum requires $S>0$; if all observations coincide, the [likelihood](../../../../../likelihood-function.md) is unbounded as $\mu=\bar x,v\downarrow0$. The normal annealing calculation below assumes $S>0$.

To maximize [likelihood](../../../../../likelihood-function.md), choose the energy $-\ell$, so the annealing law is $L^{1/T}$, not $L^{-1/T}$. This sign is important in the Poisson request: literally inserting a positive [log-likelihood](../../../../../log-likelihood.md) into a minimizing Boltzmann law would give a nonnormalizable [probability density function](../../../../../probability-density-function.md) growing like $e^{m\lambda/T}$ at infinity. We use [likelihood-power annealing](../../../../../likelihood-power-annealing.md) with the maximizing sign.

For the [normal distribution](../../../../../normal-distribution.md) model, take base measure $d\mu\,dv$. The joint annealing [probability density function](../../../../../probability-density-function.md) is

$$
\pi_T(\mu,v)\propto
v^{-m/(2T)}\exp\!\left[-\frac{S+m(\mu-\bar x)^2}{2Tv}\right].
$$

Completing the square gives the [Gibbs sampling](../../../../../gibbs-sampler.md) conditional for $\mu$. Matching the conditional $v$ [probability density function](../../../../../probability-density-function.md) to the supplied [inverse-gamma distribution](../../../../../inverse-gamma-distribution.md) convention gives

$$
\boxed{\begin{aligned}
\mu\mid v&\sim N(\bar x,Tv/m),\\
v\mid\mu&\sim\operatorname{InvGamma}\left(\frac m{2T}-1,\,
\frac{S+m(\mu-\bar x)^2}{2T}\right).
\end{aligned}}
$$

Integrating out $\mu$ contributes a factor $\sqrt v$, so the marginal law is

$$
v\sim\operatorname{InvGamma}\left(\frac m{2T}-\frac32,\frac S{2T}\right).
$$

Thus this joint Boltzmann law is proper for $T<m/3$. Its [variance](../../../../../variance-split.md) marginal and the normal conditional both concentrate at the stated estimates as $T\downarrow0$. For example, for $T<m/7$ its marginal [mean](../../../../../expected-value.md) and [variance](../../../../../variance-split.md) are

$$
\mathbb E_Tv=\frac S{m-5T},\qquad
\operatorname{Var}_T(v)=\frac{2TS^2}{(m-5T)^2(m-7T)}.
$$

Also $\mathbb E_T(\mu-\bar x)^2=(T/m)\mathbb E_Tv\to0$.

There is a direct convergence proof for the actual changing-temperature Gibbs algorithm, beyond convergence of its equilibrium [probability densities](../../../../../probability-density.md). Start at a finite deterministic $v_0>0$, choose deterministic $0<T_n\leq m/10$ with $T_n\to0$, draw $\mu_n$ conditional on $v_{n-1}$, then draw $v_n$ conditional on $\mu_n$ using the two boxed distributions. Conditional normal moments give

$$
\mathbb E[(\mu_n-\bar x)^2\mid v_{n-1}]=T_nv_{n-1}/m,\qquad
\mathbb E[(\mu_n-\bar x)^4\mid v_{n-1}]=3(T_nv_{n-1}/m)^2.
$$

The [inverse-gamma distribution](../../../../../inverse-gamma-distribution.md) first and [second moments](../../../../../second-moment.md) consequently yield

$$
\mathbb E v_n=\frac{S+T_n\mathbb E v_{n-1}}{m-4T_n},
$$

and

$$
\mathbb E v_n^2=
\frac{S^2+2ST_n\mathbb E v_{n-1}
+3T_n^2\mathbb E v_{n-1}^2}
{(m-4T_n)(m-6T_n)}.
$$

In the first recursion the coefficient of the preceding [mean](../../../../../expected-value.md) is at most $1/6$; in the second the coefficient of the preceding [second moment](../../../../../second-moment.md) is at most $1/8$. The means therefore stay bounded, and then so do the [second moments](../../../../../second-moment.md). Letting $T_n\to0$ in these formulas gives $\mathbb E v_n\to S/m$ and $\mathbb E v_n^2\to(S/m)^2$. Together with $\mathbb E(\mu_n-\bar x)^2=T_n\mathbb E v_{n-1}/m\to0$, this proves

$$
\boxed{(\mu_n,v_n)\longrightarrow(\bar x,S/m)\quad\text{in mean square and hence in probability}.}
$$

This [Gaussian likelihood Gibbs annealing](../../../../../gaussian-likelihood-gibbs-annealing.md) convergence uses the explicit conditional structure and does not assume that one [Gibbs sampling](../../../../../gibbs-sampler.md) sweep is an exact equilibrium draw.

For the [Poisson distribution](../../../../../poisson-distribution.md) model, the likelihood-power law with respect to $d\lambda$ has the normalized [probability density function](../../../../../probability-density-function.md)

$$
\pi_T(\lambda)=\frac{(m/T)^{s/T+1}}{\Gamma(s/T+1)}
\lambda^{s/T}e^{-m\lambda/T}\quad(\lambda>0),
$$

so

$$
\boxed{\lambda_T\sim\operatorname{Gamma}(s/T+1,m/T),\qquad
\mathbb E\lambda_T=\frac{s+T}{m},\quad
\operatorname{Var}(\lambda_T)=\frac{sT+T^2}{m^2}.}
$$

The [mean](../../../../../expected-value.md) tends to $\bar x$ and the [variance](../../../../../variance-split.md) to zero, proving convergence to a point mass at the Poisson [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md), including the zero-boundary case.

The [Akaike information criterion](../../../../../akaike-information-criterion.md) is $2k-2\ell(\widehat\theta)$, counting one parameter for Poisson and two for normal. With $0\log0=0$ and $S>0$, the two forms are

$$
\boxed{\mathrm{AIC}_P=2+2s-2s\log(s/m)+2\sum_i\log(x_i!),}
$$

and

$$
\boxed{\mathrm{AIC}_N=4+m\left[\log(2\pi S/m)+1\right].}
$$

Choose the smaller criterion. [Likelihood](../../../../../likelihood-function.md) constants that differ between models, including the factorial and $2\pi$ terms, cannot be discarded.

For a fully specified [trans-dimensional annealing for penalized likelihood](../../../../../trans-dimensional-annealing-for-penalized-likelihood.md), let $M=P$ or $N$ and define

$$
E_P(\lambda)=2-2\ell_P(\lambda),\qquad
E_N(\mu,v)=4-2\ell_N(\mu,v).
$$

Use the combined target, relative to counting measure on models and Lebesgue measure on their parameters,

$$
\Pi_T(M,\vartheta)\propto w_Me^{-E_M(\vartheta)/(2T)}
=w_Me^{-k_M/T}L_M(\vartheta)^{1/T},
$$

where $w_P,w_N>0$ are fixed reference weights. For $S>0$ and $0<T<m/3$ both model components are integrable. The factor $2T$ is a convenient temperature convention keeping the within-model laws exactly those already derived. The extra factor $e^{-k_M/T}$ makes the zero-temperature objective [AIC](../../../../../akaike-information-criterion.md) rather than unpenalized [likelihood](../../../../../likelihood-function.md).

Use, for example, [probability](../../../../../probability.md) $1/2$ for a model-change attempt in either model and [probability](../../../../../probability.md) $1/2$ for a within-model update. Within the [Poisson distribution](../../../../../poisson-distribution.md) model draw a fresh gamma value from its boxed law; within the [normal distribution](../../../../../normal-distribution.md) model perform the boxed [Gibbs sampling](../../../../../gibbs-sampler.md) sweep. For a Poisson-to-normal proposal, draw $u\sim q(u)=N(0,\tau^2)$ with a fixed $\tau^2>0$, and set

$$
(\mu,v)=(\lambda+u,\lambda).
$$

The inverse normal-to-Poisson proposal is $\lambda=v$ with reverse auxiliary $u=\mu-v$. This dimension matching uses one auxiliary variable to augment the one-dimensional Poisson parameter space. The absolute [Jacobian determinant](../../../../../jacobian-determinant.md) is

$$
J=\left|\det\begin{pmatrix}1&1\\1&0\end{pmatrix}\right|=1.
$$

If the forward model-jump selection [probability](../../../../../probability.md) is $b$ and the reverse [probability](../../../../../probability.md) is $d$, the [reversible-jump Markov chain Monte Carlo](../../../../../reversible-jump-markov-chain-monte-carlo.md) acceptance ratio is

$$
\boxed{R_{P\to N}=
\frac{w_Nd}{w_Pb\,q(u)}
\exp\!\left[-\frac{E_N(\lambda+u,\lambda)-E_P(\lambda)}{2T}\right]J.}
$$

Accept with [probability](../../../../../probability.md) $\min(1,R_{P\to N})$. For the reverse move compute $\lambda=v,u=\mu-v$ and use

$$
\boxed{R_{N\to P}=
\frac{w_Pb\,q(\mu-v)}{w_Nd}
\exp\!\left[-\frac{E_P(v)-E_N(\mu,v)}{2T}\right]J^{-1}.}
$$

For the suggested equal selection [probabilities](../../../../../probability.md), $b=d=1/2$ and those factors cancel. The [probability density function](../../../../../probability-density-function.md) $q$ must still be included, despite symmetry of its [normal distribution](../../../../../normal-distribution.md): it is an auxiliary draw in only the forward dimension-increasing proposal. Pairing a move with its inverse makes the accepted forward and reverse [probability](../../../../../probability.md) flows equal after the change of variables, proving [detailed balance](../../../../../detailed-balance.md) for each fixed-temperature model-switch kernel.

Cool through proper temperatures, allow enough model and parameter exploration at each stage, and retain the smallest observed $E_M$. The minima of the two energies are exactly the two [AIC](../../../../../akaike-information-criterion.md) values above. Low-temperature equilibrium mass concentrates on the better criterion and its fitted parameters; if they tie, the minimizing set contains both models. Unlike the direct normal Gibbs argument, this multimodel exploration claim needs an appropriate cooling/mixing justification and is not guaranteed by an arbitrary short run.

Finally, an exact statistical comparison must put both [likelihoods](../../../../../likelihood-function.md) on the same observable and reference-measure convention. A [Poisson distribution](../../../../../poisson-distribution.md) model is a [probability mass function](../../../../../probability-mass-function.md) on counts, whereas the displayed [normal distribution](../../../../../normal-distribution.md) model is a continuous [probability density function](../../../../../probability-density-function.md). The formulas above are the question's formal [Gaussian](../../../../../normal-distribution.md) working-likelihood comparison. A coherent exact normal approximation for count observations can instead use [probabilities](../../../../../probability.md) of rounding intervals; that changes its [likelihood](../../../../../likelihood-function.md) and generally loses the simple analytic normal estimates. This distinction matters when interpreting the numerical [AIC](../../../../../akaike-information-criterion.md) difference, while leaving the dimension-matching and annealing construction applicable to properly specified [likelihoods](../../../../../likelihood-function.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
