<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $\mathcal D=(x^{(1)},\ldots,x^{(n)})$ contain [independent](../../../../../../../independent-random-variables.md) complete observations of the $p$-dimensional vector, and let $G$ be a [Directed acyclic graph](../../../../../../../directed-acyclic-graph.md). A [Gaussian Bayesian network](../../../../../../../gaussian-bayesian-network.md) uses, for node $j$,

$$
X_j\mid X_{\operatorname{pa}_G(j)}\sim N\left(\alpha_j+\gamma_j^TX_{\operatorname{pa}_G(j)},\sigma_j^2\right).
$$

Here $\alpha_j$ is an intercept, $\gamma_j$ the vector of parent coefficients, and $\sigma_j^2>0$ the conditional [variance](../../../../../../../variance-split.md); the vector $\theta_G$ collects these [statistical parameters](../../../../../../../statistical-parameter.md). Its [likelihood function](../../../../../../../likelihood-function.md) factors as

$$
p(\mathcal D\mid\theta_G,G)=\prod_{r=1}^n\prod_{j=1}^p p(x_j^{(r)}\mid x_{\operatorname{pa}_G(j)}^{(r)},\theta_j,G).
$$

Choose a proper [statistical parameter](../../../../../../../statistical-parameter.md) [prior distribution](../../../../../../../prior-probability.md) $\pi(\theta_G\mid G)$ and a graph [prior distribution](../../../../../../../prior-probability.md) $\pi(G)$. [Bayes' theorem](../../../../../../../bayes-theorem.md) gives the [Bayesian network structure score](../../../../../../../bayesian-network-structure-score.md), up to the normalization common to graphs,

$$
\boxed{p(G\mid\mathcal D)\propto\pi(G)\,p(\mathcal D\mid G),\qquad p(\mathcal D\mid G)=\int p(\mathcal D\mid\theta_G,G)\pi(\theta_G\mid G)\,d\theta_G.}
$$

The integral is [Bayesian model evidence](../../../../../../../bayesian-model-evidence.md): it averages over [nuisance parameters](../../../../../../../nuisance-parameter.md) rather than substituting their best-fitting values. A graph prior can favor sparse graphs, while the evidence balances fit against the amount of prior [statistical parameter](../../../../../../../statistical-parameter.md) space that predicts the observations well. Compare these scores over admissible [Directed acyclic graphs](../../../../../../../directed-acyclic-graph.md), using enumeration when feasible or a search procedure otherwise; search need not find a global maximum, and observational data need not identify a unique causal orientation.

A [conjugate prior](../../../../../../../conjugate-prior.md) makes the integral analytic. For example, for $\eta_j=(\alpha_j,\gamma_j)$ take $\eta_j\mid\sigma_j^2\sim N(m_j,\sigma_j^2V_j)$, $\sigma_j^2\sim\operatorname{IG}(a_j,b_j)$, where $V_j$ is [positive-definite matrix](../../../../../../../positive-definite-matrix.md) and $a_j,b_j>0$; these are [independent](../../../../../../../independent-random-variables.md) local [normal-inverse-gamma priors](../../../../../../../normal-inverse-gamma-prior.md). Under prior [independence](../../../../../../../independent-random-variables.md) between nodes, the evidence is a product of local regression evidences. Each posterior has the same family, so the local integral is the ratio of prior and posterior normalization constants, with the likelihood's constants included. This avoids costly numerical integration and makes local graph updates inexpensive. Hyperparameters must be specified coherently if score equivalence between observationally equivalent graphs is desired; arbitrary local priors do not automatically have that property.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
