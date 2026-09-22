<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The observed-data [likelihood function](../../../../../../likelihood-function.md) integrates out the [latent variable](../../../../../../latent-variable.md):

$$
L(x\mid\theta)=\int f(x,z;\theta)\,dz.
$$

Choose an initial parameter $\theta^{(0)}$ with positive [likelihood](../../../../../../likelihood-function.md). At iteration $t$, the E-step of the [EM algorithm](../../../../../../expectation-maximization-algorithm.md) forms the entire expected complete-data [log-likelihood](../../../../../../log-likelihood.md)

$$
Q(\theta\mid\theta^{(t)})=\int h_t(z)\log f(x,z;\theta)\,dz,\qquad h_t(z)=\frac{f(x,z;\theta^{(t)})}{L(x\mid\theta^{(t)})}.
$$

The expectation is under the conditional missing-data law at the old parameter, while the argument $\theta$ remains free. The M-step then chooses

$$
\boxed{\theta^{(t+1)}\in\operatorname*{arg\,max}_{\theta}Q(\theta\mid\theta^{(t)}).}
$$

The observed data $x$ stay fixed throughout. This is not obtained merely by substituting the conditional mean of $z$ into a nonlinear [log-likelihood](../../../../../../log-likelihood.md): the expectation of all required complete-data terms must be taken. A generalized EM step only requires $Q(\theta^{(t+1)}\mid\theta^{(t)})\ge Q(\theta^{(t)}\mid\theta^{(t)})$, which suffices for the monotonicity proved next. Exact maximization assumes that an admissible maximizer exists.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
