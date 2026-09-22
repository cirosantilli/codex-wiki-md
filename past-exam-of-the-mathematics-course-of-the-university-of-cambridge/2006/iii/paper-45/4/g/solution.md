<h1 id="4/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The accepted mutation parameters have marginal [probability density function](../../../../../../probability-density-function.md)

$$
f_\Theta(\theta\mid S=k)=\frac{\pi(\theta)p_k(\theta)}{Z_k}.
$$

Estimate this [probability density function](../../../../../../probability-density-function.md) with a suitably smoothed histogram or a boundary-aware [kernel density estimator](../../../../../../kernel-density-estimation.md) from the accepted draws. On a parameter region where $\pi(\theta)>0$, divide the estimate by the known [prior density](../../../../../../prior-density.md) and maximize:

$$
\boxed{\widehat\theta_{\rm MC}\in\arg\max_{\theta}\frac{\widehat f_\Theta(\theta\mid S=k)}{\pi(\theta)}.}
$$

The unknown $Z_k$ is constant in $\theta$ and cancels. Maximizing the [posterior density](../../../../../../posterior-density.md) itself gives a posterior mode, not generally a [maximum-likelihood estimate](../../../../../../maximum-likelihood-estimator.md); the two coincide for a flat prior on a region containing the maximum. A prior excluding candidate maximizers cannot recover them through its posterior output. Boundary behavior also matters: for $k=0$, the [likelihood](../../../../../../likelihood-function.md) is decreasing in $\theta$, so the unrestricted maximum is at $\theta=0$.

The exact [likelihood](../../../../../../likelihood-function.md) provides a useful independent check. Put $W=L/2$. Its [Laplace transform](../../../../../../laplace-transform.md) is $\prod_{i=1}^{n-1}i/(i+s)$, since $jT_j/2$ is exponential of rate $j-1$. The [probability density function](../../../../../../probability-density-function.md)

$$
g_W(w)=(n-1)e^{-w}(1-e^{-w})^{n-2},\qquad w>0,
$$

has that same transform: substitute $u=e^{-w}$ to obtain $(n-1)\int_0^1u^s(1-u)^{n-2}du=\prod_{i=1}^{n-1}i/(i+s)$. Thus, expanding its binomial factor and integrating each term,

$$
p_k(\theta)=\frac{\theta^k}{k!}\int_0^\infty w^ke^{-\theta w}g_W(w)dw
=(n-1)\theta^k\sum_{r=0}^{n-2}\frac{(-1)^r\binom{n-2}{r}}{(\theta+r+1)^{k+1}}.
$$

This is the [segregating-site likelihood under the neutral coalescent](../../../../../../segregating-site-likelihood-under-the-neutral-coalescent.md). It can be maximized numerically to check the posterior-density estimate; the generating-function representation avoids cancellation in large alternating sums. For $n=2$, it reduces to $\theta^k/(1+\theta)^{k+1}$, whose maximum is at $\theta=k$ for $k>0$.

Alternatively, differentiating the integrated [likelihood](../../../../../../likelihood-function.md) gives

$$
\frac{d}{d\theta}\log p_k(\theta)=\frac{k}{\theta}-E[W\mid S=k,\theta].
$$

An interior maximum therefore satisfies $\theta=k/E[W\mid S=k,\theta]$. [Conditional expectations](../../../../../../conditional-expectation.md) of $W$ can be estimated by smoothing the accepted pairs $(\theta,W)$ near each candidate parameter value, yielding another simulation-based score equation. The simple estimator $k/a_{n-1}$ is the unbiased [Watterson estimator](../../../../../../watterson-estimator.md) from part (b), and is not generally the [likelihood](../../../../../../likelihood-function.md) maximizer.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [4](../../4.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
