<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

By part (i), finite-dimensional continuous [unitary representations](../../../../../../unitary-representation.md) separate points of the compact [group](../../../../../../group-split.md). More explicitly, if every representation sent some $g\ne e$ to the identity, all their [matrix coefficients](../../../../../../matrix-coefficient.md) would take the same values at $g$ and $e$. Uniform density would force every continuous scalar [function](../../../../../../function-split.md) to do so, contradicting separation of points on a compact Hausdorff space. Hence

$$
\bigcap_\theta\ker\theta=\{e\}.
$$

Each representation kernel is a closed [normal subgroup](../../../../../../normal-subgroup.md). We claim that the intersection can be reduced to finitely many kernels. Begin with $K_0=G$. If $K_j\ne\{e\}$, choose $g_j\in K_j\setminus\{e\}$ and a representation $\theta_{j+1}$ with $\theta_{j+1}(g_j)\ne I$. Then

$$
K_{j+1}=K_j\cap\ker\theta_{j+1}\subsetneq K_j.
$$

An indefinite continuation would violate the [descending chain condition](../../../../../../descending-chain-condition.md) for [closed subgroups](../../../../../../closed-subgroup.md). Thus after finitely many steps, $K_N=\{e\}$.

The direct sum $\rho=\theta_1\oplus\cdots\oplus\theta_N$ is consequently a finite-dimensional [faithful representation](../../../../../../faithful-representation.md), with continuous injective [homomorphism](../../../../../../homomorphism.md)

$$
\rho:G\longrightarrow U(d).
$$

Compactness of $G$ makes this a homeomorphism onto a compact, hence closed, image. The [closed-subgroup theorem](../../../../../../closed-subgroup-theorem.md) makes that image an embedded [Lie subgroup](../../../../../../lie-subgroup.md) of the finite-dimensional unitary [group](../../../../../../group-split.md). Transporting its smooth structure to $G$ proves

$$
\boxed{G\text{ is a compact Lie group.}}
$$

This is the mechanism behind the assertion that [compact groups with a descending chain condition are Lie groups](../../../../../../compact-groups-with-a-descending-chain-condition-are-lie-groups.md): the chain condition turns an arbitrarily large separating family into one finite-dimensional [faithful representation](../../../../../../faithful-representation.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
