<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $X$ denote the observed data, $Z$ the unobserved data and $\theta$ the model parameters. The [expectation-maximization algorithm](../../../../../expectation-maximization-algorithm.md) works with the complete-data [log-likelihood](../../../../../log-likelihood.md) $\ell_c(\theta;X,Z)$. Given $\theta^{(r)}$, its **E-step** computes

$$
Q(\theta\mid\theta^{(r)})=E_{\theta^{(r)}}[\ell_c(\theta;X,Z)\mid X],
$$

where the [conditional expectation](../../../../../conditional-expectation.md) uses the old parameter, while $\theta$ remains the argument to maximize. Its **M-step** chooses $\theta^{(r+1)}$ maximizing this function over the parameter space. [EM likelihood monotonicity](../../../../../em-likelihood-monotonicity.md) ensures that an M-step increasing $Q$ cannot decrease the observed-data [log-likelihood](../../../../../log-likelihood.md). It does not guarantee a global maximum, so convergence and any parameter constraints must still be checked.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
