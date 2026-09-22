<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The terminal variable $F=\phi(W_T)$ is bounded and hence [square-integrable](../../../../../../square-integrable-function.md). In the completed natural [Brownian filtration](../../../../../../brownian-filtration.md), the [Brownian martingale representation theorem](../../../../../../brownian-martingale-representation-theorem.md) says that any square-integrable $\mathcal F_T$-measurable variable admits a representation

$$
F=\mathbb E F+\int_0^T\beta_u\,dW_u
$$

with $\beta$ predictable and $\mathbb E\int_0^T\beta_u^2du<\infty$. Extend $\beta$ by zero after $T$. Thus the requested constant and integrability are

$$
\boxed{c=\mathbb E\phi(W_T),\qquad\mathbb E\int_0^\infty\beta_u^2du=\operatorname{Var}(\phi(W_T)).}
$$

Expectation determines $c$ uniquely. If two integrands give the same representation, the [Itô isometry](../../../../../../ito-isometry.md) gives $\mathbb E\int_0^\infty(\beta_u-\widetilde\beta_u)^2du=0$. Consequently **$\beta$ is unique up to $d\mathbb P\,du$-almost everywhere equality**, rather than pointwise equality at every time. The corresponding integral martingales are indistinguishable.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
