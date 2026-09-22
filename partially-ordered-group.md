# Partially ordered group

↑ **Parent:** [Group](group.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Partially_ordered_group)

A [group](group.md) with a [partial order](set.md#partially-ordered-set) preserved by multiplication on both sides: $a\le b$ implies $xay\le xby$ for all $x,y$. In additive notation this says $a\le b\Rightarrow x+a+y\le x+b+y$. Preserving only one side is a different orderability condition.

**Table of contents**

- [Positive cone of an ordered group](#positive-cone-of-an-ordered-group)
- [Convex subgroup of an ordered group](#convex-subgroup-of-an-ordered-group)
- [Lattice-ordered group](#lattice-ordered-group)
  - [Riesz decomposition in a lattice-ordered group](#riesz-decomposition-in-a-lattice-ordered-group)
  - [Lattice-ordered group homomorphism](#lattice-ordered-group-homomorphism)
  - [Absolute value in a lattice-ordered group](#absolute-value-in-a-lattice-ordered-group)
    - [Positive and negative parts in a lattice-ordered group](#positive-and-negative-parts-in-a-lattice-ordered-group)
  - [Convex lattice subgroup](#convex-lattice-subgroup)
    - [One-sided bounds for adjoining a positive element](#one-sided-bounds-for-adjoining-a-positive-element)
    - [Ordered right cosets of a convex lattice subgroup](#ordered-right-cosets-of-a-convex-lattice-subgroup)
    - [Lattice of convex lattice subgroups](#lattice-of-convex-lattice-subgroups)
    - [Principal convex lattice subgroup](#principal-convex-lattice-subgroup)
    - [Prime convex lattice subgroup](#prime-convex-lattice-subgroup)
    - [Value in a lattice-ordered group](#value-in-a-lattice-ordered-group)
      - [Squared bound from comparison at values](#squared-bound-from-comparison-at-values)
      - [Cover of a value in a lattice-ordered group](#cover-of-a-value-in-a-lattice-ordered-group)
        - [Power cofinality in the cover of a value](#power-cofinality-in-the-cover-of-a-value)
  - [Normal-valued lattice-ordered group](#normal-valued-lattice-ordered-group)
    - [Wolfenstein inequality for normal-valued lattice-ordered groups](#wolfenstein-inequality-for-normal-valued-lattice-ordered-groups)
  - [Linearly ordered group](#linearly-ordered-group)
    - [Archimedean ordered group](#archimedean-ordered-group)
      - [Archimedean linearly ordered groups are Abelian](#archimedean-linearly-ordered-groups-are-abelian)
    - [Lexicographically ordered group](#lexicographically-ordered-group)
    - [Convex subgroups of a finite-rank ordered Abelian group](#convex-subgroups-of-a-finite-rank-ordered-abelian-group)
    - [Ohnishi orderability criterion](#ohnishi-orderability-criterion)
  - [Abelian lattice-ordered group](#abelian-lattice-ordered-group)
    - [Hahn group](#hahn-group)
      - [Finite-support Hahn embedding along a countable convex chain](#finite-support-hahn-embedding-along-a-countable-convex-chain)
    - [Free Abelian lattice-ordered group](#free-abelian-lattice-ordered-group)
      - [Piecewise integer-linear representation of a free Abelian lattice-ordered group](#piecewise-integer-linear-representation-of-a-free-abelian-lattice-ordered-group)
        - [Integer-linear hinge functions have infinite independent rank](#integer-linear-hinge-functions-have-infinite-independent-rank)
  - [Lattice-ordered permutation group](#lattice-ordered-permutation-group)
    - [Order-primitive lattice permutation group](#order-primitive-lattice-permutation-group)
      - [McCleary trichotomy theorem](#mccleary-trichotomy-theorem)
    - [Holland representation theorem](#holland-representation-theorem)
    - [Order n-transitivity](#order-n-transitivity)
      - [Finite interpolation by lattice operations](#finite-interpolation-by-lattice-operations)
    - [Positive bump of an order automorphism](#positive-bump-of-an-order-automorphism)
      - [Conjugacy of positive real-line bumps](#conjugacy-of-positive-real-line-bumps)
        - [Conjugating positive bumps while preserving a fundamental interval](#conjugating-positive-bumps-while-preserving-a-fundamental-interval)

## Positive cone of an ordered group

↑ **Parent:** [Partially ordered group](partially-ordered-group.md)

The nonnegative cone determines the [partial order](set.md#partially-ordered-set) by $a\le b\iff a^{-1}b\in G_{\ge1}$. It contains the [identity element](group.md#identity-element), is closed under products and [conjugation](group-theory.md#conjugation), and intersects its inverse only in the identity. Conversely these conditions define a two-sided invariant [partial order](set.md#partially-ordered-set). Its strictly positive part omits the identity; conventions for $G^+$ differ, so specify which is intended.

## Convex subgroup of an ordered group

↑ **Parent:** [Partially ordered group](partially-ordered-group.md)

A [subgroup](group.md#subgroup) $C$ is convex if $c_1\le g\le c_2$ with $c_1,c_2\in C$ implies $g\in C$. In a [linearly ordered group](#linearly-ordered-group), convex subgroups form a chain under inclusion: positive elements witnessing incomparability would be comparable and force the smaller one into the other subgroup by convexity.

## Lattice-ordered group

↑ **Parent:** [Partially ordered group](partially-ordered-group.md)

An [ordered group](partially-ordered-group.md) whose [partial order](set.md#partially-ordered-set) is a [lattice](mathematical-logic.md#lattice). Each pair has a [join](set.md#least-upper-bound-in-a-partially-ordered-set) $f\vee g$ and a [meet](set.md#greatest-lower-bound-in-a-partially-ordered-set) $f\wedge g$. Translations preserve these operations, for example $a(f\vee g)b=afb\vee agb$. Pointwise [maximum](set.md#maximum-of-a-subset-of-a-total-order) and [minimum](set.md#minimum-of-a-subset-of-a-total-order) make the [order automorphisms](set.md#order-automorphism) of a chain into a lattice-ordered group.

### Riesz decomposition in a lattice-ordered group

↑ **Parent:** [Lattice-ordered group](#lattice-ordered-group)

For $a,b\ge1$, take $a'=x\wedge a$ and $b'=(a')^{-1}x$. Then $a'\ge1$ and $b'=1\vee a^{-1}x$ is between one and $b$. Thus $x=a'b'$. Repetition splits a positive element bounded by a finite product into factors bounded by the corresponding factors. Every resulting positive factor is also bounded by $x$.

### Lattice-ordered group homomorphism

↑ **Parent:** [Lattice-ordered group](#lattice-ordered-group)

A [group homomorphism](group-theory.md#group-homomorphism) preserving both [join](set.md#least-upper-bound-in-a-partially-ordered-set) and [meet](set.md#greatest-lower-bound-in-a-partially-ordered-set). A bijective such map is an isomorphism of [lattice-ordered groups](#lattice-ordered-group); an injective one is an embedding.

### Absolute value in a lattice-ordered group

↑ **Parent:** [Lattice-ordered group](#lattice-ordered-group)

The displayed [join](set.md#least-upper-bound-in-a-partially-ordered-set) is nonnegative in a [lattice-ordered group](#lattice-ordered-group). In an additive [Abelian group](group.md#abelian-group) it becomes $|g|=g\vee(-g)$. This order-theoretic absolute value need not be a real scalar.

#### Positive and negative parts in a lattice-ordered group

↑ **Parent:** [Absolute value in a lattice-ordered group](#absolute-value-in-a-lattice-ordered-group)

The two positive parts satisfy $g=g^+(g^-)^{-1}$, commute with one another, and have [meet](set.md#greatest-lower-bound-in-a-partially-ordered-set) one. They isolate positive and negative displacement in the pointwise model of a [lattice-ordered permutation group](#lattice-ordered-permutation-group). These are group elements, unlike the scalar positive part of a real number.

### Convex lattice subgroup

↑ **Parent:** [Lattice-ordered group](#lattice-ordered-group)

A [convex subgroup of an ordered group](#convex-subgroup-of-an-ordered-group) that is also closed under [join](set.md#least-upper-bound-in-a-partially-ordered-set) and [meet](set.md#greatest-lower-bound-in-a-partially-ordered-set). A normal convex lattice subgroup is the kernel of the quotient [lattice-ordered group homomorphism](#lattice-ordered-group-homomorphism).

#### One-sided bounds for adjoining a positive element

↑ **Parent:** [Convex lattice subgroup](#convex-lattice-subgroup)

Assume $uv\leq v^2u^2$ for all $u,v\geq1$ in a [lattice-ordered group](#lattice-ordered-group). For a [convex lattice subgroup](#convex-lattice-subgroup) $H$ and $a\geq1$, the displayed bounds allow $h\in H$ with $h\geq1$ and integers $n\geq0$. To prove the first set is a subgroup, use $(ha^n)(ka^m)\leq hk^2a^{2n+m}$. Products and inverse products are both bounded because $xy\leq|x||y|$ and $(xy)^{-1}\leq|y||x|$. Taking the larger exponent and a [join](set.md#least-upper-bound-in-a-partially-ordered-set) of the two bounds in $H$ bounds their [absolute value in a lattice-ordered group](#absolute-value-in-a-lattice-ordered-group). Inversion preserves that absolute value; common bounds using $h\vee k$ prove lattice closure and convexity. The set contains $H$ and $a$, and any convex lattice subgroup containing them contains the entire set. The second equality follows by applying the proof to the opposite group, where the required inequality is the original one with the variables interchanged.

#### Ordered right cosets of a convex lattice subgroup

↑ **Parent:** [Convex lattice subgroup](#convex-lattice-subgroup)

The displayed relation makes the right cosets into a [lattice](mathematical-logic.md#lattice), with $Pg\vee Ph=P(g\vee h)$ and $Pg\wedge Ph=P(g\wedge h)$. Antisymmetry uses convexity: $g\le ph$ and $h\le qg$ give $1\le phg^{-1}\le pq\in P$, hence $hg^{-1}\in P$. A [prime convex lattice subgroup](#prime-convex-lattice-subgroup) makes this order total even if the subgroup is not normal.

#### Lattice of convex lattice subgroups

↑ **Parent:** [Convex lattice subgroup](#convex-lattice-subgroup)

The [convex lattice subgroups](#convex-lattice-subgroup) of a [lattice-ordered group](#lattice-ordered-group) form a distributive [lattice](mathematical-logic.md#lattice), with intersection as [meet](set.md#greatest-lower-bound-in-a-partially-ordered-set) and the convex lattice subgroup generated by a union as [join](set.md#least-upper-bound-in-a-partially-ordered-set). A positive element of a join is bounded by a finite product of positive elements from the generating subgroups. [Riesz decomposition in a lattice-ordered group](#riesz-decomposition-in-a-lattice-ordered-group) splits such an element into positive factors from those subgroups. If the original element belongs to another convex subgroup $E$, every factor does too. Consequently $E\cap(C\vee D)=(E\cap C)\vee(E\cap D)$.

#### Principal convex lattice subgroup

↑ **Parent:** [Convex lattice subgroup](#convex-lattice-subgroup)

For $u\ge1$ in a [lattice-ordered group](#lattice-ordered-group), the displayed set is the smallest [convex lattice subgroup](#convex-lattice-subgroup) containing $u$. Products of two such bounds are bounded by a larger power of $u$; inversion and the [lattice](mathematical-logic.md#lattice) operations preserve the bounds. This gives an explicit test for membership.

#### Prime convex lattice subgroup

↑ **Parent:** [Convex lattice subgroup](#convex-lattice-subgroup)

A proper [convex lattice subgroup](#convex-lattice-subgroup) $P$ is prime when $a,b\ge1$ and $a\wedge b=1$ imply $a\in P$ or $b\in P$. Equivalently the ordered right cosets of $P$ form a [totally ordered set](set.md#totally-ordered-set). Prime refers to this order property, and does not require a [normal subgroup](group-theory.md#normal-subgroup) or prime index.

#### Value in a lattice-ordered group

↑ **Parent:** [Convex lattice subgroup](#convex-lattice-subgroup)

A value of $g\ne1$ is a [convex lattice subgroup](#convex-lattice-subgroup) maximal among those omitting $g$. [Zorn's lemma](set-theory.md#zorn-s-lemma) supplies a value: the union of a chain of convex lattice subgroups omitting $g$ still omits $g$. Such subgroups are prime. Their unique cover is the smallest convex lattice subgroup properly containing them.

##### Squared bound from comparison at values

↑ **Parent:** [Value in a lattice-ordered group](#value-in-a-lattice-ordered-group)

Let $p,q,x\geq1$ in a [lattice-ordered group](#lattice-ordered-group). Under the displayed hypothesis, suppose $d=(xq^{-2}p^{-2})\vee1>1$ and choose a value $P$ of $d$. If $x\in P$, then $1\leq d\leq x$ contradicts its omission. Otherwise extend $P$ to a value $V$ of $x$. The right-coset test is $Vu\leq Vv\iff(uv^{-1})\vee1\in V$. If $p\notin V$, put $c=(xq^{-2}p^{-1})\vee1\in V$. Then $(pc^{-1})\vee1\notin V$, while its inverse positive part is $(cp^{-1})\vee1=d$. These parts have [meet](set.md#greatest-lower-bound-in-a-partially-ordered-set) one, so primeness of $P$ forces $d\in P$. If $p\in V$, put $c=(xq^{-1})\vee1\in V$ and $t=p^2q\notin V$; the disjoint pair $(tc^{-1})\vee1$ and $(ct^{-1})\vee1=d$ gives the same contradiction. No normality assumption is used in this separation argument.

##### Cover of a value in a lattice-ordered group

↑ **Parent:** [Value in a lattice-ordered group](#value-in-a-lattice-ordered-group)

If $V$ is a [value in a lattice-ordered group](#value-in-a-lattice-ordered-group) of $t>1$, every [convex lattice subgroup](#convex-lattice-subgroup) strictly containing $V$ contains $t$. Thus the convex lattice subgroup generated by $V$ and $t$ is the unique least subgroup properly containing $V$. It is called the cover of $V$. There is no intermediate [convex lattice subgroup](#convex-lattice-subgroup). A [normal-valued lattice-ordered group](#normal-valued-lattice-ordered-group) requires $V$ to be a [normal subgroup](group-theory.md#normal-subgroup) of this cover, not necessarily of the whole group. Values are [prime convex lattice subgroups](#prime-convex-lattice-subgroup): maximality omitting $t$ makes them meet-irreducible in the [lattice of convex lattice subgroups](#lattice-of-convex-lattice-subgroups), so their ordered right cosets form a chain.

###### Power cofinality in the cover of a value

↑ **Parent:** [Cover of a value in a lattice-ordered group](#cover-of-a-value-in-a-lattice-ordered-group)

Under the inequality in [one-sided bounds for adjoining a positive element](#one-sided-bounds-for-adjoining-a-positive-element), if $a\geq1$ belongs to the [cover of a value in a lattice-ordered group](#cover-of-a-value-in-a-lattice-ordered-group) $V^*$ but not to $V$, then $\langle V,a\rangle_c=V^*$. Thus every $b\geq1$ in the cover is bounded above by both $va^n$ and $a^mw$ for suitable nonnegative $v,w\in V$ and integers $m,n\geq0$. The corresponding right and left coset bounds give the displayed cofinality, without first assuming that $V$ is normal. Left-coset order is obtained by inversion of right-coset order.

### Normal-valued lattice-ordered group

↑ **Parent:** [Lattice-ordered group](#lattice-ordered-group)

A [lattice-ordered group](#lattice-ordered-group) is normal-valued when every [value in a lattice-ordered group](#value-in-a-lattice-ordered-group) is a [normal subgroup](group-theory.md#normal-subgroup) of its cover. Normality in the cover is weaker than normality in the entire group. Every [linearly ordered group](#linearly-ordered-group) is normal-valued.

#### Wolfenstein inequality for normal-valued lattice-ordered groups

↑ **Parent:** [Normal-valued lattice-ordered group](#normal-valued-lattice-ordered-group)

A [lattice-ordered group](#lattice-ordered-group) is normal-valued precisely when the displayed inequality holds for all its elements. The theorem is proved without using it as a definition. In the forward direction a normal value has a linearly ordered quotient of its cover with no proper nontrivial convex subgroup. That quotient is Archimedean, hence Abelian by [Archimedean linearly ordered groups are Abelian](#archimedean-linearly-ordered-groups-are-abelian). Apply [squared bound from comparison at values](#squared-bound-from-comparison-at-values) to $p=b,q=a,x=ab$. For the reverse direction, [power cofinality in the cover of a value](#power-cofinality-in-the-cover-of-a-value) excludes a conjugate $u=a^{-1}va$ outside the value: its right cosets $Vu^n$ are all bounded by $Va$, contradicting cofinality above $Va^2$. Left-coset cofinality treats $ava^{-1}$. Every element is a quotient of nonnegative lattice parts, proving normality in the cover. In a [linearly ordered group](#linearly-ordered-group), comparison of $a,b\geq1$ immediately gives $ab\leq\max(a,b)^2\leq b^2a^2$, so every such group is normal-valued.

### Linearly ordered group

↑ **Parent:** [Lattice-ordered group](#lattice-ordered-group)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linearly_ordered_group)

A [group](group.md) with a two-sided invariant [total order](set.md#total-order). Thus it is a [lattice-ordered group](#lattice-ordered-group) whose [join](set.md#least-upper-bound-in-a-partially-ordered-set) and [meet](set.md#greatest-lower-bound-in-a-partially-ordered-set) choose the larger and smaller element. An order on only one side is not sufficient here. Every linearly ordered group is [torsion-free](fiber-bundle.md#torsion-free-connection): a positive element has strictly increasing positive powers, and a negative element has a positive inverse.

#### Archimedean ordered group

↑ **Parent:** [Linearly ordered group](#linearly-ordered-group)

An [ordered group](partially-ordered-group.md) is Archimedean when $a\ge1$ and $a^n\le b$ for all positive [integers](number-theory.md#integer) force $a=1$. In an additive [Abelian group](group.md#abelian-group) this excludes a positive element whose every integer multiple stays below one fixed bound. This generalizes the [Archimedean property](arithmetic.md#archimedean-property) of the [real numbers](arithmetic.md#real-number).

##### Archimedean linearly ordered groups are Abelian

↑ **Parent:** [Archimedean ordered group](#archimedean-ordered-group)

An [Archimedean ordered group](#archimedean-ordered-group) with a two-sided invariant [total order](set.md#total-order) is commutative. If there is a least positive element, its cofinal powers exhaust the group. Otherwise each $c>1$ has $d>1$ with $d^2<c$. To see this, choose $1<s<r<c$ and use $rs^{-1}$ if its square is below $r$; if not, the inequality $(rs^{-1})^2\geq r$ gives $s^2\leq r<c$. If positive $g,h$ satisfied $gh<hg$, put $c=(gh)^{-1}hg$ and choose such a $d$. Cofinality gives $d^m\leq g<d^{m+1}$ and $d^n\leq h<d^{n+1}$. Two-sided order invariance then gives both $hg<d^{m+n+2}$ and $hg=ghc>d^{m+n+2}$, a contradiction. Replacing negative elements by their inverses reduces arbitrary commutativity to the positive case.

#### Lexicographically ordered group

↑ **Parent:** [Linearly ordered group](#linearly-ordered-group)

For ordered [Abelian groups](group.md#abelian-group), compare tuples at their first differing coordinate. This gives a two-sided invariant [total order](set.md#total-order) on their direct product. The additive group $\mathbb Z^2$ with its first coordinate dominant is not an [Archimedean ordered group](#archimedean-ordered-group), since $n(0,1)<(1,0)$ for every positive integer $n$.

#### Convex subgroups of a finite-rank ordered Abelian group

↑ **Parent:** [Linearly ordered group](#linearly-ordered-group)

For a [torsion-free abelian group](group.md#torsion-free-abelian-group) of finite rational rank $r$, each [convex subgroup of an ordered group](#convex-subgroup-of-an-ordered-group) is pure: if $ng\in C$ for a positive integer $n$, then $g$ lies between zero and $ng$ or their negatives and hence belongs to $C$. A proper inclusion of convex subgroups therefore increases rational rank. They form a chain, so there are at most $r+1$, including zero and the whole group. A lexicographically ordered copy of $\mathbb Z^r$ attains the bound.

#### Ohnishi orderability criterion

↑ **Parent:** [Linearly ordered group](#linearly-ordered-group)

A [group](group.md) admits a two-sided invariant [total order](set.md#total-order) exactly when every finite list of nonidentity elements can be signed so that the conjugation-invariant [semigroup](algebra.md#semigroup) generated by the signed elements excludes the identity. A [compactness theorem](mathematical-logic.md#compactness-theorem) argument supplies a compatible global sign assignment. Omitting the conjugates changes the criterion to a different orderability problem.

### Abelian lattice-ordered group

↑ **Parent:** [Lattice-ordered group](#lattice-ordered-group)

A commutative [lattice-ordered group](#lattice-ordered-group), usually written additively. Examples include real-valued function groups with pointwise [addition](arithmetic.md#addition), [maximum](set.md#maximum-of-a-subset-of-a-total-order) and [minimum](set.md#minimum-of-a-subset-of-a-total-order). Such a group need not have a [total order](set.md#total-order).

#### Hahn group

↑ **Parent:** [Abelian lattice-ordered group](#abelian-lattice-ordered-group)

For a [totally ordered set](set.md#totally-ordered-set) $\Gamma$, take real coefficient families whose support satisfies the maximum condition: every nonempty subset of the support has a largest index. Add coefficients pointwise and decide the sign from the largest nonzero coordinate. This defines an ordered [Abelian group](group.md#abelian-group). For $\Gamma=\mathbb Z_{>0}$ with its usual order, the maximum condition forces finite support. Some presentations reverse the index order and use a minimum instead; specify the convention when applying an embedding theorem.

##### Finite-support Hahn embedding along a countable convex chain

↑ **Parent:** [Hahn group](#hahn-group)

Let a divisible ordered [Abelian group](group.md#abelian-group) be the union of a strictly increasing sequence of convex subgroups $C_1=0,C_2,\ldots$, with each ordered quotient $C_{n+1}/C_n$ isomorphic to the additive real line. Convexity makes every $C_n$ divisible, so these are rational [vector subspaces](vector-space.md#vector-subspace). Choose a rational-linear section for each quotient. Every element then has a unique finite sum of section values. Its sign is the sign of the coefficient of the largest active index, because convexity makes the corresponding ordered quotient decide its sign. The coefficients give an embedding, indeed an ordered-group isomorphism, into the [Hahn group](#hahn-group) with positive integer indices in the maximum-support convention. No compatibility of a separate real scalar multiplication is needed for this group embedding.

#### Free Abelian lattice-ordered group

↑ **Parent:** [Abelian lattice-ordered group](#abelian-lattice-ordered-group)

The free object on generators $x_1,\ldots,x_n$ has the [universal property](category-theory.md#universal-property) that an arbitrary assignment of these generators to an [Abelian lattice-ordered group](#abelian-lattice-ordered-group) extends uniquely to a [lattice-ordered group homomorphism](#lattice-ordered-group-homomorphism). It can be constructed from terms using addition, negation, zero, [join](set.md#least-upper-bound-in-a-partially-ordered-set) and [meet](set.md#greatest-lower-bound-in-a-partially-ordered-set), modulo identities valid in every Abelian lattice-ordered group. Its underlying group need not be finitely generated even when there are only two lattice generators.

##### Piecewise integer-linear representation of a free Abelian lattice-ordered group

↑ **Parent:** [Free Abelian lattice-ordered group](#free-abelian-lattice-ordered-group)

Evaluate the generators as coordinate projections on $\mathbb R^n$. The [lattice-ordered group](#lattice-ordered-group) they generate consists of continuous [positively homogeneous](real-analysis.md#positively-homogeneous-function-degree-one) [piecewise linear functions](function.md#piecewise-linear-function) with finitely many integer-linear pieces. Equivalently its elements are finite [joins](set.md#least-upper-bound-in-a-partially-ordered-set) of finite [meets](set.md#greatest-lower-bound-in-a-partially-ordered-set) of integer linear forms. The [universal property](category-theory.md#universal-property) follows because the real line detects every identity of [Abelian lattice-ordered groups](#abelian-lattice-ordered-group): if an identity fails, pass to a prime ordered quotient and select the finitely many active linear pieces. The resulting rational linear inequalities have a real solution by the alternative underlying [Farkas' lemma](convex-optimization.md#farkas-lemma), giving a real witness to failure. This is a statement about integer coefficients and positive homogeneity, not arbitrary real coefficients or affine constant terms.

###### Integer-linear hinge functions have infinite independent rank

↑ **Parent:** [Piecewise integer-linear representation of a free Abelian lattice-ordered group](#piecewise-integer-linear-representation-of-a-free-abelian-lattice-ordered-group)

The [piecewise linear functions](function.md#piecewise-linear-function) $h_n$, for distinct integer indices, are linearly independent over the integers. Restrict a finite integer relation to $y=1$. At $x=n$, only $h_n$ has a jump of one in its slope; hence the coefficient of that function must be zero. This proves that the underlying group of the two-generated [free Abelian lattice-ordered group](#free-abelian-lattice-ordered-group) has infinite [rank of an abelian group](group.md#rank-of-an-abelian-group).

### Lattice-ordered permutation group

↑ **Parent:** [Lattice-ordered group](#lattice-ordered-group)

A [group](group.md) of [order automorphisms](set.md#order-automorphism) of a [totally ordered set](set.md#totally-ordered-set) that is closed under pointwise [maximum](set.md#maximum-of-a-subset-of-a-total-order) and [minimum](set.md#minimum-of-a-subset-of-a-total-order). Products act on the right when writing $\alpha f$; then $\alpha(fg)=(\alpha f)g$. The pointwise lattice operations make it a [lattice-ordered group](#lattice-ordered-group).

#### Order-primitive lattice permutation group

↑ **Parent:** [Lattice-ordered permutation group](#lattice-ordered-permutation-group)

A transitive [lattice-ordered permutation group](#lattice-ordered-permutation-group) is order-primitive when its only invariant equivalence relations with convex classes are equality and the universal relation. This concerns convex blocks in a chain, rather than arbitrary blocks of a [primitive group action](group-theory.md#primitive-group-action).

##### McCleary trichotomy theorem

↑ **Parent:** [Order-primitive lattice permutation group](#order-primitive-lattice-permutation-group)

A faithful transitive [order-primitive lattice permutation group](#order-primitive-lattice-permutation-group) is either a regular Archimedean translation action, an order two-transitive action, or a periodic action. In the periodic case a fixed-point-free order automorphism of the [Dedekind completion](set.md#dedekind-completion) commutes with the action and has cofinal and coinitial iterates; the point stabilizers act order two-transitively within period intervals. Only the regular case satisfies $|f||g|\le|g|^2|f|^2$ for every pair. In either other case, order two-transitivity on the whole chain or on a period interval supplies positive $a,b$ and $x<y<z<t$ with $xa=y$, $ya=z$, $xb=x$, $yb=t$, giving $xab=t>z=xb^2a^2$. The classification itself is a theorem, not a consequence of that witness calculation.

#### Holland representation theorem

↑ **Parent:** [Lattice-ordered permutation group](#lattice-ordered-permutation-group)

Every [lattice-ordered group](#lattice-ordered-group) embeds in a [lattice-ordered permutation group](#lattice-ordered-permutation-group) on one [totally ordered set](set.md#totally-ordered-set). Choose a [value in a lattice-ordered group](#value-in-a-lattice-ordered-group) for each nonidentity element, act on its ordered right cosets, and combine these chains in an [order sum](set.md#order-sum). The original element moves its own value's identity coset, making the action faithful. The coset lattice formulas make the embedding preserve both [join](set.md#least-upper-bound-in-a-partially-ordered-set) and [meet](set.md#greatest-lower-bound-in-a-partially-ordered-set).

#### Order n-transitivity

↑ **Parent:** [Lattice-ordered permutation group](#lattice-ordered-permutation-group)

An ordered [permutation group](finite-group-theory.md#permutation-group) is order n-transitive if it can send any increasing $n$-tuple to any other increasing $n$-tuple. This compares tuples with the same relative order, unlike unrestricted [n-transitive group actions](group-theory.md#n-transitive-group-action). In the usual transitive chain setting, order two-transitivity implies every finite order-transitivity for a [lattice-ordered permutation group](#lattice-ordered-permutation-group).

##### Finite interpolation by lattice operations

↑ **Parent:** [Order n-transitivity](#order-n-transitivity)

Suppose $h_{ij}$ sends the $i$th and $j$th nodes of an increasing input tuple to the corresponding output nodes. At the $i$th input, every $h_{ij}$ agrees, so their pointwise [minimum](set.md#minimum-of-a-subset-of-a-total-order) takes the required value. At every other input it is bounded above by the required value, using the corresponding $j$ term. The pointwise [maximum](set.md#maximum-of-a-subset-of-a-total-order) over $i$ therefore interpolates the entire tuple. The construction uses closure under finite [join](set.md#least-upper-bound-in-a-partially-ordered-set) and [meet](set.md#greatest-lower-bound-in-a-partially-ordered-set), without assuming arbitrary restrictions of group elements belong to the group.

#### Positive bump of an order automorphism

↑ **Parent:** [Lattice-ordered permutation group](#lattice-ordered-permutation-group)

A positive bump of the real line is an [order automorphism](set.md#order-automorphism) whose nonempty [support of a permutation](finite-group-theory.md#support-of-a-permutation) is one open interval and which moves every point of that interval to the right. It fixes the complement. Iterating any interior point tends to the right endpoint in positive time and to the left endpoint in negative time.

##### Conjugacy of positive real-line bumps

↑ **Parent:** [Positive bump of an order automorphism](#positive-bump-of-an-order-automorphism)

Choose fundamental intervals $[x,xf)$ and $[y,yg)$ for two [positive bumps of an order automorphism](#positive-bump-of-an-order-automorphism). Any increasing bijection matching their endpoints extends by $b(xf^n)=(xb)g^n$ to their support intervals. Extend it monotonically over the two complementary rays. Then $fb=bg$, so $b^{-1}fb=g$. Bounded supports impose no further invariant for positive bumps in the full real-line order-automorphism group.

###### Conjugating positive bumps while preserving a fundamental interval

↑ **Parent:** [Conjugacy of positive real-line bumps](#conjugacy-of-positive-real-line-bumps)

If two [positive bumps of an order automorphism](#positive-bump-of-an-order-automorphism) move a point $c$ beyond an interval $[c,d]$, their [conjugacy](group-theory.md#conjugate-group-elements) can be chosen to fix that interval: begin with the identity there, complete the increasing map between fundamental intervals, and extend equivariantly along bump iterates. If both bump supports lie in one fundamental interval of another positive motion $h$, fix that cell's endpoints and repeat the conjugator on all its $h$-translates. The result commutes with $h$, and with any automorphism supported in the interval fixed pointwise.

## ↑ Ancestors (6)

1. [Group](group.md)
2. [Group theory](group-theory.md)
3. [Algebra](algebra.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)
