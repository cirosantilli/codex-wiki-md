<h1 id="4d/solution">Solution</h1>

↑ **Parent:** [4D](../4d.md)

Introduce a [Lagrange multiplier](../../../../../lagrange-multiplier.md) $\lambda$ for the normalization and vary

$$
J[u]=\int_D\bigl(|\nabla u|^2-\lambda u^2\bigr)\,dx\,dy.
$$

For a smooth variation $u+\varepsilon\eta$ with $\eta=0$ on $\partial D$, [integration by parts](../../../../../integration-by-parts.md) gives

$$
\left.\frac d{d\varepsilon}J[u+\varepsilon\eta]\right|_{\varepsilon=0}
=2\int_D(\nabla u\mathbin{\cdot}\nabla\eta-\lambda u\eta)
=-2\int_D(\nabla^2u+\lambda u)\eta.
$$

The [fundamental lemma of the calculus of variations](../../../../../fundamental-lemma-of-the-calculus-of-variations.md) therefore yields the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md)

$$
\boxed{\nabla^2u+\lambda u=0}.
$$

Multiplying by $u$ and integrating, while using

$$
\nabla\mathbin{\cdot}(u\nabla u)=|\nabla u|^2+u\nabla^2u,
$$

the [divergence theorem](../../../../../divergence-theorem.md) and $u=0$ on the boundary give

$$
0=I[u]+\int_Du\nabla^2u=I[u]-\lambda\int_Du^2.
$$

The normalization is one, so the multiplier equals the stationary value:

$$
\boxed{\lambda=I[u]}.
$$

## ↑ Ancestors (10)

1. [4D](../4d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
