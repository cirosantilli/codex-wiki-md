<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For a set of primes $\pi$, a Hall $\pi$-subgroup $H$ of a [finite group](../../../../../finite-group.md) is a subgroup whose order uses only primes in $\pi$ and whose [subgroup index](../../../../../index-of-a-subgroup.md) uses only primes outside $\pi$. Equivalently, $|H|$ is the full $\pi$-part of $|G|$. A [Hall subgroup](../../../../../hall-subgroup.md) is a Hall $\pi$-subgroup for some $\pi$. The theorem of P. Hall for finite [soluble groups](../../../../../solvable-group.md) states: Hall $\pi$-subgroups exist for every $\pi$, any two are conjugate, and every $\pi$-subgroup is contained in a Hall $\pi$-subgroup.

For the existence proof, first give the explicit coprime splitting calculation needed in the induction. Let $N$ be elementary abelian of [field characteristic](../../../../../characteristic-of-a-field.md) $r$, normal in $E$, with $r\nmid|E/N|$. Write $Q=E/N$ and use additive notation on $N$. A normalized section $s:Q\to E$ gives an action $x\cdot n=s(x)ns(x)^{-1}$ independent of its choice, since $N$ is abelian. Write $s(x)s(y)=f(x,y)s(xy)$. Associativity gives

$$
f(x,y)+f(xy,z)=x\cdot f(y,z)+f(x,yz).
$$

Sum over $z\in Q$, put $S(x)=\sum_z f(x,z)$, and divide by $|Q|$ in the [vector space](../../../../../vector-space-split.md) $N$. This is legitimate because $r\nmid|Q|$. With $b(x)=|Q|^{-1}S(x)$ one obtains

$$
f(x,y)=b(x)+x\cdot b(y)-b(xy).
$$

The new section $s'(x)=(-b(x))s(x)$ therefore has zero multiplication defect and is a [group homomorphism](../../../../../group-homomorphism.md). Its image is a complement to $N$.

We will also need a single [conjugation](../../../../../conjugation.md) carrying one complement to the other. If two homomorphic sections differ by $d(x)$, their difference satisfies $d(xy)=d(x)+x\cdot d(y)$. Summing over $y$ gives $d(x)=c-x\cdot c$, where $c=|Q|^{-1}\sum_y d(y)$. Thus the second section is $c\,s(x)c^{-1}$. This proves, by explicit averaging, both [coprime splitting over an elementary abelian normal subgroup](../../../../../coprime-splitting-over-an-elementary-abelian-normal-subgroup.md) and the existence of such a [conjugation](../../../../../conjugation.md) by an element of $N$.

Now induct on $|G|$ for [Hall subgroup existence in soluble groups](../../../../../hall-subgroup-existence-in-soluble-groups.md). A [minimal normal subgroup](../../../../../minimal-normal-subgroup.md) $N$ of a finite [soluble group](../../../../../solvable-group.md) is elementary abelian of some [field characteristic](../../../../../characteristic-of-a-field.md) $r$. Indeed, $N'$ is a [characteristic subgroup](../../../../../characteristic-subgroup.md) of $N$ and normal in $G$; it cannot equal $N$ because $N$ is soluble, so it is trivial. In this [abelian group](../../../../../abelian-group.md), a nontrivial primary component is a [characteristic subgroup](../../../../../characteristic-subgroup.md), forcing a single prime, and the [characteristic subgroup](../../../../../characteristic-subgroup.md) annihilated by that prime forces exponent $r$.

By induction $G/N$ has a Hall $\pi$-subgroup $\overline H$, with preimage $M$. If $M<G$, induction in $M$ supplies a Hall $\pi$-subgroup of $M$, which is also Hall in $G$ because $[G:M]$ is prime to all primes in $\pi$. If $M=G$, the quotient is a $\pi$-group. When $r\in\pi$, $G$ itself is a $\pi$-group. When $r\notin\pi$, the averaging construction splits off $N$, and its complement has order $|G/N|$ and is the required Hall $\pi$-subgroup. This completes the existence proof, including the identity group and empty prime set.

