<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Work in the finite-group setting. If $M$ is maximal in a nonabelian simple $G$, then $M\ne1$: otherwise every nonidentity element would generate $G$, forcing a cyclic group of prime order. Choose a [minimal normal subgroup](../../../../../../minimal-normal-subgroup.md) $N\ne1$ of $M$. Every [characteristic subgroup](../../../../../../characteristic-subgroup.md) of $N$ is normal in $M$, so minimality makes $N$ a [characteristically simple group](../../../../../../characteristically-simple-group.md). Its [normalizer](../../../../../../normalizer.md) contains $M$. By maximality it is $M$ or $G$, and the latter would make $N$ a nontrivial [normal subgroup](../../../../../../normal-subgroup.md) of the [simple group](../../../../../../simple-group.md) $G$, impossible because $N\le M<G$. This proves the [maximal subgroup normalizer criterion](../../../../../../maximal-subgroup-normalizer-criterion.md):

$$
\boxed{M=N_G(N)\text{ for some characteristically simple }N.}
$$

For $A_5$, [stabilizer subgroups](../../../../../../stabilizer-subgroup.md) have order 12. [Stabilizer subgroups](../../../../../../stabilizer-subgroup.md) of a two-element subset have order $|(S_2\times S_3)\cap A_5|=6$, and are isomorphic to $S_3$; for example $\langle(1\,2\,3),(1\,2)(4\,5)\rangle$. The [normalizer](../../../../../../normalizer.md) of a Sylow 5-subgroup has order 10: its [normalizer](../../../../../../normalizer.md) in $S_5$ has order $5\cdot4$, and exactly half its [permutations](../../../../../../permutation.md) are even, since a multiplier of order four on $\mathbb F_5$ is an odd four-cycle. This gives a [dihedral group](../../../../../../dihedral-group.md) of order 10.

To prove completeness, an intransitive [subgroup](../../../../../../subgroup.md) either fixes a point, or its orbits on five letters have sizes two and three. It therefore lies in one of the first two types. A transitive proper [subgroup](../../../../../../subgroup.md) $H$ has order divisible by 5. Its number of Sylow 5-subgroups is one or six, since $A_5$ has six and the count is $1$ modulo 5. A count of six would make $30\mid |H|$, forcing an index-two [subgroup](../../../../../../subgroup.md) and contradicting [Simplicity of the alternating group A5](../../../../../../simplicity-of-the-alternating-group-a5.md). Therefore $H$ normalizes its unique Sylow 5-subgroup and lies in the order-ten [normalizer](../../../../../../normalizer.md).

[Stabilizer subgroups](../../../../../../stabilizer-subgroup.md) are maximal because their index is prime. The order-ten group is transitive and cannot have a larger proper transitive overgroup by the preceding argument. The order-six group has no fixed point, cannot lie in a [stabilizer subgroup](../../../../../../stabilizer-subgroup.md), and cannot lie in the order-ten type because 3 does not divide 10. Thus all three types are maximal. $A_5$ is transitive on points and on unordered pairs, while Sylow conjugacy handles the [normalizers](../../../../../../normalizer.md). Consequently

$$
\boxed{A_5:\text{ three maximal-subgroup classes, of orders }6,\ 10,\ 12.}
$$

Now let $G=GL_3(2)$. Choosing independent columns gives $|G|=7\cdot6\cdot4=168$. Its simplicity follows from the elementary projective-transvection proof in part 4(i), which does not use this [subgroup](../../../../../../subgroup.md) classification.

A [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) and a plane [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) each have index seven and order 24. To construct the remaining type, identify $\mathbb F_2^3$ with $\mathbb F_8$ and take the [Singer cycle](../../../../../../singer-cycle.md) $P$ of multiplications by nonzero field elements, of order seven. Any [linear map](../../../../../../linear-map.md) commuting with a primitive multiplication commutes with all of $\mathbb F_8$, so its [centralizer](../../../../../../centralizer.md) is precisely $P$. A [normalizer](../../../../../../normalizer.md) sends a primitive element $a$ to another root of its minimum polynomial, namely $a,a^2,a^4$. The Frobenius map $x\mapsto x^2$ realizes those three choices. Hence

$$
N_G(P)=P\rtimes C_3,\qquad |N_G(P)|=21,\qquad n_7(G)=8.
$$

If $7\mid |H|$ for a proper $H<G$, its Sylow count is one or eight. Eight would make $56\mid|H|$, hence $|H|=56$. Its index-three [coset](../../../../../../coset.md) action would inject the [simple group](../../../../../../simple-group.md) $G$ into $S_3$: the kernel is normal and cannot be all of $G$. This is impossible. Thus $H$ normalizes a unique Sylow 7-subgroup and lies in the order-21 [normalizer](../../../../../../normalizer.md).

If $7\nmid |H|$, its order divides 24. In its action on seven nonzero [vectors](../../../../../../vector.md), an odd orbit has size one or three. A one-point orbit gives a fixed point. If a three-point orbit is collinear, it is the set of nonzero [vectors](../../../../../../vector.md) of an invariant plane. If its three [vectors](../../../../../../vector.md) are independent, their nonzero sum is fixed by $H$. Thus $H$ lies in a point or plane [stabilizer subgroup](../../../../../../stabilizer-subgroup.md).

The index-seven [stabilizer subgroups](../../../../../../stabilizer-subgroup.md) are maximal, and any proper overgroup of the order-21 [normalizer](../../../../../../normalizer.md) would again have a unique Sylow 7-subgroup and normalize that same [subgroup](../../../../../../subgroup.md), so the [normalizer](../../../../../../normalizer.md) is maximal too. The point and plane [stabilizer subgroups](../../../../../../stabilizer-subgroup.md) are not conjugate: a [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) fixes a point, whereas a plane [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) is transitive on its three internal points and its four external points, so fixes no point. Each type is one [conjugacy class](../../../../../../conjugacy-class.md). We have proved [maximal subgroups of GL3 over F2](../../../../../../maximal-subgroups-of-gl3-over-f2.md):

$$
\boxed{GL_3(2):\text{ three classes, of orders }21,\ 24,\ 24.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
