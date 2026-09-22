<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For minimization of an energy $E(\vartheta)$, [simulated annealing](../../../../../simulated-annealing.md) at temperature $t>0$ targets the [Boltzmann distribution](../../../../../boltzmann-distribution.md) $\pi_t(\vartheta)\propto e^{-E(\vartheta)/t}$ relative to a specified parameter reference measure. With [proposal distribution](../../../../../proposal-distribution.md) $q(\vartheta'\mid\vartheta)$, accept with

$$
a_t(\vartheta,\vartheta')=\min\left\{1,\exp\left[-\frac{E(\vartheta')-E(\vartheta)}t\right]\frac{q(\vartheta\mid\vartheta')}{q(\vartheta'\mid\vartheta)}\right\}.
$$

At each temperature run the chain long enough to explore that law, then cool and retain the best state seen. For symmetric proposals every improvement is accepted, while a worsening move is accepted with probability $e^{-\Delta E/t}$. Equilibrium laws concentrate near global minima when their normalizing integrals are finite and the minima are suitably isolated. A particular rapid cooling schedule does not automatically inherit this guarantee.

**Likelihood maximization uses energy $E=-\ell$, not $E=\ell$.** The source's later wording “$f(p)$ equal to the log-likelihood” conflicts with its preceding minimization convention. The intended maximum-likelihood [Boltzmann distribution](../../../../../boltzmann-distribution.md) is proportional to $e^{\ell/t}=L^{1/t}$. With the opposite sign, likelihood maxima would be disfavored; for binomial data with both successes and failures the density often would not even be integrable near the endpoints as $t$ decreases.

For the [maximum-likelihood estimates](../../../../../maximum-likelihood-estimator.md), write $s=\sum_{j=1}^m x_j$, $\bar x=s/m$ and $S=\sum_j(x_j-\bar x)^2$. In the [binomial distribution](../../../../../binomial-distribution.md) model with known positive integer $n$, the [log-likelihood](../../../../../log-likelihood.md) is

$$
\ell_B(p)=C_B+s\log p+(mn-s)\log(1-p),\qquad C_B=\sum_{j=1}^m\log\binom n{x_j}.
$$

Differentiating gives $s/p-(mn-s)/(1-p)=0$, hence $\widehat p=s/(mn)$. The second derivative is negative in the interior. If $s=0$ or $s=mn$, the maximum is at the corresponding endpoint. This model requires integer observations in $\{0,\ldots,n\}$; otherwise its [likelihood](../../../../../likelihood-function.md) is zero.

For the [normal distribution](../../../../../normal-distribution.md) model write $v=\sigma^2$. Its [log-likelihood](../../../../../log-likelihood.md) is

$$
\ell_N(\mu,v)=-\frac m2\log(2\pi v)-\frac{S+m(\mu-\bar x)^2}{2v}.
$$

For fixed $v$, the unique maximizing mean is $\bar x$. Substituting it and differentiating in $v$ gives $v=S/m$, so, assuming $S>0$,

$$
\boxed{\widehat p=\frac{s}{mn},\qquad\widehat\mu=\bar x,\qquad\widehat{\sigma^2}=\frac Sm.}
$$

If $S=0$, the normal density likelihood grows without bound as $v\downarrow0$ with $\mu=\bar x$; there is no finite interior maximum or ordinary finite AIC for that fit.

For [Gaussian likelihood Gibbs annealing](../../../../../gaussian-likelihood-gibbs-annealing.md), use $L_N^{1/t}$ relative to $d\mu\,dv$. Completing the square and identifying an [inverse-gamma distribution](../../../../../inverse-gamma-distribution.md) gives the [Gibbs sampler](../../../../../gibbs-sampler.md) conditionals

$$
\boxed{\mu\mid v,t\sim N(\bar x,tv/m),\qquad v\mid\mu,t\sim\operatorname{InvGamma}\left(\frac{m}{2t}-1,\frac{S+m(\mu-\bar x)^2}{2t}\right).}
$$

Integrating out $\mu$ contributes a factor proportional to $v^{1/2}$, so the marginal is $v\sim\operatorname{InvGamma}(m/(2t)-3/2,S/(2t))$. The joint target is proper for $0<t<m/3$ when $S>0$; starting the Lebesgue-based annealing above this range would require a proper reference factor or bounded parameter domain. For sufficiently small $t$, its moments satisfy

$$
E_t[v]=\frac S{m-5t},\qquad \operatorname{Var}_t(v)=\frac{2tS^2}{(m-5t)^2(m-7t)},\qquad E_t[(\mu-\bar x)^2]=\frac{tS}{m(m-5t)}.
$$

Thus equilibrium draws concentrate at $(\bar x,S/m)$ as $t\downarrow0$.

There is also a direct convergence proof for the actual successive [Gibbs sampler](../../../../../gibbs-sampler.md) updates here. Choose deterministic $0<t_r\le m/10$ with $t_r\to0$, start at a finite deterministic $v_0>0$, draw $\mu_r$ from the first conditional using $v_{r-1}$, then draw $v_r$ from the second using $\mu_r$. Conditional normal moments give $E[(\mu_r-\bar x)^2\mid v_{r-1}]=t_rv_{r-1}/m$ and $E[(\mu_r-\bar x)^4\mid v_{r-1}]=3t_r^2v_{r-1}^2/m^2$. The permitted inverse-gamma moments therefore yield

$$
E[v_r]=\frac{S+t_rE[v_{r-1}]}{m-4t_r},\qquad
E[v_r^2]=\frac{S^2+2St_rE[v_{r-1}]+3t_r^2E[v_{r-1}^2]}{(m-4t_r)(m-6t_r)}.
$$

