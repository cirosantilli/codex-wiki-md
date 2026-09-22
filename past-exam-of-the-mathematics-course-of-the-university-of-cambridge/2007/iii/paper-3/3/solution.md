<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The block statement is **[Green correspondence for blocks](../../../../../green-correspondence-for-blocks.md): if $N_G(D)\le H\le G$, blocks of $RG$ and $RH$ with defect group $D$ correspond, and their block bimodules are Green correspondents for the diagonal vertex $\Delta D$.** We prove the module correspondence underlying this statement, then specialize it to the block bimodules. This also gives the requested direct proof in the trivial-intersection situation.

Here are the elementary ingredients, including their proofs. [Mackey decomposition](../../../../../mackey-restriction-formula.md) is obtained by partitioning the tensor basis of $RG\otimes_{RL}U$ by the [double cosets](../../../../../double-coset.md) $H\backslash G/L$; the term for $g$ is induction from $H\cap{}^gL$ of the suitably conjugated restriction of $U$. The [D. Higman criterion](../../../../../d-higman-criterion.md) follows from the section constructed in Question 1. Conversely, take a splitting of the induction counit and its coefficient at the identity coset: equivariance reconstructs the section from that $H$-linear coefficient, and the splitting identity is exactly that its relative trace is $1$. Thus the trace criterion is an equivalence.

An [indecomposable module](../../../../../indecomposable-module.md) here has a [local endomorphism ring](../../../../../local-endomorphism-ring.md). Over $k$ this follows from the [Fitting lemma](../../../../../fitting-lemma.md): an endomorphism eventually splits its kernel from its image, and indecomposability makes it invertible or nilpotent. Over $\mathcal O$, the endomorphism ring is finite over a complete [discrete valuation ring](../../../../../discrete-valuation-ring.md); lift orthogonal idempotents from its finite-dimensional residue algebra to see that an indecomposable lattice has a local endomorphism ring too. The [Krull–Schmidt theorem](../../../../../krull-schmidt-theorem.md) follows by the usual exchange argument: composing the inclusion and projection of one indecomposable summand across a second decomposition writes its identity as a sum of endomorphisms; one is a unit in the local endomorphism ring and pairs that summand with a summand of the second decomposition. Remove the pair and continue. Existence follows by successively splitting nontrivial idempotents, which decreases dimension or rank.

A [vertex of an indecomposable module](../../../../../vertex-of-an-indecomposable-module.md) is a subgroup minimal for [relative projectivity](../../../../../relative-projective-module.md). It can be taken to be a $p$-subgroup because averaging over the index of a [Sylow subgroup](../../../../../sylow-subgroup.md) of any candidate subgroup is invertible. If an indecomposable module is relatively projective for $P$ and $Q$, the [Mackey decomposition](../../../../../mackey-restriction-formula.md) and its induction splittings make it a summand of a sum of modules induced from $P\cap{}^gQ$. In its local endomorphism ring one splitting component must be invertible, so it is relatively projective for one of these intersections. This proves conjugacy of minimal vertices and the useful criterion that a module with vertex $P$ can be relatively projective for $Q$ only when $P$ is conjugate into $Q$. A [source of an indecomposable module](../../../../../source-of-an-indecomposable-module.md) with vertex $P$ is an indecomposable summand $S$ of its restriction to $P$ from which the original module is an induced summand. Such a summand exists by the induction splitting and [Krull–Schmidt theorem](../../../../../krull-schmidt-theorem.md); its vertex is $P$, since a proper vertex would make the original module relatively projective for a proper subgroup of $P$.

Set

$$
\mathcal X=\{Q:Q\le D\cap{}^gD\text{ for some }g\notin H\},\qquad
\mathcal Y=\{Q:Q\le H\cap{}^gD\text{ for some }g\notin H\}.
$$

When saying a module is $\mathcal X$- or $\mathcal Y$-projective, allow conjugates in the relevant ambient group and finite sums of modules relatively projective for members of that family. No conjugate of $D$ inside $H$ belongs to $\mathcal Y$: if $D\le{}^h(H\cap{}^gD)$, equality of orders gives $D={} ^{hg}D$, so $hg\in N_G(D)\subseteq H$, contradicting $g\notin H$. Every member of $\mathcal X$ is a proper subgroup of $D$.

