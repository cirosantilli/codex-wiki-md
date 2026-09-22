<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Conditioned on the parameters, the [data augmentation](../../../../../../../data-augmentation.md) labels are independent. By [Bayes' theorem](../../../../../../../bayes-theorem.md), the [conditional probability](../../../../../../../conditional-probability.md) of component $i$ for observation $j$ is

$$
\boxed{P(z_j=i\mid\boldsymbol\mu,\mathbf v,\boldsymbol\omega,\mathbf x)=r_{ji}=\frac{\omega_i\varphi(x_j;\mu_i,v_i)}{\sum_{h=1}^k\omega_h\varphi(x_j;\mu_h,v_h)}.}
$$

This is the [mixture responsibility](../../../../../../../mixture-responsibility.md). Draw an independent [uniform random variable](../../../../../../../uniform-random-variable.md) and select $i$ using the cumulative sums of $(r_{j1},\ldots,r_{jk})$. Refresh every label before recomputing the component sufficient statistics for the next [Gibbs sampler](../../../../../../../gibbs-sampler.md) sweep. Numerically, form the log scores $\log\omega_i-\tfrac12\log v_i-(x_j-\mu_i)^2/(2v_i)$, subtract their maximum and exponentiate before normalization.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 43](../../../../paper-43-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
