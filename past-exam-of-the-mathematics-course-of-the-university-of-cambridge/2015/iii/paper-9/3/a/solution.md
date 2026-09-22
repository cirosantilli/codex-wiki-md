<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a [Lipschitz continuous](../../../../../../lipschitz-continuity.md) [cutoff function](../../../../../../cutoff-function.md) $\eta$ which equals one on $B_R(x_0)$, vanishes outside $B_{2R}(x_0)$, takes values in $[0,1]$, and has $|\nabla\eta|\leq2/R$. Its [gradient](../../../../../../gradient.md) is supported in the [annulus](../../../../../../annulus-mathematics.md) $A_R=B_{2R}(x_0)\setminus B_R(x_0)$. The function $\eta^2(u-c)$ is an admissible [test function](../../../../../../test-function.md) in the zero-boundary [Sobolev space](../../../../../../sobolev-space-split.md) for the [weak solution](../../../../../../weak-solution.md), by approximation with smooth compactly supported [test functions](../../../../../../test-function.md). If $\Lambda_0$ bounds the [operator norm](../../../../../../operator-norm.md) of $(a^{ij})$, we can take $\Lambda_0=n\Lambda$. The weak equation and [uniform ellipticity](../../../../../../uniformly-elliptic-operator.md) give

$$
\lambda\int\eta^2|\nabla u|^2\leq2\Lambda_0\int_{A_R}\eta|\nabla u|\,|u-c|\,|\nabla\eta|.
$$

[Young inequality](../../../../../../young-s-inequality-for-products.md) bounds the right side by

$$
\frac\lambda2\int\eta^2|\nabla u|^2+\frac{2\Lambda_0^2}{\lambda}\int_{A_R}|u-c|^2|\nabla\eta|^2.
$$

After absorption, this [annular Caccioppoli inequality](../../../../../../annular-caccioppoli-inequality.md) is

$$
\boxed{\int_{B_R(x_0)}|\nabla u|^2\leq\frac{16\Lambda_0^2}{\lambda^2R^2}\int_{A_R}|u-c|^2.}
$$

The dimension is fixed in the notation $C(\lambda,\Lambda)$ of the question; with the entrywise coefficient bound its dependence on $n$ is absorbed there. If the larger ball merely lies in $B$ without its closure being compactly contained, approximation from smaller [cutoff functions](../../../../../../cutoff-function.md) gives the same admissible [test function](../../../../../../test-function.md) and estimate. Crucially, the right side uses only the [annulus](../../../../../../annulus-mathematics.md), where the [cutoff function](../../../../../../cutoff-function.md) varies. The constant $c$ is arbitrary because constants have zero [gradient](../../../../../../gradient.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
