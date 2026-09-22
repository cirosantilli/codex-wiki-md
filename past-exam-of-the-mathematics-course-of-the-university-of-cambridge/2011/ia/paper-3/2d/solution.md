<h1 id="2d/solution">Solution</h1>

↑ **Parent:** [2D](../2d.md)

[Lagrange's theorem](../../../../../lagrange-s-theorem.md) says that for a [finite group](../../../../../finite-group.md) $G$ and a [subgroup](../../../../../subgroup.md) $H$,

$$
|G|=[G:H]|H|.
$$

In particular, $|H|$ divides $|G|$. To prove it, consider the left [cosets](../../../../../coset.md) $gH$. Every element lies in one, and if $gH$ and $g'H$ intersect, then $gh=g'h'$ for some $h,h'\in H$. Hence $g=g'h'h^{-1}$ and $gH=g'H$. Distinct [cosets](../../../../../coset.md) are therefore disjoint and partition $G$. Multiplication by $g$ is a [bijection](../../../../../bijection.md) $H\to gH$, so every [coset](../../../../../coset.md) has $|H|$ elements. Counting this partition proves the formula.

Write the [dihedral group](../../../../../dihedral-group.md) as

$$
D_{2n}=\langle r,s:r^n=s^2=e,\ srs=r^{-1}\rangle,
$$

where $r$ is a rotation and $s$ a reflection. If $k\mid n$, the [cyclic subgroup](../../../../../cyclic-subgroup.md) $\langle r^{n/k}\rangle$ has order $k$. If $k\mid2n$ but $k\nmid n$, then $k$ is even: an odd divisor of $2n$ would divide $n$. Put $m=k/2$, so $m\mid n$. The [subgroup](../../../../../subgroup.md)

$$
\boxed{\langle r^{n/m},s\rangle}
$$

contains exactly the $m$ rotations $r^{jn/m}$ and the $m$ reflections $r^{jn/m}s$, for $0\leq j<m$. The inversion relation makes this set closed under multiplication and inverses. These $2m=k$ elements are distinct, so it has the required order. This proves the [dihedral subgroups of every divisor order](../../../../../dihedral-subgroups-of-every-divisor-order.md) property. The construction works for every even divisor, including those already covered by the cyclic construction.

## ↑ Ancestors (10)

1. [2D](../2d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
