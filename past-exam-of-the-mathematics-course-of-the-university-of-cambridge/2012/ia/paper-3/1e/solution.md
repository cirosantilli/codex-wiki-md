<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

For a [finite group](../../../../../finite-group.md) $G$ and a [subgroup](../../../../../subgroup.md) $H$, [Lagrange's theorem](../../../../../lagrange-s-theorem.md) states

$$
|G|=[G:H]|H|.
$$

In particular $|H|$ divides $|G|$: the left [cosets](../../../../../coset.md) partition $G$, and multiplication by a representative is a [bijection](../../../../../bijection.md) from $H$ to each [coset](../../../../../coset.md). Apply this to the [cyclic subgroup](../../../../../cyclic-subgroup.md) $\langle g\rangle$. Its size is the [order of a group element](../../../../../order-of-a-group-element.md) $g$, so **every element order divides $|G|$**.

Under the square condition, every [group](../../../../../group-split.md) element is its own [inverse element](../../../../../inverse-element.md). Consequently

$$
gh=(gh)^{-1}=h^{-1}g^{-1}=hg
$$

for all $g,h$. This proves that a [group of exponent two is abelian](../../../../../group-of-exponent-two-is-abelian.md), including the trivial [group](../../../../../group-split.md).

For the fourth-power condition a counterexample to commutativity is the [quaternion group](../../../../../quaternion-group.md)

$$
\boxed{Q_8=\{\pm1,\pm i,\pm j,\pm k\}.}
$$

Here $i^2=j^2=k^2=-1$ and $ij=k=-ji$. Thus its six elements outside $\{\pm1\}$ have [order of a group element](../../../../../order-of-a-group-element.md) four, while $1$ and $-1$ have orders one and two. All fourth powers are the identity, yet $ij\ne ji$.

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
