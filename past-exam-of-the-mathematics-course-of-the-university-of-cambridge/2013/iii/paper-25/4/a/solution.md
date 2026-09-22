<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The drift $b(z)=\tanh z$ has derivative $b'(z)=1/\cosh^2z$, so $|b'(z)|\le1$. Hence it is globally Lipschitz. The diffusion coefficient $\sigma(z)=1$ is globally Lipschitz as well, and both coefficients satisfy a linear growth bound.

The [global existence theorem for stochastic differential equations with Lipschitz coefficients](../../../../../../global-existence-theorem-for-stochastic-differential-equations-with-lipschitz-coefficients.md) states that globally Lipschitz coefficients with linear growth give, for each deterministic initial point, an adapted continuous [strong solution of a stochastic differential equation](../../../../../../strong-solution-of-a-stochastic-differential-equation.md) on every finite interval, with pathwise uniqueness and no finite-time explosion. Applying this theorem gives **a unique strong solution for every $X_0=x\in\mathbb R$**, satisfying

$$
X_t=x+\int_0^t\tanh X_s\,ds+W_t.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
