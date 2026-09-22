<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Throughout, [modules](../../../../../module-mathematics.md) are finite-dimensional over $k$, or finitely generated $\mathcal O$-free lattices when the coefficient ring is $\mathcal O$. The [p-modular system](../../../../../p-modular-system.md) has a complete [discrete valuation ring](../../../../../discrete-valuation-ring.md) $\mathcal O$, maximal ideal $(\pi)$, fraction [field](../../../../../field.md) $K$ of characteristic zero and residue [field](../../../../../field.md) $k$ of characteristic $p$.

A [block of a group algebra](../../../../../block-of-a-group-algebra.md) is a nonzero, indecomposable two-sided ideal direct summand of $A=RG$. Equivalently it is $Ae$ for a primitive [central idempotent](../../../../../central-idempotent.md) $e$. To see the equivalence, suppose $A=B\oplus C$ as two-sided [ideals](../../../../../ideal.md) and write $1=e+f$ with $e\in B$, $f\in C$. Products between $B$ and $C$ vanish because they lie in their zero intersection. Thus $e$ is the identity on $B$, zero on $C$, and is a [central idempotent](../../../../../central-idempotent.md), with $B=Ae$. Conversely $A=Ae\oplus A(1-e)$. Splitting $Ae$ further is equivalent to splitting $e$ into orthogonal nonzero [central idempotents](../../../../../central-idempotent.md); indecomposability is exactly primitivity. If $1=\sum e_i$ is the block decomposition, $M=\bigoplus e_iM$. A nonzero [indecomposable module](../../../../../indecomposable-module.md) therefore belongs to exactly one [block of a group algebra](../../../../../block-of-a-group-algebra.md), namely the one with $e_iM=M$.

For [modular reduction of block idempotents](../../../../../modular-reduction-of-block-idempotents.md), the conjugacy class sums are an $R$-basis of $Z(RG)$. Hence $Z(\mathcal OG)/\pi Z(\mathcal OG)\cong Z(kG)$. In the complete commutative [algebra](../../../../../algebra-split.md) $Z(\mathcal OG)$, [idempotent lifting](../../../../../idempotent-lifting.md) gives a unique lift of each [idempotent](../../../../../idempotent.md) of $Z(kG)$; uniqueness follows because commuting idempotents congruent modulo the [Jacobson radical](../../../../../jacobson-radical.md) are equal. Orthogonal decompositions lift too, so primitivity is preserved. **Reduction gives a bijection between the integral and modular blocks.**

Here is a definition of [defect groups of a block](../../../../../defect-group-of-a-block.md) which also proves the required relative-projectivity assertion. Give $RG$ its conjugation action and, for $H\le G$, define the [relative trace](../../../../../relative-trace.md) and its [transfer ideal of conjugation-fixed elements](../../../../../transfer-ideal-of-conjugation-fixed-elements.md) by

$$
\operatorname{Tr}_H^G(a)=\sum_{g\in G/H}gag^{-1},\qquad a\in(RG)^H,\qquad I_H=\operatorname{Tr}_H^G((RG)^H)\subseteq Z(RG).
$$

A [defect group of a block](../../../../../defect-group-of-a-block.md) $RGe$ is a $p$-subgroup $D$ minimal with $e\in I_D$. Such a subgroup exists: for a [Sylow subgroup](../../../../../sylow-subgroup.md) $P$, $[G:P]$ is a unit in $R$ and $e=\operatorname{Tr}_P^G(e/[G:P])$. The [defect of a block](../../../../../defect-of-a-block.md) is $d$ where $|D|=p^d$.

For completeness, this definition is independent of a choice up to conjugacy. Multiplying two [relative traces](../../../../../relative-trace.md) and grouping the pairs of cosets by [double cosets](../../../../../double-coset.md) gives

$$
I_D I_E\subseteq\sum_{g\in D\backslash G/E}I_{D\cap{}^gE}.
$$

