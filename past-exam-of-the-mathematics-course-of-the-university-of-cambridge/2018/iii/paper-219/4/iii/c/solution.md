<h1 id="4/iii/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Keeping the powers and exponentials of $v$ and $\tau$ in the joint kernel gives the two [inverse-gamma distributions](../../../../../../../inverse-gamma-distribution.md), using the printed shape–scale convention:

$$
\boxed{v\mid\text{rest}\sim\operatorname{IG}\left(\frac N2,\frac12\sum_s(C_s-\mu_C)^2\right),\qquad\tau\mid\text{rest}\sim\operatorname{IG}\left(N,\sum_sE_s\right)}.
$$

Indeed their kernels are $v^{-(N/2+1)}\exp[-\sum_s(C_s-\mu_C)^2/(2v)]$ and $\tau^{-(N+1)}\exp[-\sum_sE_s/\tau]$. With positive measurement [variances](../../../../../../../variance-split.md) and generic continuously drawn latent values, the two scale parameters are positive almost surely. Together with (a),(b), these are all $2N+3$ formal full conditional updates.

There is, however, no joint posterior probability distribution to sample under the stated priors. Integrate out the intrinsic $C_s$ first. For fixed $\mu_C,v>0$, the observational marginal density is

$$
L(\mu_C,v,\tau)=\prod_s\int_0^\infty\tau^{-1}e^{-E/\tau}\,\phi_{v+r_s}(o_s-\mu_C-E)\,dE,
$$

where $\phi_V$ is the centred normal density of [variance](../../../../../../../variance-split.md) $V$. Substitute $E=\tau u$. Dominated convergence gives

$$
\lim_{\tau\downarrow0}L(\mu_C,v,\tau)=\prod_s\phi_{v+r_s}(o_s-\mu_C)>0.
$$

The convergence is uniform on any compact $\mu_C$ interval and any compact positive $v$ interval, since the normal densities are uniformly bounded and continuous there. Hence some such region has $L\ge c>0$ for all sufficiently small $\tau$, and

$$
\int_0^\varepsilon L(\mu_C,v,\tau)\frac{d\tau}{\tau}=\infty.
$$

Integrating over those positive-measure intervals proves that the full normalizing constant is infinite. If all $r_s>0$, the $v\downarrow0$ boundary also gives a positive marginal likelihood and a divergent $dv/v$ integral at fixed $\tau>0$. Thus $\boxed{\text{the stated joint posterior is improper}}$, even though its generic full conditionals are proper. Apparent stability of a simulated chain cannot establish a nonexistent stationary probability law.

A valid repair that preserves direct sampling is to replace the two log-flat priors by independent proper $v\sim\operatorname{IG}(a_v,b_v)$ and $\tau\sim\operatorname{IG}(a_\tau,b_\tau)$, with all four constants positive. The normal and truncated-normal updates remain as above, while

$$
v\mid\text{rest}\sim\operatorname{IG}\left(a_v+\frac N2,b_v+\frac12\sum_s(C_s-\mu_C)^2\right),\quad\tau\mid\text{rest}\sim\operatorname{IG}\left(a_\tau+N,b_\tau+\sum_sE_s\right).
$$

With positive $r_s$, the flat $\mu_C$ prior is then harmless: after integrating it out, the Gaussian measurement likelihood is bounded uniformly over the latent shifts and the scales, and the remaining proper priors integrate to one. A proper prior on $\mu_C$ is also possible.

For this repaired model, initialize $v,\tau>0$, $E_s\ge0$ and finite $C_s,\mu_C$. Repeatedly choose one of the $2N+3$ coordinates with fixed positive probabilities and redraw from its full conditional using the latest values. This [Random-scan Gibbs sampler](../../../../../../../random-scan-gibbs-sampler.md) preserves the proper target and satisfies [detailed balance](../../../../../../../detailed-balance.md): for each coordinate, both forward and reverse flows equal the marginal density of the remaining coordinates times the product of the two conditional densities. A systematic full sweep is another invariant scheme, though it need not itself be reversible.

Run several dispersed chains; inspect traces of both scales, $\mu_C$, representative latent values and the log posterior. Assess rank-normalized split $\widehat R$, [autocorrelation](../../../../../../../autocorrelation.md), and the [effective sample size of a Markov chain](../../../../../../../effective-sample-size-of-a-markov-chain.md), and extend runs until relevant Monte Carlo errors are sufficiently small. Scale–latent dependence can cause slow mixing, so diagnostics must include boundary exploration and alternative initializations. Keep post-warmup draws without automatic thinning. These are convergence checks for the repaired posterior; the printed model admits only the formal update algorithm, not a valid posterior-sampling interpretation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [Iii](../../iii.md)
3. [4](../../../4.md)
4. [Paper 219](../../../../paper-219-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
