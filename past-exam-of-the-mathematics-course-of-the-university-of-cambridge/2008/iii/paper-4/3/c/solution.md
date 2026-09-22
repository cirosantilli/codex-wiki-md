<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $B=kGe$ have defect [group](../../../../../../group-split.md) $D$. Use two vertex-and-source facts, with their relevant content made explicit. Every [indecomposable module](../../../../../../indecomposable-module.md) in $B$ has a [module vertex](../../../../../../vertex-of-an-indecomposable-module.md) conjugate into $D$. Also $B$, as a $k[G\times G]$-module with $(g,h)a=gah^{-1}$, is an indecomposable permutation-module summand with [module vertex](../../../../../../vertex-of-an-indecomposable-module.md) $\Delta D=\{(d,d):d\in D\}$ and trivial [module source](../../../../../../source-of-an-indecomposable-module.md). The second fact is the bimodule characterization of a [defect group of a block](../../../../../../defect-group-of-a-block.md); the first follows by applying its relative-$\Delta D$ induction splitting to $B\otimes_{kG}M=M$.

If $D$ is cyclic, every [module source](../../../../../../source-of-an-indecomposable-module.md) for every [module vertex](../../../../../../vertex-of-an-indecomposable-module.md) $Q\le D$ occurs among the finitely many [indecomposable modules for a cyclic p-group](../../../../../../indecomposable-modules-for-a-cyclic-p-group.md). Each [module](../../../../../../module-mathematics.md) in the block is a summand of an induction of one of these finitely many [module sources](../../../../../../source-of-an-indecomposable-module.md). There are finitely many [subgroups](../../../../../../subgroup.md) $Q$ and each [induced representation](../../../../../../induced-representation.md) has finitely many indecomposable summands by [Krull–Schmidt theorem](../../../../../../krull-schmidt-theorem.md). Thus **cyclic defect implies finite representation type of the block**.

For the converse, the restriction $B\downarrow_{D\times D}$ has the regular $kD$-bimodule as a [direct summand](../../../../../../direct-summand.md). To see this from [module vertices](../../../../../../vertex-of-an-indecomposable-module.md) and [module sources](../../../../../../source-of-an-indecomposable-module.md), its [Brauer quotient of a module](../../../../../../brauer-quotient-of-a-module.md) at $\Delta D$ is nonzero. Its summands are [permutation modules](../../../../../../permutation-module.md) for the $p$-group $D\times D$ and have [module vertices](../../../../../../vertex-of-an-indecomposable-module.md) of order at most $|D|$. A summand detected at $\Delta D$ therefore has [module vertex](../../../../../../vertex-of-an-indecomposable-module.md) $\Delta D$ and trivial [module source](../../../../../../source-of-an-indecomposable-module.md), hence is

$$
\operatorname{Ind}_{\Delta D}^{D\times D}k\cong kD.
$$

Here a transitive [permutation module](../../../../../../permutation-module.md) for a $p$-group is indecomposable: it has one-dimensional [head of a module](../../../../../../head-of-a-module.md) over the local [group algebra](../../../../../../group-algebra.md) and cannot split into two nonzero [modules](../../../../../../module-mathematics.md). This also explains the Brauer-quotient detection used in the argument.

For any $kD$-module $U$, tensor that split bimodule inclusion with $U$. It gives

$$
U\mid\operatorname{Res}_D^G(B\otimes_{kD}U),
$$

where $\mid$ denotes being a [direct summand](../../../../../../direct-summand.md). If $B$ has only finitely many [indecomposable modules](../../../../../../indecomposable-module.md) $M_1,\ldots,M_s$, each $B\otimes_{kD}U$ is a sum of these. Therefore every indecomposable $U$ must occur among the summands of the finite list $M_i\downarrow_D$. Thus $kD$ has finite representation type.

A noncyclic $p$-group has a quotient $C_p\times C_p$: its [Frattini quotient](../../../../../../frattini-quotient.md) has rank at least two, since a one-generator [Frattini quotient](../../../../../../frattini-quotient.md) forces the [group](../../../../../../group-split.md) itself to be cyclic. Inflation along this quotient embeds all the [indecomposable modules](../../../../../../indecomposable-module.md) of that elementary abelian [group](../../../../../../group-split.md), preserving isomorphisms and indecomposability. Part (b) rules out finite type when $k$ is infinite.

The conclusion remains valid if the splitting [field](../../../../../../field.md) $k$ is finite. For completeness, replace the scalar parameter in part (b) by an $m\times m$ companion matrix $T_f$ of an irreducible polynomial $f$. On $k^m\oplus k^m$ use

$$
x=\begin{pmatrix}0&0\\I&0\end{pmatrix},\qquad
y=\begin{pmatrix}0&0\\T_f&0\end{pmatrix}.
$$

An endomorphism commuting with these has form $\left(\begin{smallmatrix}A&0\\C&A\end{smallmatrix}\right)$ with $AT_f=T_fA$. Its [endomorphism ring](../../../../../../endomorphism-ring.md) has a square-zero [ideal](../../../../../../ideal.md) of the $C$-matrices and quotient $k[T_f]\cong k[t]/(f)$, a [field](../../../../../../field.md), so it is local and the [module](../../../../../../module-mathematics.md) is indecomposable. Finite [fields](../../../../../../field.md) have irreducible polynomials of arbitrarily large degrees, giving infinitely many dimensions. This also excludes noncyclic $D$ in that case. Altogether,

$$
\boxed{B\text{ has finite representation type}\quad\Longleftrightarrow\quad D\text{ is cyclic}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
