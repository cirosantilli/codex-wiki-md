<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The joint density factors as $p(\psi)\prod_jp(\theta_j\mid\psi)p(y_j\mid\theta_j)$. In the [full conditional distribution](../../../../../../full-conditional-distribution.md) of $\theta_i$, all factors not involving $\theta_i$ cancel. The remaining [likelihood function](../../../../../../likelihood-function.md) and [exponential distribution](../../../../../../exponential-distribution.md) prior give

$$
p(\theta_i\mid\theta_{-i},\psi,y)\propto\theta_i^{y_i}e^{-\theta_i}e^{-\psi\theta_i}
=\theta_i^{y_i}e^{-(1+\psi)\theta_i}.
$$

In shape–rate convention this is $\boxed{\theta_i\mid\psi,y\sim\operatorname{Gamma}(y_i+1,\,1+\psi)}$, a special case of the [Gamma–Poisson hierarchical model](../../../../../../gamma-poisson-hierarchical-model.md). It depends only on the node's observed child $y_i$ and parent $\psi$, as required for its [Gibbs sampler](../../../../../../gibbs-sampler.md) update.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
