<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Parameterize the initial product [normal distribution](../../../../../../normal-distribution.md) by $\eta=(m,\rho)$, using

$$
X^{(0)}_\eta=m+\operatorname{diag}(e^{\rho_1},\ldots,e^{\rho_p})\varepsilon,
\qquad \varepsilon\sim N(0,I_p).
$$

Run the given recursion with independent [random variables](../../../../../../random-variable-split.md) with [uniform distributions](../../../../../../continuous-uniform-distribution.md) to obtain $X_\eta=F_t(X^{(0)}_\eta,Z_{1:t})$. Because the noise laws do not depend on $\eta$, the [chain rule](../../../../../../chain-rule.md) and [automatic differentiation](../../../../../../automatic-differentiation.md) give [reparameterization gradients](../../../../../../reparameterization-gradient.md) through the entire simulated trajectory. The variational objective is $J(\eta)=\operatorname{KL}(q_\eta\Vert\pi)$, where $q_\eta=K^t\nu_\eta$ and $\pi=\mu(\cdot\mid y)$.

One must account for the output [differential entropy](../../../../../../differential-entropy.md), not just optimize $\mathbb E[\log\pi(X_\eta)]$. Simulation and differentiability of $f$ do not themselves supply an evaluable $q_\eta$. If $K$ retains the [reversible Markov chain](../../../../../../reversible-markov-chain.md) assumption from part (b), a concrete algorithm avoids a transition-density oracle using [reversible density-ratio propagation](../../../../../../reversible-density-ratio-propagation.md). Write $\pi=h/Z_\pi$, with $h$ an evaluable unnormalized [posterior density](../../../../../../posterior-density.md), and define

$$
A_\eta(x)=\mathbb E_{B\sim K^t(x,\cdot)}\left[\frac{\nu_\eta(B)}{h(B)}\right].
$$

[Detailed balance](../../../../../../detailed-balance.md) implies

$$
q_\eta(x)=h(x)A_\eta(x),\qquad
\boxed{J(\eta)=\log Z_\pi+\mathbb E[\log A_\eta(X_\eta)].}
$$

For example, integrate $\nu_\eta(b)K^t(b,dx)$ and replace $h(b)K^t(b,dx)$ by $h(x)K^t(x,db)$ to obtain the first identity. This also proves [absolute continuity of measures](../../../../../../absolute-continuity-of-measures.md) of $K^t\nu_\eta$ with respect to $\pi$ when $\nu_\eta\ll\pi$. An everywhere finite differentiable [log-posterior](../../../../../../log-posterior.md) has positive density, so an ordinary product [normal distribution](../../../../../../normal-distribution.md) has this domination.

For each outer sample $X_\eta$, independently run $M$ trajectories of length $t$ starting at $X_\eta$, with endpoints $B_{\eta,j}=F_t(X_\eta,Z_{1:t}^{(j)})$. These are reverse trajectories because of [detailed balance](../../../../../../detailed-balance.md); the same recursion simulates them. Estimate $A_\eta(X_\eta)$ by

$$
\widehat A_\eta(X_\eta)=\frac1M\sum_{j=1}^M
\frac{\nu_\eta(B_{\eta,j})}{h(B_{\eta,j})}.
$$

Average $\log\widehat A$ over an outer batch. Compute it stably by a logarithmic sum of exponentials. Differentiate through both outer and reverse trajectories and through the explicit product-normal [probability density function](../../../../../../probability-density-function.md) $\nu_\eta$. Only the given state [gradients](../../../../../../gradient.md) of $f$ and $\log h$, together with elementary normal-density [derivatives](../../../../../../derivative.md), are needed. Apply [stochastic gradient descent](../../../../../../stochastic-gradient-descent.md) to $m$ and $\rho$, refreshing the independent noise batches. The logarithmic scale parameters keep all [variances](../../../../../../variance-split.md) positive.

This is [nested Monte Carlo](../../../../../../nested-monte-carlo.md) optimization of the exact objective in the limit of adequately increasing inner and outer sample sizes. For fixed $M$, $\log\widehat A$ is generally biased, even though $\widehat A$ is an [unbiased estimator](../../../../../../unbiased-estimator.md). Finite logarithmic moments, suitable uniform integrability, and justified [differentiation under the integral sign](../../../../../../differentiation-under-the-integral-sign.md) are needed for consistency and [gradient](../../../../../../gradient.md) interchange. Under those conditions increasing $M$ and controlling the optimization error yields a justified numerical approximation; nonconvexity prevents a generic guarantee of a global optimum.

There is a real assumption issue: part (c) redefines $K$ without explicitly restating reversibility. The algorithm above uses the reversible interpretation inherited from part (b). For an arbitrary differentiable recursion, one additionally needs access to output densities or a simulatable reverse kernel and regularity of the objective. Differentiability alone is insufficient: $f(x,z)=0$ is differentiable and, with a standard-normal target, makes $K^t\nu$ a point mass for $t\geq1$, so every candidate has infinite [Kullback-Leibler divergence](../../../../../../kullback-leibler-divergence.md). Thus a universal finite-objective algorithm cannot be justified solely from the literal differentiability assumptions. An invertible recursion with computable density transformations offers a different sufficient route, but invertibility is not stated here.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
