<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Brauer morphism](../../../../../brauer-morphism.md) retains precisely the fixed group-basis elements under conjugation by $D$:

$$
\operatorname{Br}_D\left(\sum_{g\in G}a_gg\right)=\sum_{g\in C_G(D)}a_gg,\qquad a\in(kG)^D.
$$

It is unital and surjective because $kC_G(D)\subseteq(kG)^D$. For multiplicativity, fix $x\in C_G(D)$. Its coefficient in a product is $\sum_{gh=x}a_gb_h$. Conjugation by $D$ permutes these pairs and the summand is constant on each orbit. Nonsingleton orbits have p-divisible size and contribute zero. Singleton pairs have both entries in $C_G(D)$, so they give exactly the coefficient in $\operatorname{Br}_D(a)\operatorname{Br}_D(b)$. This proves the ring-homomorphism assertion.

Orbit sums form a basis of $(kG)^D$. A nonfixed orbit sum of $g$ is $\operatorname{Tr}_{C_D(g)}^D(g)$, a proper-subgroup [relative trace](../../../../../relative-trace.md). Conversely any proper-subgroup trace has zero coefficient on a fixed basis element, since that coefficient is multiplied by $[D:Q]=0$ in $k$. Thus

$$
\boxed{\ker\operatorname{Br}_D=\sum_{Q<D}\operatorname{Tr}_Q^D((kG)^Q).}
$$

There is no assertion that this whole kernel is nilpotent.

[Brauer first main theorem](../../../../../brauer-first-main-theorem.md) bijects the [modular blocks](../../../../../block-of-a-group-algebra.md) of $kG$ with defect $D$ and those of $kN_G(D)$ with defect $D$, matching their nonzero Brauer images. Here is a proof with its auxiliary ingredients.

Write $N=N_G(D)$, $C=C_G(D)$ and define

$$
I_D(G)=\operatorname{Tr}_D^G((kG)^D)\subseteq Z(kG),\qquad
J_D=\operatorname{Tr}_D^N(kC)\subseteq(kC)^N.
$$

These are ideals in the indicated commutative algebras, since an invariant multiplier passes through a [relative trace](../../../../../relative-trace.md). The [Brauer morphism and relative trace](../../../../../brauer-morphism-and-relative-trace.md) identity

$$
\operatorname{Br}_D\operatorname{Tr}_D^G(a)=\operatorname{Tr}_D^N\operatorname{Br}_D(a)
$$

follows by letting $D$ act on $G/D$. Fixed [cosets](../../../../../coset.md) have representatives in $N$; projection onto $C$ gives equal contributions on each other orbit, whose p-divisible size makes the contribution zero. Thus $\operatorname{Br}_D$ surjects $I_D(G)$ onto $J_D$.

To prove the [trace criterion for defect groups](../../../../../trace-criterion-for-defect-groups.md), choose a [p-subgroup](../../../../../p-subgroup.md) $E$ of least order with a given block idempotent $b$ in $I_E(G)$. Such a choice exists because a Sylow $P$ gives $b=\operatorname{Tr}_P^G(b/[G:P])$. Write $b=\operatorname{Tr}_E^G(a)$ and replace $a$ by $ba$. If $\operatorname{Br}_E(b)=0$, the kernel formula and trace transitivity give $b\in\sum_{Q<E}I_Q(G)$. But $bZ(kG)$ is an [Artinian local ring](../../../../../artinian-local-ring.md), and a finite sum of proper ideals cannot contain its identity. Multiplication by $b$ therefore forces $b\in I_Q(G)$ for some smaller $Q$, a contradiction. Hence $\operatorname{Br}_E(b)\ne0$.

If $F$ is not conjugate into $E$, its action on $G/E$ has no fixed [coset](../../../../../coset.md) and the same orbit argument gives $\operatorname{Br}_F(I_E(G))=0$. Every subgroup with nonzero Brauer image of $b$ is therefore conjugate into $E$. Its maximal such subgroups are exactly the conjugates of $E$, proving the definition's conjugacy assertion and

$$
b\in I_D(G)\ \Longleftrightarrow\ \text{a defect group of }b\text{ is conjugate into }D.
$$

Among block idempotents in this ideal, the Brauer image at $D$ survives precisely when their defect is $D$.