A [Sylow basis](../../../../../sylow-basis.md) is a family $\{P_p:p\mid|G|\}$ containing one [Sylow subgroup](../../../../../sylow-subgroup.md) for each prime, with $P_pP_q=P_qP_p$ for each pair. This is permutability of subgroups, not commutation of all their elements. The product of any subfamily is a subgroup: commuting the factors as sets proves closure and closure under inversion. Inductively its order is the product of the prime-power orders, since the newly adjoined factor has trivial intersection with the earlier product. It is thus the corresponding [Hall subgroup](../../../../../hall-subgroup.md).

Prove existence of a [Sylow basis](../../../../../sylow-basis.md) by induction on $|G|$, again using elementary abelian $N$ of [field characteristic](../../../../../characteristic-of-a-field.md) $r$. Choose a basis $\{\overline P_p\}$ of $G/N$, taking $\overline P_r=1$ if $r$ does not divide that quotient's order. The product $\overline H=\prod_{p\ne r}\overline P_p$ is its Hall $r'$-subgroup. In its full preimage $T$, the averaging lemma supplies a complement $H$ to $N$, mapping isomorphically to $\overline H$. For $p\ne r$, let $P_p$ be the inverse image of $\overline P_p$ under this isomorphism within $H$. Let $P_r$ be the full preimage of $\overline P_r$ in $G$. These are [Sylow subgroups](../../../../../sylow-subgroup.md) of $G$. The other-prime pairs permute because they do so in $\overline H$. For $P_r$ and $P_p$, their product is contained in the full preimage of the subgroup $\overline P_r\overline P_p$ and has exactly that preimage's order $|N|\,|\overline P_r|\,|\overline P_p|$. Equality follows, so the product is a subgroup and these two factors permute as well. This constructs a basis.

To obtain a simultaneous [conjugation](../../../../../conjugation.md) of two bases, take two bases. Their images in $G/N$ are bases: $N$ lies in every Sylow $r$-subgroup, and the other-prime [Sylow subgroups](../../../../../sylow-subgroup.md) project injectively. By induction, conjugate one basis so that all corresponding images agree. The products of their non-$r$ factors are then two complements to $N$ in the same preimage $T$ of their common Hall $r'$-subgroup. The averaging lemma for complements supplies a single element of $N$ conjugating these complements. In the resulting common complement each corresponding [Sylow subgroup](../../../../../sylow-subgroup.md) is the unique lift of its agreed quotient subgroup, so all non-$r$ factors agree. The $r$-factors already equal the full preimage of their common quotient factor and are preserved by [conjugation](../../../../../conjugation.md) from $N$. Thus **all [Sylow bases](../../../../../sylow-basis.md) of a finite [soluble group](../../../../../solvable-group.md) are conjugate**.

In $S_4$ there are three Sylow $2$-subgroups of order eight: the action on the three pair-partitions of four points has kernel $V_4$, and these subgroups are the preimages of the three order-two subgroups of $S_3$. There are four Sylow $3$-subgroups, one for each three-point support. Every choice $P_2,P_3$ has trivial intersection and product of cardinality $8\cdot3=24$, so $P_2P_3=S_4=P_3P_2$. Therefore

$$
\boxed{b(S_4)=3\cdot4=12.}
$$

For $E=V\rtimes S_4$, $V=\mathbb F_5^4$, the Sylow $5$-subgroup is uniquely $V$. In a [Sylow basis](../../../../../sylow-basis.md) the product $P_2P_3$ is a Hall $5'$-subgroup, hence a complement to $V$. Conversely, a basis of any complement together with $V$ is a basis of $E$, because $V$ is normal. The averaging lemma makes all complements conjugate by $V$. The [stabilizer](../../../../../stabilizer-subgroup.md) of the standard complement $S_4$ under this [conjugation](../../../../../conjugation.md) is $C_V(S_4)$: if a vector normalizes it, its [group commutator](../../../../../group-commutator.md) with each complement element lies in both $V$ and that complement, hence is trivial. The fixed vectors under the natural coordinate [permutation action](../../../../../group-action.md) are exactly $(a,a,a,a)$, so $|C_V(S_4)|=5$. There are consequently $5^4/5=125$ complements, and each has twelve bases. The complement is uniquely recovered from its basis as $P_2P_3$, so no basis is counted twice. The [counting Sylow bases in a coprime elementary abelian extension](../../../../../counting-sylow-bases-in-a-coprime-elementary-abelian-extension.md) formula yields

$$
\boxed{b(5^4\rtimes S_4)=125\cdot12=1500.}
$$

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