The coefficient on the preceding first moment is at most $1/6$, and that on the preceding second moment is at most $1/8$. The remaining coefficients are uniformly bounded, so both moment sequences are bounded by iteration. Since $t_r\to0$, the recursions then give $E[v_r]\to S/m$ and $E[v_r^2]\to(S/m)^2$. Also $E[(\mu_r-\bar x)^2]=t_rE[v_{r-1}]/m\to0$. Hence

$$
\boxed{E[(v_r-S/m)^2]\longrightarrow0,\qquad E[(\mu_r-\bar x)^2]\longrightarrow0.}
$$

This proves convergence in mean square, and thus in probability, to the normal [maximum-likelihood estimates](../../../../../maximum-likelihood-estimator.md) for this explicit cooling/update scheme, rather than merely assuming equilibration.

For [binomial likelihood-power annealing](../../../../../binomial-likelihood-power-annealing.md), normalizing $p^{s/t}(1-p)^{(mn-s)/t}$ on $(0,1)$ gives

$$
\boxed{p\sim\operatorname{Beta}\left(\frac st+1,\frac{mn-s}t+1\right).}
$$

Its mean is $(s+t)/(mn+2t)$, and its [variance](../../../../../variance-split.md) is

$$
\operatorname{Var}_t(p)=\frac{t(s+t)(mn-s+t)}{(mn+2t)^2(mn+3t)}.
$$

The mean tends to $s/(mn)$ and the variance tends to zero, proving concentration at the binomial [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md), including the endpoint cases. Independent exact draws from these beta laws are a simple annealing implementation within this model.

For model selection, the [Akaike information criterion](../../../../../akaike-information-criterion.md) is $2d-2\widehat\ell$ with $d_B=1$ and $d_N=2$. Thus

$$
\boxed{\begin{aligned}
\operatorname{AIC}_B&=2-2\left\{C_B+s\log\widehat p+(mn-s)\log(1-\widehat p)\right\},\\
\operatorname{AIC}_N&=4+m\left\{\log(2\pi S/m)+1\right\}.
\end{aligned}}
$$

Use the endpoint convention $0\log0=0$. For a [trans-dimensional annealing for penalized likelihood](../../../../../trans-dimensional-annealing-for-penalized-likelihood.md) construction, target the disjoint model spaces with unnormalized densities

$$
\Pi_t(B,p)=e^{(\ell_B(p)-1)/t},\qquad \Pi_t(N,\mu,v)=e^{(\ell_N(\mu,v)-2)/t}
$$

relative to $dp$ and $d\mu\,dv$, respectively. The energies are half the unoptimized AIC, $d-\ell$; their joint minimizer is the fitted model with smaller AIC. Keep constants such as $C_B$ and the normal density normalization, which do not cancel across models. The within-model conditional draws are unchanged by these constant penalties.

Here is a complete dimension-changing proposal. Select a binomial-to-normal move with probability $b>0$ and a normal-to-binomial move with probability $d>0$, both fixed; other steps can use the within-model updates. From $B,p$, draw $u\sim N(0,1)$ with density $h(u)=(2\pi)^{-1/2}e^{-u^2/2}$ and set

$$
\mu'=\log\frac p{1-p},\qquad v'=e^u.
$$

This bijection from $(p,u)\in(0,1)\times\mathbb R$ onto $(\mu',v')\in\mathbb R\times(0,\infty)$ has inverse $p=(1+e^{-\mu'})^{-1}$, $u=\log v'$. Its absolute [Jacobian determinant](../../../../../jacobian-determinant.md) is $v'/[p(1-p)]$. The [Binomial-normal reversible-jump annealing](../../../../../binomial-normal-reversible-jump-annealing.md) acceptance ratio is therefore

$$
\boxed{R_{B\to N}=\exp\left[\frac{\ell_N(\mu',v')-2-\ell_B(p)+1}t\right]\frac{d}{b\,h(u)}\frac{v'}{p(1-p)},\qquad a_{B\to N}=\min(1,R_{B\to N}).}
$$

For a reverse proposal from $N,\mu,v$, compute $p'=(1+e^{-\mu})^{-1}$ and $u'=\log v$ deterministically and accept with

$$
\boxed{R_{N\to B}=\exp\left[\frac{\ell_B(p')-1-\ell_N(\mu,v)+2}t\right]\frac{b\,h(u')}{d}\frac{p'(1-p')}{v},\qquad a_{N\to B}=\min(1,R_{N\to B}).}
$$

These ratios are reciprocal at inverse states and enforce [detailed balance](../../../../../detailed-balance.md) on the dimension-matched augmented spaces. They specify the proposal density, model-selection probabilities and Jacobian explicitly. The map is a valid example, not a claim of optimal mixing. Positive-temperature beta draws stay in the open interval even when the limiting estimate is an endpoint. At each temperature ensure adequate model switching; retain the best fitted penalized likelihood encountered. If minima tie, limiting concentration need not choose a unique model.

There is a material measurement qualification. A binomial probability mass and an unrounded normal density use different observation reference measures. **Their raw AIC values are not an invariant, scientifically calibrated comparison of the same recorded data.** The expressions and jump algorithm above implement the formal density comparison suggested by the question, with its units fixed. For integer-recorded measurements, a compatible normal model instead assigns probabilities $P_{\mu,v}(x-1/2<Z\le x+1/2)$, suitably adjusting boundaries or truncation if required. Then both models describe the same recorded outcomes relative to counting measure. Use those masses in the normal likelihood and the same reversible-jump formula; its simple normal MLE and conjugate Gibbs updates will generally no longer apply. This observation-model correction cannot be silently combined with the continuous-normal formulas.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
