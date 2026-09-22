<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The marginal [Metropolis–Hastings algorithm](../../../../../../metropolis-hastings-algorithm.md) avoids storing allocation labels, but each component update changes every mixture likelihood term. Cache component contributions, calculate [log-likelihoods](../../../../../../log-likelihood.md) stably and tune the [proposal scale and random-walk Metropolis efficiency](../../../../../../proposal-scale-and-random-walk-metropolis-efficiency.md) during a pilot run; then fix proposal scales or use a justified adaptive scheme. Means and variances may be strongly dependent, making separate random walks inefficient. Weight proposals must respect the simplex, variance proposals must respect positivity, and the displayed acceptance ratios must retain all relevant priors and proposal corrections.

The augmented [Gibbs sampler](../../../../../../gibbs-sampler.md) uses elementary conditionals and typically costs order $nk$ for a label sweep, followed by sufficient-statistic updates. It avoids Metropolis rejections in these conditional draws, but does not remove slow mixing: ambiguous allocations can lock means, variances and labels into strongly coupled configurations. Empty components must be updated from their priors, not deleted automatically. The proper inverse-gamma scale $\beta>0$ suppresses arbitrarily small variances even though an unregularized Gaussian-mixture likelihood can be singular.

With exchangeable component priors, [label switching](../../../../../../label-switching.md) creates $k!$ equivalent posterior modes. Ordering component means is an identification constraint, not an innocuous change unless the intended inferential model is made explicit. Predictive density and permutation-invariant summaries avoid arbitrary labelling; component-specific summaries require an appropriate relabelling convention. If the Dirichlet parameters differ between components, exact label symmetry may be broken, but substantial multimodality can remain.

Use dispersed initial states, multiple chains and diagnostics on several scientifically relevant functions. Report [effective sample size of a Markov chain](../../../../../../effective-sample-size-of-a-markov-chain.md) and [Monte Carlo error](../../../../../../monte-carlo-error.md) estimates, not just a large iteration count. Burn-in can reduce initialization bias but does not prove convergence; thinning cannot by itself cure poor exploration. **Closed-form Gibbs updates simplify computation, while reliable inference still requires adequate exploration of the posterior.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
