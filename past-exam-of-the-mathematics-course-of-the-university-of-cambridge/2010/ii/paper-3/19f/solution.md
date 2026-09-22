<h1 id="19f/solution">Solution</h1>

↑ **Parent:** [19F](../19f.md)

We use the standard facts that finite [complex representations](../../../../../complex-representation.md) are completely reducible, [irreducible characters](../../../../../irreducible-character.md) are orthonormal, the regular character is $\sum_\chi\chi(1)\chi$, and the number of [irreducible characters](../../../../../irreducible-character.md) equals the number of conjugacy classes. We also use Schur's lemma, Sylow's theorem and the nontrivial center of a nontrivial finite $p$-group.

For an [irreducible character](../../../../../irreducible-character.md) $\chi$ of degree $d$, a [conjugacy-class sum](../../../../../conjugacy-class-sum.md) $z_C$ acts as the scalar $\lambda_C=|C|\chi(g)/d$ by Schur's lemma and taking [traces](../../../../../matrix-trace.md). This scalar is an [algebraic integer](../../../../../algebraic-integer.md): class sums form an [integral](../../../../../integral.md) basis of the center of the [integral](../../../../../integral.md) [group algebra](../../../../../group-algebra.md), their multiplication has [integer](../../../../../integer.md) structure constants, and multiplication by $z_C$ satisfies its monic [integer](../../../../../integer.md) characteristic [polynomial](../../../../../polynomial-split.md). That same [polynomial](../../../../../polynomial-split.md) annihilates its image in any [irreducible representation](../../../../../irreducible-representation.md). Character values are also [algebraic integers](../../../../../algebraic-integer.md), since they are sums of roots of unity. [Character orthogonality](../../../../../character-orthogonality.md) now gives

$$
\frac{|G|}{d}=\sum_C\frac{|C|\chi(g)}d\overline{\chi(g)}=\sum_C\lambda_C\overline{\chi(g)}.
$$

This is a rational [algebraic integer](../../../../../algebraic-integer.md), hence an [integer](../../../../../integer.md). Therefore **$\chi(1)$ divides $|G|$**.

The [Burnside's pa qb theorem](../../../../../burnside-s-theorem.md) states that every [finite group](../../../../../finite-group.md) of order $p^a q^b$ is soluble. We prove its character-theoretic ingredient. If a class has size $m$ coprime to $d$, [integers](../../../../../integer.md) $u,v$ with $ud+vm=1$ give

$$
\frac{\chi(g)}d=u\chi(g)+v\frac{m\chi(g)}d,
$$

an [algebraic integer](../../../../../algebraic-integer.md). Every [algebraic conjugate](../../../../../conjugate-element-field-theory.md) of this number is the average of $d$ roots of unity and has modulus at most one. If it is nonzero, its algebraic norm is a nonzero [integer](../../../../../integer.md) of absolute value at least one; since every factor has modulus at most one, all must have modulus one. In particular $|\chi(g)|=d$. Equality in the [triangle inequality](../../../../../triangle-inequality.md) for the unit-modulus [eigenvalues](../../../../../eigenvalue.md) implies that $\rho(g)$ is scalar. Thus **if $(m,d)=1$, either $\chi(g)=0$ or $\rho(g)$ is scalar**.

Suppose a [group](../../../../../group-split.md) of order $p^a q^b$ were nonabelian simple, with both [primes](../../../../../prime-number.md) present. Choose a nonidentity $g$ in the center of a Sylow $p$-subgroup. Its centralizer contains that [Sylow subgroup](../../../../../sylow-subgroup.md), so its class size is a power of $q$. Every nontrivial [irreducible representation](../../../../../irreducible-representation.md) is faithful by simplicity. If it sent $g$ to a scalar, faithfulness would make $g$ central in the [group](../../../../../group-split.md), impossible in a nonabelian simple [group](../../../../../group-split.md). The ingredient above therefore gives $\chi(g)=0$ for every nontrivial character with degree coprime to $q$. Evaluating the regular character at $g\ne1$ gives

$$
0=1+\sum_{q\mid\chi(1)}\chi(1)\chi(g),\qquad
\frac1q=-\sum_{q\mid\chi(1)}\frac{\chi(1)}q\chi(g).
$$

The right side is an [algebraic integer](../../../../../algebraic-integer.md), but $1/q$ is not, a contradiction. A [group](../../../../../group-split.md) of prime-power order cannot be nonabelian simple either, by its nontrivial center. Induct on the order: every nonsimple [group](../../../../../group-split.md) has a proper nontrivial [normal subgroup](../../../../../normal-subgroup.md), and that subgroup and the quotient have smaller orders with at most these two [prime](../../../../../prime-number.md) divisors. By induction both are soluble; their derived-series extensions make the original [group](../../../../../group-split.md) soluble. Simple [abelian groups](../../../../../abelian-group.md) have [prime](../../../../../prime-number.md) order and start the induction. This proves **Burnside's theorem**.

For the final divisibility, let $|G|=n$ be odd and let $k$ be its number of conjugacy classes. All irreducible degrees are odd by the divisibility just proved. We use the standard [Frobenius-Schur indicator](../../../../../frobenius-schur-indicator.md) theorem: $\nu(\chi)=n^{-1}\sum_g\chi(g^2)$ is zero precisely for an [irreducible character](../../../../../irreducible-character.md) not equal to its conjugate, and is $\pm1$ otherwise. Squaring is a bijection on an odd-order [group](../../../../../group-split.md): for each $g$, its unique square root is $g^{(n+1)/2}$, since every element order divides $n$. For every nontrivial [irreducible character](../../../../../irreducible-character.md), orthogonality to the trivial character consequently gives $\nu(\chi)=n^{-1}\sum_g\chi(g)=0$. The nontrivial characters therefore occur in distinct conjugate pairs of equal odd degree. Since an odd square is one modulo eight,

$$
n-k=\sum_\chi(\chi(1)^2-1)
$$

is a sum of pairs $2(d^2-1)$, each divisible by sixteen; the trivial character contributes zero. Hence

$$
\boxed{16\mid n-k.}
$$

## ↑ Ancestors (10)

1. [19F](../19f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
