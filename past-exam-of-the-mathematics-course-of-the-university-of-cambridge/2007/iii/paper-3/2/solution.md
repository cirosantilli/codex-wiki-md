<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Brauer first main theorem](../../../../../brauer-first-main-theorem.md) says that, for a fixed [p-subgroup](../../../../../p-subgroup.md) $D$ and $N=N_G(D)$, there is a bijection between [blocks of a group algebra](../../../../../block-of-a-group-algebra.md) of $kG$ with [defect group of a block](../../../../../defect-group-of-a-block.md) $D$ and blocks of $kN$ with that defect group. Correspondents have the same nonzero image under $\operatorname{Br}_D$. The integral version follows by [modular reduction of block idempotents](../../../../../modular-reduction-of-block-idempotents.md).

Here is a proof using [relative traces](../../../../../relative-trace.md). Put $C=C_G(D)$ and

$$
I_D^G=\operatorname{Tr}_D^G((kG)^D),\qquad J_D=\operatorname{Tr}_D^N(kC)\subseteq(kC)^N.
$$

The latter ambient [algebra](../../../../../algebra-split.md) is commutative because invariance under $N$ includes invariance under $C$. The [Brauer morphism and relative trace](../../../../../brauer-morphism-and-relative-trace.md) identity is

$$
\operatorname{Br}_D\operatorname{Tr}_D^G(a)=\operatorname{Tr}_D^N\operatorname{Br}_D(a).
$$

Indeed $D$ acts on $G/D$. Its fixed cosets are exactly $N/D$. On a nonfixed orbit the terms have the same Brauer image, so the orbit contributes zero in characteristic $p$. The fixed cosets give the right-hand side. Since every element of $kC$ is $D$-fixed, this proves that $\operatorname{Br}_D:I_D^G\twoheadrightarrow J_D$ is a surjective [algebra homomorphism](../../../../../algebra-homomorphism-over-a-field.md) of commutative ideals. The same argument for $N$ has exactly the same target.

We use the following elementary fact about [primitive idempotents under a surjection of commutative Artinian ideals](../../../../../primitive-idempotents-under-a-surjection-of-commutative-artinian-ideals.md). Under a surjection $f:I\twoheadrightarrow J$ of ideals in finite-dimensional commutative [algebras](../../../../../algebra-split.md), the primitive ambient idempotents lying in $I$ and having nonzero image correspond bijectively to the primitive idempotents in $J$. To prove it, decompose the source ambient algebra into [Artinian local rings](../../../../../artinian-local-ring.md) $A_i$. Either $I\cap A_i=A_i$, or it is a proper, hence nilpotent, ideal. Proper components contribute no idempotents to the image. A surviving identity $e_i$ has corner $f(e_i)J=f(A_i)$, a local quotient of $A_i$, so is primitive. The surviving identities are orthogonal and exhaust the idempotents of the target. Notice that this proof does not assert that the whole kernel is nilpotent: it can kill entire block components.

By the [trace criterion for defect groups](../../../../../trace-criterion-for-defect-groups.md) proved above, primitive block idempotents in $I_D^G$ have defect conjugate into $D$. Among them, the [Brauer morphism](../../../../../brauer-morphism.md) is nonzero precisely for defect $D$, again by that criterion and its Brauer characterization. The identical reasoning applies to $I_D^N$. Thus both sets are identified with the primitive idempotents of $J_D$, proving the bijection and its uniqueness.