We also use [primitive idempotents under a surjection of commutative Artinian ideals](../../../../../primitive-idempotents-under-a-surjection-of-commutative-artinian-ideals.md). Decompose the ambient algebras into local factors. The component of an ideal in a local factor is either the whole factor, possessing its identity, or a proper ideal in its nilpotent radical, possessing no nonzero idempotent. A nonzero quotient of a local algebra is local. A surjection of these ideals consequently bijects its surviving primitive idempotents with those of the target. Entire factors may be killed; the whole kernel need not be nilpotent.

Apply this result to $I_D(G)\to J_D$. Its surviving primitive idempotents are exactly the [modular blocks](../../../../../block-of-a-group-algebra.md) of $G$ with defect $D$. Apply it also to $I_D(N)\to J_D$, where the target is identical since $N_N(D)=N$ and $C_N(D)=C$. Its surviving primitive idempotents are exactly the [modular blocks](../../../../../block-of-a-group-algebra.md) of $N$ with defect $D$. Matching images in $J_D$ proves **[Brauer first main theorem](../../../../../brauer-first-main-theorem.md)**, in both directions and with uniqueness.

For the last construction, the intended hypothesis is that **$D$ is a [defect group](../../../../../defect-group-of-a-block.md) of the source [modular block](../../../../../block-of-a-group-algebra.md) $b$**. Put $L=N_H(D)$ and use the theorem inside $H$ to obtain the corresponding [modular block](../../../../../block-of-a-group-algebra.md) $c$ of $kL$. The [centralizer](../../../../../centralizer.md) condition gives $C_H(D)=C_G(D)$, so $\operatorname{Br}_D$ maps $Z(kG)$ into $Z(kL)$. Let $\omega_c:Z(kL)\to F_c$ be the [central character of a block](../../../../../central-character-of-a-block.md), retaining its residue field $F_c$ rather than assuming it equals $k$. The unital composite

$$
Z(kG)\xrightarrow{\operatorname{Br}_D}Z(kL)\xrightarrow{\omega_c}F_c
$$

sends exactly one global block idempotent to one, because their orthogonal idempotent images sum to one in a field. **Define $b^G$ to be this unique [modular block](../../../../../block-of-a-group-algebra.md).** This is [block induction](../../../../../block-induction.md), independent of the chosen $H$-conjugate of $D$. It needs no containment of $N_G(D)$ in $H$, and its defect may be larger than $D$. With that containment it agrees with the first-main-theorem correspondence.

The printed PDF does not require $D$ to be a [defect group](../../../../../defect-group-of-a-block.md) of $b$. Its literal conditions do not always define the usual induced [modular block](../../../../../block-of-a-group-algebra.md). For example, over an algebraically closed field of characteristic three, take $G=A_5$, $H=A_4$ as a point stabilizer, and $D=\langle(123)\rangle$. Then $DC_G(D)=D\leq H$. The ordinary degree-three irreducible of $A_4$ gives a defect-zero [modular block](../../../../../block-of-a-group-algebra.md) $b$ on reduction. The two distinct ordinary degree-three irreducibles of $A_5$ give distinct defect-zero [modular blocks](../../../../../block-of-a-group-algebra.md) $B_+$ and $B_-$. Both restrict to that same character of $A_4$, with values $3,-1,0$ on its identity, double transpositions and three-cycles.

The standard defect-zero lifting theorem says that these reductions are simple [projective modules](../../../../../projective-module.md) and their block algebras are full matrix algebras. Thus both [module restrictions](../../../../../restriction-of-a-representation.md) $B_+\downarrow_{H\times H}$ and $B_-\downarrow_{H\times H}$ contain the same [modular block](../../../../../block-of-a-group-algebra.md) [bimodule](../../../../../bimodule.md) $b$; indeed each [module restriction](../../../../../restriction-of-a-representation.md) is isomorphic to it here. The actual defect of $b$ is 1, whose [centralizer](../../../../../centralizer.md) is $G$, not a subgroup of $H$. The unrelated subgroup $D=C_3$ cannot select between the two [modular blocks](../../../../../block-of-a-group-algebra.md). This is [block induction requires the block's defect centralizer](../../../../../block-induction-requires-the-block-s-defect-centralizer.md); the qualified construction above answers the intended request.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
