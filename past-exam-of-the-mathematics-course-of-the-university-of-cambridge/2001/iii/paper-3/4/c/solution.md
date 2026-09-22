<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose $\alpha\in\Omega$ and identify $\Omega$ with $N$ by $n\mapsto n\alpha$. Normality means that the [point stabilizer](../../../../../../stabilizer-subgroup.md) $H_\alpha$ acts on $N$ by conjugation, and

$$
h(n\alpha)=(hnh^{-1})\alpha\qquad(h\in H_\alpha).
$$

Double transitivity therefore says that $H_\alpha$ is transitive on $N\setminus\{1\}$. All nonidentity elements of $N$ have the same order. By [Cauchy's theorem for finite groups](../../../../../../cauchy-theorem-for-groups.md), some element has order a prime $p$ dividing $|N|$, so that common order is $p$. Cauchy's theorem excludes every other prime from $|N|$, hence $N$ is a finite p-group.

By the center argument from Q1, $Z(N)\ne1$. The center is characteristic in $N$ and therefore invariant under the conjugation action of $H_\alpha$. Its nonidentity elements form a nonempty invariant subset of the transitive set $N\setminus\{1\}$, so $Z(N)=N$. Thus $N$ is abelian of exponent $p$:

$$
\boxed{N\cong(\mathbb F_p^d,+)\quad\text{for some }d\geq1.}
$$

This is [elementary abelian regular kernels in doubly transitive groups](../../../../../../elementary-abelian-regular-kernels-in-doubly-transitive-groups.md); knowing only that all element orders agree would not by itself prove commutativity.

Every $h\in H$ is uniquely $nh_0$ with $n\in N$ and $h_0\in H_\alpha$, because regularity supplies the unique $n$ sending $\alpha$ to $h\alpha$. Hence $H=N\rtimes H_\alpha$. The conjugation action of $H_\alpha$ on $N$ is faithful: an element centralizing $N$ and fixing $\alpha$ fixes every $n\alpha$, and is the identity [permutation](../../../../../../permutation.md). [Group automorphisms](../../../../../../group-automorphism.md) of an elementary abelian p-group are exactly invertible $\mathbb F_p$-linear maps, so $H_\alpha\leq GL(d,p)$. Choosing a vector-space [basis](../../../../../../basis.md) therefore gives

$$
\boxed{H\hookrightarrow\mathbb F_p^d\rtimes GL(d,p)=AGL(d,p).}
$$

Under this embedding, $N$ is the translation [subgroup](../../../../../../subgroup.md) and the [point stabilizer](../../../../../../stabilizer-subgroup.md) is a linear [subgroup](../../../../../../subgroup.md) transitive on nonzero [vectors](../../../../../../vector.md). The action is assumed to have at least two points, as usual for a doubly transitive [group](../../../../../../group-split.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
