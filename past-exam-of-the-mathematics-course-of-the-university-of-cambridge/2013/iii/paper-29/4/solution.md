<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [reversible-jump Markov chain Monte Carlo](../../../../../reversible-jump-markov-chain-monte-carlo.md) state comprises the model index and that model's parameter. Its unnormalized posterior density in model $j$ is

$$
h_j(\theta)=\varpi_j p_j(x\mid\theta)\pi_j(\theta).
$$

For models of equal dimension, choose model $k\ne j$ with probability $s_{jk}(\theta)$ and propose $\theta'$ using density $q_{jk}(\theta'\mid\theta)$ on the destination parameter space. The [equal-dimension reversible-jump acceptance probability](../../../../../equal-dimension-reversible-jump-acceptance-probability.md) is

$$
\boxed{a((j,\theta),(k,\theta'))=
\min\left\{1,\frac{h_k(\theta')s_{kj}(\theta')q_{kj}(\theta\mid\theta')}
{h_j(\theta)s_{jk}(\theta)q_{jk}(\theta'\mid\theta)}\right\}.}
$$

On acceptance change both model and parameter; on rejection retain both. Choose model proposals connecting all models of positive posterior mass and within-model kernels exploring their supports, with aperiodicity, to obtain an ergodic chain. Include within-model updates targeting its conditional [posterior](../../../../../bayesian-posterior.md), and use model occupation proportions after the initial transient to estimate [posterior](../../../../../bayesian-posterior.md) model probabilities. The formula includes the model [prior probabilities](../../../../../prior-probability.md), parameter [prior densities](../../../../../prior-density.md), [likelihoods](../../../../../likelihood-function.md), reverse model-selection probability, and reverse parameter-proposal density.

This direct-density formula is [Metropolis–Hastings algorithm](../../../../../metropolis-hastings-algorithm.md) on a disjoint union of equal-dimensional spaces. If instead a move uses a deterministic bijection $T:(\theta,u)\mapsto(\theta',u')$ with auxiliary proposal densities $g_{jk}(u\mid\theta)$ and $g_{kj}(u'\mid\theta')$, use

$$
\min\left\{1,\frac{h_k(\theta')s_{kj}(\theta')g_{kj}(u'\mid\theta')}
{h_j(\theta)s_{jk}(\theta)g_{jk}(u\mid\theta)}
\left|\det\frac{\partial(\theta',u')}{\partial(\theta,u)}\right|\right\}.
$$

The [Jacobian determinant](../../../../../jacobian-determinant.md) is one for identity matching, but equal model dimensions alone do not make a nonlinear map volume-preserving. For a direct proposal density the change of variables is already included in that density, so no additional Jacobian factor is inserted.

For the two Poisson models, use the shape-rate convention for the [gamma distribution](../../../../../gamma-distribution.md):

$$
\pi(g)=\frac{b^a}{\Gamma(a)}g^{a-1}e^{-bg},\qquad g>0.
$$

If $b$ denotes scale instead, replace every occurrence of the rate $b$ below by $1/b$. Introduce the inactive $\gamma_2$ under model $2$ with the proper [pseudo-prior](../../../../../pseudo-prior.md) $\pi(\gamma_2)$, [independent](../../../../../independent-random-variables.md) of $\gamma_1$. This [pseudo-prior augmentation for model comparison](../../../../../pseudo-prior-augmentation-for-model-comparison.md) does not change model $2$'s marginal likelihood because the inactive density integrates to one. The two augmented targets on the same positive quadrant are

$$
h_1=\tfrac12 L_1(\gamma_1,\gamma_2)\pi(\gamma_1)\pi(\gamma_2),\qquad
h_2=\tfrac12 L_2(\gamma_1)\pi(\gamma_1)\pi(\gamma_2),
$$

where

$$
L_1=\frac{e^{-(\gamma_1+\gamma_2)}\gamma_1^{x_1}\gamma_2^{x_2}}{x_1!x_2!},\qquad
L_2=\frac{e^{-2\gamma_1}\gamma_1^{x_1+x_2}}{x_1!x_2!}.
$$

Use a symmetric cross-model proposal that flips the model label and leaves both parameters unchanged. The matching map is the identity, with unit [Jacobian determinant](../../../../../jacobian-determinant.md), and the common prior factors cancel. Hence the **model-switch acceptance probabilities** are

$$
\boxed{a_{1\to2}=\min\left\{1,e^{\gamma_2-\gamma_1}\left(\frac{\gamma_1}{\gamma_2}\right)^{x_2}\right\},\qquad
a_{2\to1}=\min\left\{1,e^{\gamma_1-\gamma_2}\left(\frac{\gamma_2}{\gamma_1}\right)^{x_2}\right\}.}
$$

Only the second observation's factor changes because $\gamma_1$ is retained as its shared candidate mean. Evaluate the ratio on a logarithmic scale as $\gamma_2-\gamma_1+x_2(\log\gamma_1-\log\gamma_2)$ for the first direction.

For within-model moves, [Poisson-gamma conjugacy](../../../../../poisson-gamma-conjugacy.md) gives exact [Gibbs sampling](../../../../../gibbs-sampler.md) refreshes:

$$
\begin{aligned}
M_1:\quad&\gamma_1\mid x\sim\operatorname{Gamma}(a+x_1,b+1),\quad
\gamma_2\mid x\sim\operatorname{Gamma}(a+x_2,b+1),\\
M_2:\quad&\gamma_1\mid x\sim\operatorname{Gamma}(a+x_1+x_2,b+2),\quad
\gamma_2\mid x\sim\operatorname{Gamma}(a,b).
\end{aligned}
$$

The two draws are conditionally [independent](../../../../../independent-random-variables.md) within either model. Choose with fixed positive probabilities between this block refresh and the cross-model proposal. Both moves preserve the augmented [posterior](../../../../../bayesian-posterior.md); refreshing the inactive parameter maintains its correct distribution and supports mixing. **The fraction of retained states labelled $M_j$ estimates $\mathbb P(M_j\mid x)$**.

An equivalent literal dimension-changing implementation deletes $\gamma_2$ on a proposed $1\to2$ move, and on a $2\to1$ move draws an auxiliary $u\sim\operatorname{Gamma}(a,b)$ and sets $\gamma_2=u$. The birth matching has $1+1=2+0$ dimensions and unit [Jacobian determinant](../../../../../jacobian-determinant.md). Its proposal density cancels the new parameter's prior density, giving the same acceptance ratios above for symmetric selection of move directions. This provides suitable moves without storing an inactive parameter.

For an independent check of [Poisson mean equality model comparison](../../../../../poisson-mean-equality-model-comparison.md), the exact [Bayes factor](../../../../../bayes-factor.md) is

$$
\frac{m_2(x)}{m_1(x)}=
\frac{\Gamma(a+x_1+x_2)\Gamma(a)}{\Gamma(a+x_1)\Gamma(a+x_2)}
\frac{(b+1)^{2a+x_1+x_2}}{b^a(b+2)^{a+x_1+x_2}}.
$$

It follows by integrating the two gamma likelihood kernels; the common factorial terms cancel. With equal model priors, the exact posterior probability of $M_2$ is $m_2/(m_1+m_2)$, which can also be used to check the [RJ-MCMC](../../../../../reversible-jump-markov-chain-monte-carlo.md) occupation estimate.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
