<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each person, infection occurs with probability $\lambda$ and, conditional on infection, a GP visit occurs with probability $\rho_G$. Independent [Bernoulli thinning](../../../../../../bernoulli-thinning.md) therefore gives visit probability $\lambda\rho_G$. More explicitly, the [probability generating function](../../../../../../probability-generating-function.md) is

$$
\mathbb E[s^{Y_G}\mid N,\lambda,\rho_G]
=\bigl(1-\lambda+\lambda(1-\rho_G+\rho_Gs)\bigr)^N
=(1-\lambda\rho_G+\lambda\rho_Gs)^N.
$$

Thus

$$
Y_G\mid N,\lambda,\rho_G\sim
\operatorname{Binomial}(N,\lambda\rho_G),
$$

and the likelihood is

$$
\boxed{L_G(\lambda,\rho_G;y_G)
=\binom Ny_G(\lambda\rho_G)^{y_G}
(1-\lambda\rho_G)^{N-y_G}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
