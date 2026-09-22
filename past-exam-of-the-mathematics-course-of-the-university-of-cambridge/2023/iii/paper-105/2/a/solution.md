<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The zero-boundary [Sobolev space](../../../../../../sobolev-space-split.md) is

$$
H_0^1(\Omega)=\overline{C_c^\infty(\Omega)}^{\,H^1}.
$$

On it define

$$
(u,v)_{H_0^1}=\int_\Omega\nabla u\cdot\nabla v.
$$

If this quadratic form vanishes, then $\nabla u=0$. The [Poincaré inequality](../../../../../../poincare-inequality.md) gives

$$
\|u\|_{L^2}\leq C\|\nabla u\|_{L^2}=0,
$$

so $u=0$. It is therefore an inner product, and its norm is equivalent to the usual $H^1$ norm.

A function $u\in H_0^1(\Omega)$ is a [weak solution](../../../../../../weak-solution.md) when

$$
\int_\Omega\nabla u\cdot\nabla\varphi
=-\int_\Omega f\varphi
\qquad\text{for every }\varphi\in H_0^1(\Omega).
$$

This follows from [integration by parts](../../../../../../integration-by-parts.md) and incorporates the homogeneous [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) through membership in $H_0^1$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
