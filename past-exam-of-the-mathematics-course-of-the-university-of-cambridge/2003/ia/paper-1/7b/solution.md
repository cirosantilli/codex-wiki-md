<h1 id="7b/solution">Solution</h1>

↑ **Parent:** [7B](../7b.md)

There are nontrivial proper [normal subgroups](../../../../../normal-subgroup.md). The [determinant](../../../../../determinant.md) defines a surjective [group homomorphism](../../../../../group-homomorphism.md) $G\to\{1,-1\}$. Its kernel is the [rotational symmetry group of a cube](../../../../../rotational-symmetry-group-of-a-cube.md), a normal subgroup of order twenty-four. Also $\{I,-I\}$ is a central subgroup of order two: central inversion preserves the cube and commutes with every matrix. Both provide affirmative examples.

For the body diagonal through $(1,1,1)$, write a general cube symmetry as $D_\varepsilon P$, with $P$ a [permutation matrix](../../../../../permutation-matrix.md) and $D_\varepsilon=\operatorname{diag}(\varepsilon_1,\varepsilon_2,\varepsilon_3)$, each $\varepsilon_j=\pm1$. Since $P(1,1,1)^T=(1,1,1)^T$, preserving the unoriented diagonal requires $(\varepsilon_1,\varepsilon_2,\varepsilon_3)$ to be either $(1,1,1)$ or $(-1,-1,-1)$. Thus

$$
H=\{\varepsilon P:\varepsilon\in\{1,-1\},\ P\text{ a }3\times3\text{ permutation matrix}\}.
$$

The map $(\pi,\varepsilon)\mapsto\varepsilon P_\pi$ from $S_3\times C_2$ to $H$ is a [group homomorphism](../../../../../group-homomorphism.md), because central inversion commutes with every coordinate permutation. It is surjective by the displayed description and injective because a permutation matrix cannot equal the negative of another permutation matrix. Consequently the [body-diagonal stabilizer in the cube symmetry group](../../../../../body-diagonal-stabilizer-in-the-cube-symmetry-group.md) is

$$
\boxed{H\cong S_3\times C_2,\qquad |H|=12.}
$$

This also agrees with the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) for the transitive action on the four body diagonals. The line is preserved as a set, so exchanging its opposite endpoints is allowed.

## ↑ Ancestors (10)

1. [7B](../7b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
