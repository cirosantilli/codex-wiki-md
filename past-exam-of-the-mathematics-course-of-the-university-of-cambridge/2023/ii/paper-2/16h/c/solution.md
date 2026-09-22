<h1 id="16h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Suppose first that $\delta>2$ is [multiplicatively closed](../../../../../../multiplicatively-closed-ordinal.md). It is also additively closed. Indeed, for $\beta,\gamma<\delta$, let $\mu=\max\{\beta,\gamma\}$. Monotonicity of [ordinal addition](../../../../../../ordinal-addition.md) gives

$$
\beta+\gamma\leq\mu+\mu=\mu\,2<\delta,
$$

where the last inequality uses $\mu<\delta$, $2<\delta$, and multiplicative closure. Part (b) therefore gives

$$
\delta=\omega^\lambda
$$

for some nonzero ordinal $\lambda$.

For any $\rho,\sigma<\lambda$, strict monotonicity gives

$$
\omega^\rho,\omega^\sigma<\omega^\lambda=\delta.
$$

Multiplicative closure and the exponent law now imply

$$
\omega^{\rho+\sigma}
=\omega^\rho\omega^\sigma
<\omega^\lambda,
$$

hence $\rho+\sigma<\lambda$. Thus $\lambda$ is additively closed, and part (b) gives $\lambda=\omega^\alpha$. Consequently

$$
\boxed{\delta=\omega^{\omega^\alpha}}.
$$

Conversely, let $\delta=\omega^\lambda$ with $\lambda=\omega^\alpha$. By part (b), $\lambda$ is additively closed. Take nonzero $\beta,\gamma<\delta$, with leading exponents $\rho,\sigma<\lambda$ in [Cantor normal form](../../../../../../cantor-normal-form.md). If $\gamma$ is finite, the product $\beta\gamma$ has leading exponent $\rho<\lambda$. If $\gamma$ is infinite, the [leading exponent of an ordinal product](../../../../../../leading-exponent-of-an-ordinal-product.md) is

$$
\rho+\sigma<\lambda
$$

by additive closure of $\lambda$. In either case

$$
\beta\gamma<\omega^\lambda=\delta.
$$

Products involving zero are immediate, so $\delta$ is multiplicatively closed. This is the [multiplicative closure criterion for a power of omega](../../../../../../multiplicative-closure-criterion-for-a-power-of-omega.md) and completes both directions.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [16H](../../16h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
