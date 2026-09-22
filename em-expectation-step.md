# EM expectation step

↑ **Parent:** [Expectation-maximization algorithm](expectation-maximization-algorithm.md)

Hold the old [statistical parameters](statistical-parameter.md) fixed when taking the [conditional expectation](conditional-expectation.md), while keeping the candidate [statistical parameters](statistical-parameter.md) $\theta$ variable:

$$
q_t(z)=p_{\theta^{(t)}}(z\mid y),\qquad Q(\theta\mid\theta^{(t)})=\mathbb E_{q_t}[\log p_\theta(y,Z)].
$$

For [independent](independent-random-variables.md) observations in a [finite mixture model](finite-mixture-model.md), $Z_i$ is a hidden component label. [Bayes' theorem](bayes-theorem.md) gives its [mixture responsibilities](mixture-responsibility.md):

$$
r_{ij}^{(t)}=\mathbb P_{\theta^{(t)}}(Z_i=j\mid Y_i=y_i)=\frac{\pi_j^{(t)}f_j(y_i;\theta^{(t)})}{\sum_k\pi_k^{(t)}f_k(y_i;\theta^{(t)})},\qquad \sum_jr_{ij}^{(t)}=1.
$$

These [posterior probabilities](posterior-probability.md) are the [conditional expectations](conditional-expectation.md) of the [mixture allocation indicators](mixture-allocation-indicator.md); they turn hidden counts into fractional counts.[Section 4.3, printed pp. 15-16, especially the paragraph following equation (4.3.3): conditional indicator probabilities and weighted counts](maximum-likelihood-from-incomplete-data-via-the-em-algorithm-by-arthur-pentland-dempster-and-others.md) They condition on a current fixed fit, rather than averaging over a [posterior distribution](bayesian-posterior.md) of the [statistical parameters](statistical-parameter.md). Taking the [conditional expectation](conditional-expectation.md) of the complete-data [log-likelihood](log-likelihood.md) is essential: substituting a single guessed label, or merely substituting the [conditional mean](conditional-expectation.md) into a nonlinear complete-data expression, generally gives a different algorithm.

## ↑ Ancestors (8)

1. [Expectation-maximization algorithm](expectation-maximization-algorithm.md)
2. [Latent variable](latent-variable-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
