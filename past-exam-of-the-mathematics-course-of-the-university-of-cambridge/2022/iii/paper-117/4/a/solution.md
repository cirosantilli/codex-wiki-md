<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $g\in\mathcal H_N$, write

$$
\widehat g(\alpha)=\sum_{n\leq N}g(n)e(\alpha n).
$$

The [orthogonality of complex exponentials](../../../../../../orthogonality-of-complex-exponentials.md) converts the [linear configuration count](../../../../../../linear-configuration-count.md) into

$$
T(g,g,g,g)=\int_0^1\widehat g(\alpha)\widehat g(2\alpha)\widehat g(3\alpha)\widehat g(-4\alpha)\,d\alpha.
$$

Expand the difference between the products for $g_1$ and $g_2$ by changing one factor at a time. A typical term is

$$
\int_0^1\bigl(\widehat g_1(\alpha)-\widehat g_2(\alpha)\bigr)\widehat h_2(2\alpha)\widehat h_3(3\alpha)\widehat h_4(-4\alpha)\,d\alpha,
$$

where each $h_j$ is either $g_1$ or $g_2$. The assumed [uniform norm](../../../../../../supremum-norm.md) bound controls the first factor by $\varepsilon N$. The substitution $\alpha\mapsto k\alpha$ preserves an integral over the [circle group](../../../../../../circle-group.md), so [Hölder's inequality](../../../../../../holder-s-inequality.md) and the three supplied $L^3$ bounds give

$$
\int_0^1\prod_{j=2}^4|\widehat h_j(k_j\alpha)|\,d\alpha
\leq\prod_{j=2}^4\left(\int_0^1|\widehat h_j(\alpha)|^3\,d\alpha\right)^{1/3}
\ll N^2.
$$

Each of the four terms is therefore $O(\varepsilon N^3)$, and hence

$$
\boxed{|T(g_1,g_1,g_1,g_1)-T(g_2,g_2,g_2,g_2)|=O(\varepsilon N^3).}
$$

This is [Fourier stability of a linear configuration count](../../../../../../fourier-stability-of-a-linear-configuration-count.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 117](../../../paper-117-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