For the more general subgroup, $D$ is understood to be a [defect group of a block](../../../../../defect-group-of-a-block.md) $b$ of $kH$. This is the implicit hypothesis needed to apply the theorem; it is not repeated in the printed sentence. Without it the printed uniqueness assertion is false: take $G=A_5$, $H=A_4$, $p=3$ and $D=C_3$. The centralizer of $D$ in $A_5$ is $D$, but the unique three-dimensional defect-zero block of $kA_4$ is the bimodule restriction of each of the two three-dimensional defect-zero blocks of $kA_5$. The two ordinary degree-three characters both restrict to the degree-three character of $A_4$, with values $3,-1,0$ on its identity, involutions and elements of order three. Defect-zero reduction gives the same simple projective $kA_4$-module, so both restricted block bimodules are this same matrix block. This illustrates why [block induction requires the block's defect centralizer](../../../../../block-induction-requires-the-block-s-defect-centralizer.md). Write $e_b$ for its block idempotent and $K=N_H(D)$. Since $DC_G(D)\le H$, we have $DC_G(D)\le K\le N_G(D)$. Apply the theorem inside $H$ to obtain the unique corresponding block $\beta$ of $kK$. Its [center of an associative algebra](../../../../../center-of-an-associative-algebra.md) has a residue [field](../../../../../field.md) $F_\beta$, and the quotient map is its [central character of a block](../../../../../central-character-of-a-block.md) $\omega_\beta:Z(kK)\to F_\beta$. No assumption that $k$ is algebraically closed is needed here. Define

$$
\omega_b^G(z)=\omega_\beta(\operatorname{Br}_D^G(z)),\qquad z\in Z(kG).
$$

The Brauer image is in $(kC_G(D))^{N_G(D)}\subseteq Z(kK)$, so this is a unital [algebra homomorphism](../../../../../algebra-homomorphism-over-a-field.md). Among the orthogonal primitive [central idempotents](../../../../../central-idempotent.md) of $kG$, exactly one has image $1$. **The block it selects is $b^G$.** If $H$ contains $N_G(D)$ this is the inverse of the bijection just proved. For arbitrary $H$, the resulting block can have a strictly larger defect group. [Block induction](../../../../../block-induction.md) is transitive on admissible intermediate subgroups. For the normalizer chain used in the proof below, the required transitivity will be verified directly with Brauer images.

To prove the bimodule characterization, we explicitly state the standard permutation-module fact used here. For a [permutation module](../../../../../permutation-module.md), the [Brauer quotient of a module](../../../../../brauer-quotient-of-a-module.md) at $P$ has as basis the permutation-basis points fixed by $P$. An indecomposable summand has nonzero quotient at $P$ exactly when its [vertex of an indecomposable module](../../../../../vertex-of-an-indecomposable-module.md) contains a conjugate of $P$. For summands with vertex exactly $P$, taking this quotient, with its $N(P)/P$-action, detects the summand and detects which orthogonal idempotent projection acts as its identity. These facts hold for [trivial source modules](../../../../../trivial-source-module.md); the fixed-basis description follows by deleting proper transfers, and the detection assertion is the permutation form of the first-main-theorem argument, applied to their endomorphism algebra.

As an $H\times H$ [permutation module](../../../../../permutation-module.md), with $(h_1,h_2)g=h_1gh_2^{-1}$, the group algebra decomposes as

$$
kG\downarrow_{H\times H}=kH\oplus\bigoplus_{g\in H\backslash G/H,\ g\notin H}kHgH.
$$

The block bimodule $b$ is an [indecomposable module](../../../../../indecomposable-module.md) with [vertex of an indecomposable module](../../../../../vertex-of-an-indecomposable-module.md) $\Delta D=\{(d,d):d\in D\}$. None of the other double-coset modules can contain $b$: a basis element fixed by $\Delta D$ centralizes $D$, hence lies in $C_G(D)\subseteq H$, whereas those double cosets lie outside $H$. Thus $b$ occurs exactly once as an indecomposable summand of this restriction, in the $kH$ term. Decomposing $kG$ into its global block bimodules therefore puts this occurrence in precisely one of them, say $B$.

Under the fixed-basis description, the quotient of $kG$ at $\Delta D$ is $kC_G(D)$, and multiplication by $e_B$ induces multiplication by $\operatorname{Br}_D(e_B)$. The quotient of $b$ is $\operatorname{Br}_D^H(e_b)kC_G(D)=e_\beta kC_G(D)$. Consequently the detecting projection for this occurrence of $b$ satisfies

$$
\operatorname{Br}_D^G(e_B)e_\beta=e_\beta,
$$

which is equivalent to $\omega_b^G(e_B)=1$. Thus $B=b^G$, proving the requested **unique-block direct-summand characterization**. Here the restriction is to $H\times H$; the extra subscript in the converted TeX is a transcription error, not a different subgroup.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