The two key assertions can now be proved rather than assumed. First, if $W$ is an indecomposable $D$-projective $RH$-module, then

$$
\operatorname{Res}_H^G\operatorname{Ind}_H^G W=W\oplus W',\qquad W'\text{ is }\mathcal Y\text{-projective}.
$$

Choose $U$ with $W\mid\operatorname{Ind}_D^H U$. [Mackey decomposition](../../../../../mackey-restriction-formula.md) gives $\operatorname{Res}_H^G\operatorname{Ind}_D^G U=\operatorname{Ind}_D^H U\oplus T$, with $T$ $\mathcal Y$-projective. Write $\operatorname{Ind}_D^H U=W\oplus W''$ and apply induction and restriction. Both $\operatorname{Res}\operatorname{Ind}W$ and $\operatorname{Res}\operatorname{Ind}W''$ contain their original modules, by the identity double coset. Comparing multiplicities of every indecomposable which is not $\mathcal Y$-projective, their extra multiplicities are nonnegative and have sum zero. Therefore neither has such an extra summand, proving the assertion.

Second, suppose $W$ has vertex $D$, and choose an indecomposable $V\mid\operatorname{Ind}_H^G W$ whose restriction contains $W$; such a $V$ exists by the first assertion. Write $\operatorname{Ind}W=V\oplus V'$. Its restriction has just one summand isomorphic to $W$ and all other summands are $\mathcal Y$-projective, so $\operatorname{Res}V'$ is $\mathcal Y$-projective. Any indecomposable $Z\mid V'$ has a vertex $P\le D$ after conjugacy. A source $S$ with vertex $P$ is a summand of $\operatorname{Res}_P Z$. Restricting a $\mathcal Y$-projective decomposition of $\operatorname{Res}_H Z$ to $P$ and using [Mackey decomposition](../../../../../mackey-restriction-formula.md) forces $P$ to lie in an $H$-conjugate of some $H\cap{}^gD$, $g\notin H$. Since $P\le D$, this puts $P$ in $\mathcal X$. Thus $V'$ is $\mathcal X$-projective. Moreover $V$ has vertex $D$, since it is $D$-projective and its restriction contains $W$ with vertex $D$. We have proved

$$
\operatorname{Ind}_H^G W=V\oplus V',\qquad V\text{ has vertex }D,\quad V'\text{ is }\mathcal X\text{-projective}.
$$

In particular $V$ is unique.

Conversely, let $V$ be an indecomposable $RG$-module with vertex $D$ and source $S$. Decompose $\operatorname{Ind}_D^H S$ and choose $W$ whose induction contains $V$. Its vertex is contained in $D$ and cannot be proper, since induction would then make $V$ relatively projective for a smaller subgroup. Thus $W$ has vertex $D$, and the previous assertion makes $V$ its unique vertex-$D$ induced summand. Restriction of an $\mathcal X$-projective module is $\mathcal Y$-projective: in a Mackey term a conjugating element inside $H$ preserves the containment in an $H$-conjugate of $\mathcal Y$, and one outside $H$ gives a subgroup of $H\cap{}^gD$. Comparing the two decompositions of $\operatorname{Res}\operatorname{Ind}W$ now gives

$$
\operatorname{Res}_H^G V=W\oplus U,\qquad U\text{ is }\mathcal Y\text{-projective}.
$$

These assignments are mutually inverse. To check sources, restrict $\operatorname{Ind}_D^H S$ back to $D$. Its terms of full vertex are conjugates of $S$ by $N_H(D)$; the other terms are induced from proper intersections. Applying the source criterion and [Krull–Schmidt theorem](../../../../../krull-schmidt-theorem.md) shows that the source of $W$ is one of those conjugates. The same argument in $G$, and the uniqueness just proved, matches the source classes on the two sides. Thus [Green correspondence](../../../../../green-correspondence.md) preserves sources up to normalizer conjugacy.

