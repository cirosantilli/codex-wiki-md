# Bayesian network structure score

↑ **Parent:** [Bayesian network](bayesian-network.md)

For observations $\mathcal D$ and graph $G$, [Bayes' theorem](bayes-theorem.md) gives $p(G\mid\mathcal D)\propto\pi(G)\int p(\mathcal D\mid\theta_G,G)\pi(\theta_G\mid G)\,d\theta_G$. Here $\pi(G)$ is the graph [prior distribution](prior-probability.md) and $\theta_G$ the local distribution [statistical parameters](statistical-parameter.md). The integral is [Bayesian model evidence](bayesian-model-evidence.md); it averages over [nuisance parameters](nuisance-parameter.md) with a proper [statistical parameter](statistical-parameter.md) [prior distribution](prior-probability.md). For [independent](independent-random-variables.md) complete observations, the node-factorized [likelihood function](likelihood-function.md) and [independence](independent-random-variables.md) of local [statistical parameter](statistical-parameter.md) [prior distributions](prior-probability.md) make the evidence factor over nodes; suitable [conjugate priors](conjugate-prior.md) can make the local integrals analytic. With missing node observations, integrating out unobserved values can couple the local parameters, so [independence](independent-random-variables.md) of local [prior distributions](prior-probability.md) alone does not guarantee this factorization. Proper priors and coherent hyperparameters matter for comparing different graphs.

## ↑ Ancestors (7)

1. [Bayesian network](bayesian-network.md)
2. [Probabilistic graphical model](probabilistic-graphical-model.md)
3. [Statistical model](statistical-model-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-207/2/b/iii/solution.md)
