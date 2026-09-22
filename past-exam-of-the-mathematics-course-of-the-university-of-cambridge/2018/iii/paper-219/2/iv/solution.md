<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

A log-flat [improper prior](../../../../../../improper-prior.md) $p(v)\propto1/v$ is not appropriate when all known $r_s=\sigma_{m,s}^2$ are positive: the integrated likelihood in (iii) has a positive finite limit as $v\downarrow0$, so its integral against $dv/v$ diverges. One defensible noninformative choice is the scalar [Jeffreys prior for an additive variance component](../../../../../../jeffreys-prior-for-an-additive-variance-component.md), calculated holding the mean parameters fixed:

$$
\boxed{p(v)\propto\left[\frac12\sum_s(v+r_s)^{-2}\right]^{1/2},\qquad v\ge0}.
$$

Indeed the normal [variance](../../../../../../variance-split.md) score has information $I_{vv}=\frac12\sum_s(v+r_s)^{-2}$. This is a scalar conditional-information prior, not a claim that its product with the flat mean prior is the joint Jeffreys prior. It is bounded near zero and is $O(v^{-1})$ at infinity. The integrated likelihood is uniformly bounded near zero and is bounded by a constant times $v^{-(N-1)/2}$ at infinity, independently of the mean-shape parameters, since $e^{-Q/2}\le1$. Thus $N>1$ and a proper external prior on the physically admissible $(w,\Omega_M)$ ensure [posterior propriety](../../../../../../posterior-propriety.md). Proper weak scale priors are another option. If known errors vanish, the boundary argument and appropriate prior need separate reconsideration.

For an efficient parameterization, use $\theta=(\beta,u,w,\Omega_M)$ with $u=\log v$ and $\beta=M_0+h(H_0)$. A chain on this joint reduced parameter space targets

$$
\widetilde\pi(\theta)\propto L(\beta,e^u,H_{\rm ref},w,\Omega_M)\,p(e^u)e^u\,p(w,\Omega_M).
$$

The factor $e^u$ is the [Jacobian determinant](../../../../../../jacobian-determinant.md). At each iteration propose $\theta'=\theta+\varepsilon$, with $\varepsilon\sim N(0,\Sigma_q)$ for a fixed nonsingular proposal [covariance](../../../../../../covariance.md), and accept with probability $\min\{1,\widetilde\pi(\theta')/\widetilde\pi(\theta)\}$. Proposals outside the physical prior domain have target zero. Tune $\Sigma_q$ during warmup and freeze it for the retained [Random-walk Metropolis algorithm](../../../../../../random-walk-metropolis-algorithm.md). To obtain samples of the full original parameter vector, independently draw $H_0$ from its retained positive prior and reconstruct $M_0=\beta-h(H_0)$; the resulting vector is $(M_0,v,H_0,w,\Omega_M)$. Analytically marginalizing $\beta$ using (iii) would also be valid.

Use several dispersed chains, trace plots, rank-normalized split $\widehat R$, and the [effective sample size of a Markov chain](../../../../../../effective-sample-size-of-a-markov-chain.md) for each parameter and for $w,w^2$. These [Markov chain Monte Carlo convergence diagnostics](../../../../../../markov-chain-monte-carlo-convergence-diagnostics.md) reveal poor mixing and disagreement but do not prove convergence. Estimate the [integrated autocorrelation time](../../../../../../integrated-autocorrelation-time.md) $\tau_{\rm int}$; with $B$ retained draws, $B_{\rm eff}\approx B/\tau_{\rm int}$. Default to no [thinning of a Markov chain](../../../../../../thinning-of-a-markov-chain.md), so the thinning factor is $1$. If storage requires thinning, choose a spacing after inspecting the autocorrelation and verify the retained-chain effective sample size; no finite spacing guarantees independent draws.

Using the retained $w_b$ samples, compute

$$
\boxed{\widehat{\mathbb E}[w]=\frac1B\sum_bw_b,\qquad\widehat{\operatorname{SD}}(w)=\left[\frac1{B-1}\sum_b(w_b-\bar w)^2\right]^{1/2}}.
$$

These are posterior summaries, provided the corresponding moments exist, not uncertainties of the numerical estimates. A proper prior alone does not ensure finite second moments; choose or check the external prior accordingly. The Monte Carlo standard error of the posterior mean is approximately $\widehat{\operatorname{SD}}(w)/\sqrt{B_{\rm eff}}$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
