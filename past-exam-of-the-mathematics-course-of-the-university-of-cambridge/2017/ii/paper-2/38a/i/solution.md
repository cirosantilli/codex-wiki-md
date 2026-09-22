<h1 id="38a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume sufficient smoothness up to the boundary for uniform Taylor remainders, for example $u\in C^8(\overline\Omega)$ and $f=\Delta u\in C^6(\overline\Omega)$. Direct Taylor expansion of the [nine-point finite-difference stencil](../../../../../../nine-point-finite-difference-stencil.md) gives

$$
\Gamma_9u=h^2\Delta u+\frac{h^4}{12}\Delta^2u
+\frac{h^6}{360}(u_{xxxxxx}+u_{yyyyyy}+5u_{xxxxyy}+5u_{xxyyyy})+O(h^8).
$$

Thus the normalized [local truncation error](../../../../../../local-truncation-error.md) $h^{-2}\Gamma_9u-f$ is $\boxed{O(h^2)}$. The unscaled residual $\Gamma_9u-h^2f$ is $O(h^4)$. Stating the normalization avoids ambiguity in the meaning of truncation order.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [38A](../../38a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
