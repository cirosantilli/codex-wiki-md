<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For one object, the [probabilistic graphical model](../../../../../../probabilistic-graphical-model.md) factorization is

$$
\boxed{
p(x_i,y_i,\xi_i,\eta_i\mid\alpha,\beta,\sigma^2,\mu,\tau^2)
=p(x_i\mid\xi_i)p(y_i\mid\eta_i)
p(\eta_i\mid\xi_i,\alpha,\beta,\sigma^2)
p(\xi_i\mid\mu,\tau^2).}
$$

Each factor is the [normal distribution](../../../../../../normal-distribution.md) density specified by the model. This factorization displays the [conditional independences](../../../../../../conditional-independence.md) of the [latent variables](../../../../../../latent-variable.md) $\xi_i,\eta_i$ and the noisy observations $x_i,y_i$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