This identity follows by writing each pair of cosets as a simultaneous $G$-orbit; its stabilizer is $D\cap{}^gE$, and its contribution is a trace from that stabilizer. If $D,E$ are both minimal for $e$, then $e=e^2$ belongs to the displayed sum. The commutative block center $eZ(RG)$ is a [local ring](../../../../../local-ring.md): in the field case it is a commutative [Artinian ring](../../../../../artinian-ring.md) with no nontrivial [idempotents](../../../../../idempotent.md); in the integral case its reduction has this property and completeness detects units. A sum of proper ideals cannot contain its identity. Consequently $e\in I_{D\cap{}^gE}$ for some $g$, forcing $D={}^gE$ by minimality. The same argument with an arbitrary $E$ shows that $e\in I_E$ precisely when $E$ contains a conjugate of $D$. This is the [trace criterion for defect groups](../../../../../trace-criterion-for-defect-groups.md).

To relate this to the usual modular definition, the [Brauer morphism](../../../../../brauer-morphism.md) deletes the coefficients outside the [centralizer](../../../../../centralizer.md):

$$
\operatorname{Br}_P:(kG)^P\longrightarrow kC_G(P),\qquad\sum a_g g\longmapsto\sum_{g\in C_G(P)}a_g g.
$$

It is an [algebra homomorphism](../../../../../algebra-homomorphism-over-a-field.md): in the coefficient of an element centralizing $P$ in a product, $P$ acts on the contributing pairs; nonfixed orbits have size divisible by $p$, while fixed pairs have both entries in $C_G(P)$. Its kernel is the sum of proper-subgroup transfers, because the nonfixed conjugation orbit sums form a basis of that kernel. If $D$ is minimal for $e=\operatorname{Tr}_D^G(a)$ and $\operatorname{Br}_D(e)=0$, replace $a$ by $ea$. The kernel description gives $e\in\sum_{Q<D}I_Q$, contradicting the local-center argument. Also $\operatorname{Br}_P(I_D)=0$ unless $P$ is conjugate into $D$: group the cosets of $G/D$ into $P$-orbits, which have no fixed point otherwise. Thus the minimal transfer subgroups are exactly the maximal $p$-subgroups with nonzero [Brauer morphism](../../../../../brauer-morphism.md) of $e$.

Now take $M=eM$ and write $e=\operatorname{Tr}_D^G(a)$. Multiplication by $a$ is a $D$-linear endomorphism $\alpha$ of $M$, and

$$
\operatorname{Tr}_D^G(\alpha)=\operatorname{id}_M.
$$

Here is the splitting behind the [D. Higman criterion](../../../../../d-higman-criterion.md). The natural map $\varepsilon:RG\otimes_{RD}M\to M$, $g\otimes m\mapsto gm$, has a $G$-linear section

$$
s(m)=\sum_{g\in G/D}g\otimes\alpha(g^{-1}m).
$$

Changing a representative by an element of $D$ leaves this tensor unchanged, $G$ permutes the terms, and $\varepsilon s=\operatorname{id}_M$. Hence

$$
\boxed{M\mid\operatorname{Ind}_D^G\operatorname{Res}_D^G M.}
$$

This is [relative projectivity](../../../../../relative-projective-module.md) for $D$, proving the [Green relative projectivity theorem](../../../../../modules-in-a-block-are-projective-relative-to-its-defect-group.md); indecomposability was needed only to speak of a single [block of a group algebra](../../../../../block-of-a-group-algebra.md) or [vertex of an indecomposable module](../../../../../vertex-of-an-indecomposable-module.md).

Finally let $\hat e$ lift $e$. A trace expression for $\hat e$ reduces to one for $e$, so a modular [defect group of a block](../../../../../defect-group-of-a-block.md) is contained, up to conjugacy, in an integral one. Conversely choose a modular defect group $D$ and $a\in(kG)^D$ with $e=\operatorname{Tr}_D^G(a)$. Conjugation orbit sums lift $a$ to $\hat a\in(\mathcal OG)^D$. The element

$$
u=\hat e\operatorname{Tr}_D^G(\hat a)\in\hat eZ(\mathcal OG)
$$

reduces to its block identity, hence is a unit in that block center. Its inverse there is central, so

$$
\hat e=\operatorname{Tr}_D^G(u^{-1}\hat e\hat a).
$$

The integral defect is therefore contained in the modular one. **The corresponding blocks have the same conjugacy class of defect groups and the same defect.**

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
