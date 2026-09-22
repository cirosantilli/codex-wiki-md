<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Integrate the [latent variable](../../../../../../latent-variable.md) out to obtain the hospital's [marginal likelihood](../../../../../../bayesian-model-evidence.md):

$$
p(y_i\mid\psi)=\frac{\psi}{y_i!}\int_0^\infty\theta^{y_i}e^{-(1+\psi)\theta}d\theta
=\frac{\psi}{(1+\psi)^{y_i+1}}.
$$

For $\phi=(1+\psi)^{-1}$ this becomes $\boxed{p(y_i\mid\phi)=(1-\phi)\phi^{y_i}}$. It is a [geometric distribution](../../../../../../geometric-distribution.md) on the nonnegative integers, with success probability $1-\phi$. The transformation concerns the likelihood, so no Jacobian is inserted here.

## ↑ Ancestors (11)

1. [C](../c.md)
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