To pass to [blocks of a group algebra](../../../../../block-of-a-group-algebra.md), regard $RG$ as the [permutation module](../../../../../permutation-module.md) $R[(G\times G)/\Delta G]$. A summand of a permutation module has trivial source. Here is why: over a [finite p-group](../../../../../finite-p-group.md), every transitive permutation module is indecomposable, since its socle is the one-dimensional fixed line and every nonzero module has nonzero fixed points. The latter follows by induction on the group order, using a central element of order $p$ and the nilpotence of its difference from $1$. Over $\mathcal O$ indecomposability follows by reduction. Restrict a permutation summand to a vertex $P$ and apply [Krull–Schmidt theorem](../../../../../krull-schmidt-theorem.md); a source must be a transitive permutation module $R[P/Q]$. Its vertex is contained in $Q$, so minimality forces $Q=P$, and its source is the trivial module.

For a permutation module, its [Brauer quotient of a module](../../../../../brauer-quotient-of-a-module.md) at $P$ has the fixed permutation points as basis: every nontrivial orbit sum is a proper transfer. An indecomposable trivial-source summand with vertex $Q$ has nonzero quotient only at subgroups conjugate into $Q$, by its induced-permutation realization, and its quotient at $Q$ is nonzero because its restriction contains its trivial source. Applied to a block $B=kGe$, the quotient at $\Delta P$ is $\operatorname{Br}_P(e)kC_G(P)$. Together with the maximal-subgroup characterization of defect from Question 1, this proves that its bimodule vertices are precisely $\Delta D$ for its defect groups $D$. The integral conclusion follows by orbit-sum reduction and idempotent lifting.

Finally

$$
N_{G\times G}(\Delta D)=\{(a,b):a,b\in N_G(D),\ b^{-1}a\in C_G(D)\}\subseteq H\times H.
$$

Apply the just-proved [Green correspondence](../../../../../green-correspondence.md) with ambient group $G\times G$. Its unique vertex-$\Delta D$ summand of $B\downarrow_{H\times H}$ lies in $RH$: outside $H$ there is no $\Delta D$-fixed group-basis point, as in Question 2. Since the indecomposable $H\times H$ summands of $RH$ are exactly its block ideals, this summand is a block $b$ with defect group $D$. Conversely induction of $b$ has $B$ as its unique vertex-$\Delta D$ summand. The block bijection is the [Brauer correspondence](../../../../../brauer-correspondence.md) of Question 2, giving the claimed block form over either coefficient ring.

For the final special case put $N=N_G(D)$ with $D$ a trivial-intersection [Sylow subgroup](../../../../../sylow-subgroup.md). For $g\notin N$, the intersection $N\cap{}^gN$ has order prime to $p$. Indeed every $p$-subgroup of it lies both in the normal Sylow subgroup $D$ of $N$ and in ${}^gD$, whose intersection is trivial. [Mackey decomposition](../../../../../mackey-restriction-formula.md) therefore gives

$$
\operatorname{Res}_N^G\operatorname{Ind}_N^G M=M\oplus P,
$$

where every other double-coset term is induced from a group of order prime to $p$. By [Maschke's theorem](../../../../../maschke-s-theorem.md) such modules are projective, and induction preserves projectivity, so $P$ is projective.

Every nonprojective $kG$-module has nonprojective restriction to $N$: $[G:N]$ is prime to $p$, so averaging makes the module a summand of the induction of its restriction. A projective restriction would therefore make the original module projective. Decompose $\operatorname{Ind}_N^G M$ into indecomposables. Each nonprojective summand contributes a nonprojective summand on restriction, whereas the displayed Mackey formula and [Krull–Schmidt theorem](../../../../../krull-schmidt-theorem.md) have exactly one nonprojective summand, $M$, with multiplicity one. There must be one, since $M$ is nonprojective. Hence

$$
\boxed{\operatorname{Ind}_N^G M=M_0\oplus M_1,\quad M_0\text{ indecomposable and nonprojective},\quad M_1\text{ projective}.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
