<h1 id="4f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let

$$
U=X_1+X_2,\qquad V=X_1-X_2.
$$

They are jointly normal because they are linear combinations of a Gaussian [vector](../../../../../../vector.md). When $\sigma_1=\sigma_2=\sigma$,

$$
\operatorname{cov}(U,V)
=\operatorname{var}(X_1)-\operatorname{var}(X_2)=0.
$$

Hence [uncorrelated jointly normal variables are independent](../../../../../../uncorrelated-jointly-normal-variables-are-independent.md). Their means and variances are

$$
\mathbb EU=\mu_1+\mu_2,
\qquad
\operatorname{var}U=2\sigma^2(1+\rho),
$$

and

$$
\mathbb EV=\mu_1-\mu_2,
\qquad
\operatorname{var}V=2\sigma^2(1-\rho).
$$

Therefore

$$
\boxed{U\sim N(\mu_1+\mu_2,2\sigma^2(1+\rho))},
$$



$$
\boxed{V\sim N(\mu_1-\mu_2,2\sigma^2(1-\rho))},
$$

independently.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4F](../../4f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
