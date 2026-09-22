<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [expectation-maximization algorithm](../../../../../../expectation-maximization-algorithm.md) alternates conditional averaging over missing data with maximization over the parameter. Start at a parameter value $\theta^{(0)}$ for which the observed [likelihood function](../../../../../../likelihood-function.md) is positive. At iteration $t$, its E-step forms

$$
Q(\theta\mid\theta^{(t)})=E_{\theta^{(t)}}[\log f(x,Z;\theta)\mid x],
$$

using the current conditional law of $Z$ but treating $\theta$ as the candidate parameter. Its M-step takes

$$
\boxed{\theta^{(t+1)}\in\arg\max_\theta Q(\theta\mid\theta^{(t)}).}
$$

Repeat until the parameter or observed [log-likelihood](../../../../../../log-likelihood.md) stabilizes. An increase of $Q$ implies an increase of the observed [log-likelihood](../../../../../../log-likelihood.md): if $q_t(z)=f(z\mid x;\theta^{(t)})$, then

$$
\ell(\theta)-\ell(\theta^{(t)})
=Q(\theta\mid\theta^{(t)})-Q(\theta^{(t)}\mid\theta^{(t)})
 +D_{\mathrm{KL}}(q_t\|f(\cdot\mid x;\theta)),
$$

where [Kullback-Leibler divergence](../../../../../../kullback-leibler-divergence.md) is nonnegative. In general this monotonicity does not guarantee a global maximum; distinct initializations may approach different stationary points. The particular observed [log-likelihood](../../../../../../log-likelihood.md) below is concave, which makes a stronger conclusion possible there.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
