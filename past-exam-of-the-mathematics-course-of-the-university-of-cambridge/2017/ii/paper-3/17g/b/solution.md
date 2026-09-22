<h1 id="17g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Conjugation](../../../../../../conjugation.md) by $P$ partitions $H$ into [orbits](../../../../../../orbit-dynamical-system.md). Each non-singleton [orbit](../../../../../../orbit-dynamical-system.md) has size divisible by $p$, by the [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md). The singleton [orbits](../../../../../../orbit-dynamical-system.md) are exactly $H\cap Z(P)$. Since $|H|$ is divisible by $p$, $|H\cap Z(P)|\equiv0\pmod p$. This [set](../../../../../../set-split.md) contains $1$, so $\boxed{|H\cap Z(P)|\geq p}$.

For the deduction we also give the representation-theoretic ingredient behind [Burnside's theorem](../../../../../../burnside-s-theorem.md): a nonabelian finite [simple group](../../../../../../simple-group.md) has no nontrivial [conjugacy class](../../../../../../conjugacy-class.md) of [prime power](../../../../../../prime-power.md) size. Here is a proof, so no stronger theorem is being assumed without justification. Suppose $g\ne1$ has class size $p^b$. For an [irreducible character](../../../../../../irreducible-character.md) $\chi$ of degree $d$ coprime to $p$, the [class sum](../../../../../../conjugacy-class-sum.md) acts as the scalar $p^b\chi(g)/d$, which is an [algebraic integer](../../../../../../algebraic-integer.md): the [class sum](../../../../../../conjugacy-class-sum.md) has an integer-entry [matrix](../../../../../../matrix.md) in the [regular representation](../../../../../../regular-representation.md), which contains every [irreducible representation](../../../../../../irreducible-representation.md), so this scalar is an eigenvalue of an integer-entry matrix. Also $\chi(g)$ is an [algebraic integer](../../../../../../algebraic-integer.md). Bezout's identity then makes $\chi(g)/d$ an [algebraic integer](../../../../../../algebraic-integer.md). All its [algebraic conjugates](../../../../../../conjugate-element-field-theory.md) have modulus at most $1$, because [character values of a representation](../../../../../../character-value-of-a-representation.md) are sums of $d$ [roots of unity](../../../../../../root-of-unity.md). An [algebraic integer](../../../../../../algebraic-integer.md) with this property is zero or a [root of unity](../../../../../../root-of-unity.md): the monic [polynomials](../../../../../../polynomial-split.md) of all its powers have uniformly bounded [integer](../../../../../../integer.md) coefficients, so two powers must coincide unless it is zero.

Every nontrivial [irreducible representation](../../../../../../irreducible-representation.md) of a [simple group](../../../../../../simple-group.md) is faithful. If $\chi(g)/d$ were a [root of unity](../../../../../../root-of-unity.md), equality in the triangle inequality would force its representing [matrix](../../../../../../matrix.md) to be scalar, hence $g$ central, impossible. Thus $\chi(g)=0$ whenever $p\nmid d$, except for the trivial [character of a representation](../../../../../../character-of-a-representation.md). Orthogonality of the identity column and the $g$ column in the [character table](../../../../../../character-table.md) now gives

$$
 0=1+\sum_{p\mid\chi(1)}\chi(1)\overline{\chi(g)}.
$$

This would make $1/p$ an [algebraic integer](../../../../../../algebraic-integer.md), contradicting the fact that rational [algebraic integers](../../../../../../algebraic-integer.md) are [integers](../../../../../../integer.md). The same proof covers class size $1$ directly through triviality of the center.

If an abelian [subgroup](../../../../../../subgroup.md) $A$ had index $p^a$, every $g\in A\setminus\{1\}$ would have $A\subseteq C_G(g)$, making its class size a [divisor](../../../../../../divisor.md) of $p^a$, a contradiction. Such a $g$ exists: if $A=1$, then $G$ is a nontrivial [p-group](../../../../../../p-group.md), whose center is nontrivial by the first argument with $H=P$. Therefore **a nonabelian [simple group](../../../../../../simple-group.md) has no abelian [subgroup](../../../../../../subgroup.md) of [prime power](../../../../../../prime-power.md) index**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17G](../../17g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
