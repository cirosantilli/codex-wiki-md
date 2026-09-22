<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [Bradley-Terry model](../../../../../bradley-terry-model.md) assigns comparison probability $q_i=\theta_i/(\theta_i+\theta_{i+1})$ to each observed edge. Up to factors independent of the parameters, its [likelihood function](../../../../../likelihood-function.md) is

$$
L(\theta)=\prod_{i=0}^{n-1}q_i^{mp_i}(1-q_i)^{m(1-p_i)}.
$$

The comparison graph is a [path graph](../../../../../path-graph.md), hence a [tree](../../../../../tree-graph-theory.md). After fixing $\theta_n=1$, its edge ratios are unconstrained positive coordinates: every collection $r_i=\theta_i/\theta_{i+1}>0$ determines uniquely $\theta_i=\prod_{k=i}^{n-1}r_k$.

For a convenient strict-[concavity](../../../../../concave-function.md) calculation, use the [edge log-ratios in a Bradley-Terry comparison tree](../../../../../edge-log-ratios-in-a-bradley-terry-comparison-tree.md) $\eta_i=\log r_i$. The [log-likelihood](../../../../../log-likelihood.md) separates as

$$
\ell(\eta)=m\sum_{i=0}^{n-1}\left[p_i\eta_i-\log(1+e^{\eta_i})\right]+\text{constant}.
$$

Each derivative is $m(p_i-q_i)$, where $q_i$ is the [logistic function](../../../../../logistic-function.md) of $\eta_i$, and each second derivative is $-mq_i(1-q_i)<0$. Because $0<p_i<1$, there is a unique finite global maximum at

$$
\widehat\eta_i=\log\frac{p_i}{1-p_i},\qquad \widehat q_i=p_i.
$$

Converting back gives the [Bradley-Terry maximum-likelihood estimate on a path](../../../../../bradley-terry-maximum-likelihood-estimate-on-a-path.md):

$$
\boxed{\widehat\theta_n=1,\qquad
\widehat\theta_i=\prod_{k=i}^{n-1}\frac{p_k}{1-p_k},\quad 0\leq i<n.}
$$

Equivalently, recurse backwards using $\widehat\theta_i=\widehat\theta_{i+1}p_i/(1-p_i)$. All estimates are finite and positive. The sample size $m$ changes the curvature of the [likelihood](../../../../../likelihood-function.md) but not this maximizer; absence of comparison cycles is what permits every empirical edge proportion to be fitted simultaneously.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
