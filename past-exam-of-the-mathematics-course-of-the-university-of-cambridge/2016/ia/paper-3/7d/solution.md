<h1 id="7d/solution">Solution</h1>

↑ **Parent:** [7D](../7d.md)

For a [group action](../../../../../group-action.md) of a [finite group](../../../../../finite-group.md) $G$ on a set and a point $x$, the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) is

$$
\boxed{|Gx|=[G:G_x],\qquad |G|=|G_x||Gx|,}
$$

where $G_x=\{g:gx=x\}$ is the [stabilizer subgroup](../../../../../stabilizer-subgroup.md). The map $gG_x\mapsto gx$ is well defined because elements of the same [coset](../../../../../coset.md) act identically on $x$. If $gx=hx$, then $h^{-1}g\in G_x$, so their [cosets](../../../../../coset.md) agree; every orbit point has the form $gx$, giving surjectivity. This is a [bijection](../../../../../bijection.md). [Lagrange's theorem](../../../../../lagrange-s-theorem.md), $|G|=[G:H]|H|$ for any [subgroup](../../../../../subgroup.md) $H$, yields the counting formula.

Apply the [conjugation action](../../../../../conjugation-action.md) of the [finite p-group](../../../../../finite-p-group.md) $G$ to its nontrivial [normal subgroup](../../../../../normal-subgroup.md) $N$. Normality ensures the action stays inside $N$. The singleton [orbits of a group action](../../../../../orbit-of-a-group-action.md) are exactly the elements of $N\cap Z(G)$. Every larger [orbit of a group action](../../../../../orbit-of-a-group-action.md) has size a positive power of $p$, by the [orbit-stabilizer theorem](../../../../../orbit-stabilizer-theorem.md) and [Lagrange's theorem](../../../../../lagrange-s-theorem.md). Therefore

$$
|N|\equiv |N\cap Z(G)|\pmod p.
$$

Since $N$ is nontrivial, its order is divisible by $p$. The intersection contains the identity and has cardinality a positive multiple of $p$, so it contains a nonidentity element. This proves the [central intersection property of normal subgroups of finite p-groups](../../../../../central-intersection-property-of-normal-subgroups-of-finite-p-groups.md).

For the proper [subgroup](../../../../../subgroup.md) $H$, let $H$ act by left multiplication on the left [cosets](../../../../../coset.md) $G/H$. A [coset](../../../../../coset.md) $gH$ is fixed by every $h\in H$ exactly when $g^{-1}Hg\subseteq H$. Both groups have the same finite size, so this inclusion is equality; the fixed [cosets](../../../../../coset.md) are precisely those with $g\in N_G(H)$. Hence their number is $[N_G(H):H]$. All non-singleton [orbits of a group action](../../../../../orbit-of-a-group-action.md) have size divisible by $p$, so

$$
[G:H]\equiv[N_G(H):H]\pmod p.
$$

Since $H$ is proper, $[G:H]$ is a positive power of $p$ greater than one. The fixed-coset count is nonzero, because $H$ itself is fixed, and is divisible by $p$. Therefore **the [normalizer](../../../../../normalizer.md) strictly contains $H$**:

$$
\boxed{[N_G(H):H]\geq p,\qquad\exists g\in G\setminus H:\ g^{-1}Hg=H.}
$$

This is the [normalizer condition for finite p-groups](../../../../../normalizer-condition-for-finite-p-groups.md). The proof also covers $H=\{1\}$, whose action fixes all [cosets](../../../../../coset.md).

## ↑ Ancestors (10)

1. [7D](../7d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
