<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First choose a [test function](../../../../../../test-function.md) $v\in C_c^\infty(U)$. The [weak formulation](../../../../../../weak-formulation.md) and [integration by parts](../../../../../../integration-by-parts.md) give

$$
\int_U(-\Delta u-f)v\,dx=0.
$$

The [fundamental lemma of the calculus of variations](../../../../../../fundamental-lemma-of-the-calculus-of-variations.md) implies $-\Delta u=f$ pointwise because $u\in C^2(\overline U)$ and $f$ is continuous. The [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) on $\Gamma_1$ already follows from $u\in V$ and continuity of $u$.

For arbitrary $v\in V$, [Green's first identity](../../../../../../green-s-first-identity.md) and the interior equation now reduce the weak identity to

$$
\int_{\Gamma_2}(\partial_\nu u)v\,dS=0.
$$

The traces of smooth members of $V$ can be chosen freely on compact subsets of $\Gamma_2$. Another application of the [fundamental lemma of the calculus of variations](../../../../../../fundamental-lemma-of-the-calculus-of-variations.md), now on the boundary, gives $\partial_\nu u=0$ pointwise on $\Gamma_2$. Hence $u$ is a [classical solution](../../../../../../classical-solution.md) of the complete [mixed boundary value problem](../../../../../../mixed-boundary-condition.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
