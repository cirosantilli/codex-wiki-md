# Paper 83

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_83.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_83.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 83](paper-83.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Here the [power set](../../../set.md#power-set) notation gives $xEy\iff\mathcal P(x)\subseteq y$. Suppose a nonempty [set](../../../set.md) $A$ has no $E$-minimal member. Form its [intersection](../../../set.md#set-intersection) $b=\bigcap A$. This is a set: for any one $a_0\in A$, use the [axiom schema of separation](../../../set-theory.md#axiom-schema-of-specification) inside $a_0$ to define the elements common to all members of $A$. Selecting a single witness to nonemptiness is not an application of the [axiom of choice](../../../set-theory.md#axiom-of-choice).

For an arbitrary $y\in A$, lack of minimality supplies some $x\in A$ with $\mathcal P(x)\subseteq y$. Since $b\subseteq x$, every [subset](../../../set.md#subset) of $b$ is a subset of $x$, so

$$
\mathcal P(b)\subseteq\mathcal P(x)\subseteq y.
$$

This conclusion holds for each $y\in A$, without choosing all the corresponding $x$ simultaneously. Intersecting over $y$ gives $\mathcal P(b)\subseteq b$.

For completeness, the contradiction in [Cantor's theorem](../../../set.md#cantor-s-theorem) is completely explicit here. By the [axiom schema of separation](../../../set-theory.md#axiom-schema-of-specification) put $d=\{u\in b:u\notin u\}$. Then $d\in\mathcal P(b)\subseteq b$, and consequently

$$
d\in d\quad\Longleftrightarrow\quad d\notin d,
$$

which is impossible. Thus no such $A$ exists:

$$
\boxed{E\text{ is well-founded, without Choice or Foundation}.}
$$

This [power-set-predecessor relation](../../../set-theory.md#power-set-predecessor-relation) proof uses neither a descending sequence nor a comparison of possibly non-well-orderable [cardinalities](../../../set-theory.md#cardinality). It proves [well-foundedness](../../../set-theory.md#well-founded-relation) directly from the minimal-member definition.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Order the collection $\operatorname{Ch}(P)$ of every [chain in a partial order](../../../set.md#chain-in-a-partial-order), including the empty chain, by inclusion. Suppose that $j:\operatorname{Ch}(P)\to P$ is an [order-preserving function](../../../set.md#order-preserving-function) and an [injection](../../../algebra.md#injective-function). Let $\theta=h(P)$ be the [Hartogs ordinal](../../../set-theory.md#hartogs-number): by [Hartogs theorem](../../../set-theory.md#hartogs-theorem), no [injection](../../../algebra.md#injective-function) from $\theta$ to $P$ exists.

Use [transfinite recursion](../../../set-theory.md#transfinite-recursion) to define, for $\alpha<\theta$,

$$
C_\alpha=\{p_\beta:\beta<\alpha\},\qquad p_\alpha=j(C_\alpha).
$$

We verify both that $j(C_\alpha)$ is defined and that the values are strictly increasing. Assume inductively that the earlier values are strictly increasing. Then $C_\alpha$ is a [chain in a partial order](../../../set.md#chain-in-a-partial-order). For any $\beta<\alpha$, $C_\beta\subseteq C_\alpha$, so the fact that $j$ is [order-preserving](../../../set.md#order-preserving-function) gives $p_\beta\le p_\alpha$. Furthermore $p_\beta\in C_\alpha$, whereas $p_\beta\notin C_\beta$ by distinctness of the earlier values. Thus $C_\beta\ne C_\alpha$, and [injectivity](../../../algebra.md#injective-function) gives $p_\beta\ne p_\alpha$. We have proved

$$
\beta<\alpha\quad\Longrightarrow\quad p_\beta<p_\alpha.
$$

The empty initial chain starts the induction, and the same argument applies at every [limit ordinal](../../../set-theory.md#limit-ordinal).

If a globally defined recursion rule is desired, apply $j$ when the earlier range is a chain and otherwise use the fixed value $j(\varnothing)$. The induction shows that the fallback case never occurs. Thus no choices of new points are being made: the [function](../../../function.md) $j$ uniquely determines every stage.

The resulting [function](../../../function.md) $\alpha\mapsto p_\alpha$ is an [injection](../../../algebra.md#injective-function) from $\theta$ to $P$, contrary to its defining [Hartogs ordinal](../../../set-theory.md#hartogs-number) property. Hence the [chain-poset nonembedding lemma](../../../set.md#chain-poset-nonembedding-lemma) gives

$$
\boxed{\text{No order-preserving injection }\operatorname{Ch}(P)\longrightarrow P\text{ exists}.}
$$

## 2

↑ **Parent:** [Paper 83](paper-83.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

We work in the ambient theory [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice) for this question. Write $t(x)=\operatorname{TC}(\{x\})$, using the [transitive closure](../../../set-theory.md#transitive-closure) convention that $t(x)$ contains $x$ and all its membership descendants.

**First construct a set containing exactly the intended objects.** If $t(x)$ is a [countable set](../../../set-theory.md#countable-set), apply [well-founded induction](../../../set-theory.md#well-founded-induction) to membership on this [transitive set](../../../set-theory.md#transitive-set). If all members $z$ of $y\in t(x)$ have [countable](../../../set-theory.md#countable-set) [set-theoretic rank](../../../set-theory.md#rank-of-a-set), then

$$
\operatorname{rank}(y)=\sup_{z\in y}\bigl(\operatorname{rank}(z)+1\bigr)<\omega_1.
$$

Indeed $y\subseteq t(x)$ is [countable](../../../set-theory.md#countable-set), and a [countable union of countable sets](../../../set-theory.md#countable-union-of-countable-sets) is [countable](../../../set-theory.md#countable-set) in [ZFC](../../../set-theory.md#zermelo-fraenkel-set-theory-with-choice). The induction therefore gives $\operatorname{rank}(x)<\omega_1$. The collection

$$
C=\{x\in V_{\omega_1}:t(x)\text{ is countable}\}
$$

is now a genuine [set](../../../set.md) by the [axiom schema of separation](../../../set-theory.md#axiom-schema-of-specification) inside the [cumulative hierarchy](../../../set-theory.md#cumulative-hierarchy) level $V_{\omega_1}$, and it contains every [hereditarily countable set](../../../set-theory.md#hereditarily-countable-set). It is a [transitive set](../../../set-theory.md#transitive-set), since $y\in x$ implies $t(y)\subseteq t(x)$.

If $a$ is a [countable](../../../set-theory.md#countable-set) subset of $C$, then

$$
t(a)\subseteq\{a\}\cup\bigcup_{x\in a}t(x).
$$

The right side is [countable](../../../set-theory.md#countable-set), so $a\in C$. Thus $C$ has [countable-subset closure](../../../set-theory.md#countable-subset-closure). This proves existence of a set with the required closure before taking any intersection.

To make the least-set argument precise, form the nonempty set

$$
\mathcal F=\{B\subseteq C:\text{every countable subset of }B\text{ belongs to }B\}.
$$

It is a subset of $\mathcal P(C)$ and contains $C$. Its [intersection](../../../set.md#set-intersection) $H=\bigcap\mathcal F$ is also closed: a [countable](../../../set-theory.md#countable-set) subset of $H$ is a [countable](../../../set-theory.md#countable-set) subset of every $B\in\mathcal F$ and therefore belongs to each such $B$. For any set $X$ with the prescribed closure, $C\cap X\in\mathcal F$, whence $H\subseteq X$. This is leastness among all such sets, not just among subsets of $C$.

Finally, [well-founded induction](../../../set-theory.md#well-founded-induction) on $C$ shows $C\subseteq X$ for every such $X$: when all members of $x\in C$ are in $X$, the [countable](../../../set-theory.md#countable-set) set $x$ is a [countable](../../../set-theory.md#countable-set) subset of $X$, so $x\in X$. Hence $H=C$, proving that the definition gives precisely

$$
\boxed{HC=\{x:\operatorname{TC}(\{x\})\text{ is countable}\}.}
$$

**For the cardinal bound, code the entire [countable](../../../set-theory.md#countable-set) membership ancestry.** A code is a triple $(D,R,n)$, where $D\subseteq\omega$, $R\subseteq D^2$ is a [well-founded relation](../../../set-theory.md#well-founded-relation) and an [extensional relation](../../../set-theory.md#extensional-relation), and $n\in D$ is distinguished. There are at most $2^{\aleph_0}$ such codes: $D$ and $R$ are coded by subsets of [countable](../../../set-theory.md#countable-set) sets, and a [Cantor pairing function](../../../set-theory.md#cantor-pairing-function) with finitely many tags codes the triple as a subset of $\omega$.

The [well-founded recursion](../../../set-theory.md#well-founded-recursion)

$$
c_R(k)=\{c_R(l):lRk\}
$$

defines its collapse, as in the [Mostowski collapse theorem](../../../set-theory.md#mostowski-collapse-theorem). The range $\{c_R(k):k\in D\}$ is [countable](../../../set-theory.md#countable-set) and transitive; thus each decoded $c_R(n)$ belongs to $HC$. Conversely, for $x\in HC$, choose a [bijection](../../../function.md#bijection) $e:D\to t(x)$ and the point $n$ with $e(n)=x$. Set $lRk$ exactly when $e(l)\in e(k)$. Transitivity of $t(x)$ makes this relation extensional, and [Axiom of foundation](../../../set-theory.md#axiom-of-regularity) makes it well-founded. The recursion then gives $c_R(k)=e(k)$, so this code decodes to $x$.

We have a [surjection](../../../algebra.md#surjective-function) from a set of at most continuum many codes onto $HC$. Using the permitted [axiom of choice](../../../set-theory.md#axiom-of-choice), well-order the codes and assign each $x$ its least code; this is an [injection](../../../algebra.md#injective-function). In fact every subset of $\omega$ is hereditarily [countable](../../../set-theory.md#countable-set), giving the reverse bound as well:

$$
\boxed{|HC|=2^{\aleph_0},\quad\text{in particular }|HC|\le 2^{\aleph_0}.}
$$

Every member has rank below $\omega_1$, while every [countable](../../../set-theory.md#countable-set) [ordinal](../../../set-theory.md#ordinal) $\alpha$ belongs to $HC$ and has rank $\alpha$. Consequently

$$
\boxed{\operatorname{rank}(HC)=\omega_1.}
$$

**The axioms hold except Power Set.** [axiom of extensionality](../../../set-theory.md#axiom-of-extensionality) and [Axiom of foundation](../../../set-theory.md#axiom-of-regularity) are inherited by this transitive structure. The empty set and $\omega$ belong to it, giving the empty-set axiom and the [axiom of infinity](../../../set-theory.md#axiom-of-infinity). The [axiom of pairing](../../../set-theory.md#axiom-of-pairing) follows from [countable](../../../set-theory.md#countable-set)-subset closure. For $a\in HC$, $\bigcup a$ is a [countable](../../../set-theory.md#countable-set) subset of $HC$, giving the [Axiom of union](../../../set-theory.md#axiom-of-union). Any subset of $a$ is [countable](../../../set-theory.md#countable-set) and lies in $HC$, so the [axiom schema of separation](../../../set-theory.md#axiom-schema-of-specification) holds for all formulas interpreted in $(HC,\in)$.

For the [Axiom schema of replacement](../../../set-theory.md#axiom-schema-of-replacement), let a formula interpreted in $(HC,\in)$ assign a unique $y\in HC$ to each $x\in a\in HC$. Relativize that formula to the set $HC$ and use the ambient [Axiom schema of replacement](../../../set-theory.md#axiom-schema-of-replacement) to collect its range. The range is [countable](../../../set-theory.md#countable-set) and consists of members of $HC$, hence belongs to $HC$. The same argument, selecting one witness for each member of the [countable](../../../set-theory.md#countable-set) domain, proves [axiom schema of collection](../../../set-theory.md#axiom-schema-of-collection). An ambient choice function on a family $a\in HC$ has a [countable](../../../set-theory.md#countable-set) graph of ordered pairs of hereditarily [countable](../../../set-theory.md#countable-set) sets. Each such pair is in $HC$, and [countable](../../../set-theory.md#countable-set)-subset closure puts the graph in $HC$, proving the internal [axiom of choice](../../../set-theory.md#axiom-of-choice).

However, all external subsets of $\omega$ are elements of $HC$. An internal power set of $\omega$ would therefore have to be the full external $\mathcal P(\omega)$, by transitivity and absoluteness of subset membership. That is [uncountable](../../../set-theory.md#uncountable-set) by [Cantor's theorem](../../../set.md#cantor-s-theorem), whereas every member of $HC$ is [countable](../../../set-theory.md#countable-set). Thus the [axioms satisfied by hereditarily countable sets](../../../set-theory.md#axioms-satisfied-by-hereditarily-countable-sets) are

$$
\boxed{HC\models\mathrm{ZFC}\text{ with Power Set deleted},\qquad
HC\not\models\mathrm{Power\ Set}.}
$$

Here the asserted axiom list includes both [Axiom schema of replacement](../../../set-theory.md#axiom-schema-of-replacement) and [axiom schema of collection](../../../set-theory.md#axiom-schema-of-collection); no equivalence relying on Power Set is being silently invoked.

## 3

↑ **Parent:** [Paper 83](paper-83.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Put $\kappa=|X|$, an infinite [cardinal number](../../../set-theory.md#cardinal-number). The original PDF has the double exponent $2^{2^{|X|}}$; the single-exponent expression in the TeX aid is a transcription error.

We explicitly construct an [independent family of subsets](../../../set-theory.md#independent-family-of-sets) with $2^\kappa$ members on a set of size $\kappa$. Let

$$
D=\{(s,H):s\in[\kappa]^{<\omega},\ H\subseteq\mathcal P(s)\}.
$$

For each finite $s$ there are finitely many possibilities for $H$. The collection of finite subsets of an infinite cardinal has size $\kappa$, so $|D|\le\kappa$; the points $(\{\xi\},\varnothing)$ give the reverse bound. Thus $|D|=\kappa$.

For every $B\subseteq\kappa$ define

$$
A_B=\{(s,H)\in D:B\cap s\in H\}.
$$

To verify independence, take distinct $B_1,\ldots,B_n$ and bits $\varepsilon_1,\ldots,\varepsilon_n$. For each pair $i<j$, choose a point of $B_i\mathbin{\triangle}B_j$ and let $s$ contain all these finitely many points. The traces $B_i\cap s$ are pairwise distinct. Set

$$
H=\{B_i\cap s:\varepsilon_i=1\}.
$$

Then $(s,H)\in A_{B_i}$ exactly for those $i$ with $\varepsilon_i=1$. Every finite Boolean pattern is therefore realized. The cases $n=0,1$ work by the same definition, allowing $s=\varnothing$. In particular the sets $A_B$ are all distinct, so the [finite-trace independent family construction](../../../set-theory.md#fichtenholz-kantorovich-independent-family) gives exactly $2^\kappa$ independent members.

For each [function](../../../function.md) $\varepsilon:\mathcal P(\kappa)\to\{0,1\}$, prescribe $A_B$ when $\varepsilon(B)=1$ and $D\setminus A_B$ when $\varepsilon(B)=0$. Independence gives the [finite intersection property](../../../topology.md#finite-intersection-property). Their finite intersections generate a proper [filter on a set](../../../set-theory.md#filter-set-theory): its members are the subsets of $D$ containing one of those intersections.

To extend this to an [ultrafilter](../../../set-theory.md#ultrafilter), order its proper filter extensions by inclusion. The union of a chain is again a proper filter, so [Zorn's lemma](../../../set-theory.md#zorn-s-lemma) supplies a maximal one, $U_\varepsilon$. If neither a subset $Y$ nor its complement belonged to this filter, adjoining $Y$ would still generate a proper filter: otherwise some existing member would be disjoint from $Y$ and force its complement into the filter already. Maximality therefore gives the ultrafilter dichotomy. Using the ambient [axiom of choice](../../../set-theory.md#axiom-of-choice), choose such an extension for every $\varepsilon$.

Distinct functions differ at some $B$. Their ultrafilters respectively contain $A_B$ and its complement, and cannot be equal. There are $2^{2^\kappa}$ such functions. Transporting the ultrafilters along a [bijection](../../../function.md#bijection) $D\to X$ proves the lower bound. The upper bound is immediate because every ultrafilter is a subset of $\mathcal P(X)$:

$$
2^{2^\kappa}\le|\operatorname{Ult}(X)|
\le|\mathcal P(\mathcal P(X))|=2^{2^\kappa}.
$$

Thus the [number of ultrafilters on an infinite set](../../../set-theory.md#number-of-ultrafilters-on-an-infinite-set) is

$$
\boxed{|\operatorname{Ult}(X)|=2^{2^{|X|}}.}
$$

## 4

↑ **Parent:** [Paper 83](paper-83.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The maximum is $2^{\aleph_1}$. We construct that many [aleph-one-like linear orders](../../../set.md#aleph-one-like-linear-order), whose proper initial segments are [countable](../../../set-theory.md#countable-set), and prove that they are nonisomorphic. As usual the rational-type requirement concerns nonempty proper initial segments; the empty segment occurs in every order.

Let $D$ be the [club set](../../../set-theory.md#club-set) of nonzero [limit ordinals](../../../set-theory.md#limit-ordinal) below $\omega_1$. For $S\subseteq D$, form the [order sum](../../../set.md#order-sum)

$$
L_S=\sum_{\alpha<\omega_1}B_\alpha,\qquad
B_\alpha=
\begin{cases}
1+\mathbb Q,&\alpha\in S,\\
\mathbb Q,&\alpha\notin S.
\end{cases}
$$

Here $1+\mathbb Q$ means a new least point followed by a copy of the [rational numbers](../../../number-theory.md#rational-number); distinct blocks are disjoint, and all points of an earlier block precede every point of a later one. Every block is [countable](../../../set-theory.md#countable-set), dense and has no greatest point. Since $0\notin S$, the full [total order](../../../set.md#total-order) has neither a least nor a greatest point. It has size $\aleph_1$.

The sum is dense: within a block use density, and for points in different blocks choose a larger point in the earlier block. If $I$ is a proper initial segment and $y\notin I$ lies in block $\alpha$, then $I$ is contained in the union of the blocks through $\alpha$. There are only countably many such blocks, each [countable](../../../set-theory.md#countable-set). Thus $I$ is [countable](../../../set-theory.md#countable-set), rather than an [uncountable](../../../set-theory.md#uncountable-set) interval in an aleph-one-dense order.

Every nonempty $I$ is dense and has no least point. If it has no greatest point either, the [back-and-forth method](../../../foundations-of-mathematics.md#back-and-forth-method) gives $I\cong\mathbb Q$: enumerate both orders, alternately include the least unused element from either enumeration in a finite partial [order isomorphism](../../../set.md#order-isomorphism), and choose its partner in the appropriate open interval. Density and absence of endpoints always supply a new partner. The union is a bijective order isomorphism. If $I$ has a greatest point, remove it, apply the same argument, and reattach it. Hence every nonempty proper initial segment is isomorphic to $\mathbb Q$ or $\mathbb Q+1$.

**The stationary information is recorded at the limit cuts.** Write

$$
F^S_\alpha=\bigcup_{\beta<\alpha}B_\beta.
$$

This is a continuous increasing [kappa-filtration](../../../set-theory.md#kappa-filtration) by [countable](../../../set-theory.md#countable-set) initial segments. At a limit $\delta$, the complement $L_S\setminus F^S_\delta$ has a least point exactly when $\delta\in S$.

Suppose $f:L_S\to L_T$ is an [order isomorphism](../../../set.md#order-isomorphism). Since each filtration stage is [countable](../../../set-theory.md#countable-set), its image under $f$ and the corresponding image under $f^{-1}$ are bounded in block index: the supremum of their [countable](../../../set-theory.md#countable-set) collection of [countable ordinals](../../../set-theory.md#countable-ordinal) remains below $\omega_1$. Choose $g(\alpha)<\omega_1$ so that

$$
f[F^S_\alpha]\subseteq F^T_{g(\alpha)},\qquad
f^{-1}[F^T_\alpha]\subseteq F^S_{g(\alpha)}.
$$

The set

$$
C=\{\delta\in D:(\forall\alpha<\delta)\ g(\alpha)<\delta\}
$$

is a [club set](../../../set-theory.md#club-set). To see unboundedness, start above any given ordinal and recursively choose $\gamma_{n+1}>\gamma_n$ larger than every $g(\alpha)$ for $\alpha\le\gamma_n$. The supremum of the [countable](../../../set-theory.md#countable-set) sequence remains below $\omega_1$ and belongs to $C$. Closure follows because below a limit of members of $C$, each fixed $\alpha$ lies below one of those members.

For $\delta\in C$, continuity of the filtrations gives both inclusions needed for

$$
f[F^S_\delta]=F^T_\delta.
$$

The isomorphism therefore preserves whether the complementary final segment has a least point. Consequently

$$
\delta\in S\quad\Longleftrightarrow\quad\delta\in T
\qquad(\delta\in C).
$$

This [club agreement of countable filtrations](../../../set-theory.md#club-agreement-of-countable-filtrations) proves the invariant: if $S\mathbin{\triangle}T$ is stationary, the orders cannot be isomorphic.

We also construct enough pairwise different stationary encodings. For each $\beta<\omega_1$, fix an [injection](../../../algebra.md#injective-function) $e_\beta:\beta\to\omega$, and set

$$
A_{\xi,n}=\{\beta\in D:\xi<\beta,\ e_\beta(\xi)=n\}.
$$

For fixed $\xi$, these sets partition the stationary tail $D\setminus(\xi+1)$. At least one $A_{\xi,n}$ is stationary: otherwise choose a club avoiding each one and intersect the countably many clubs to obtain a club avoiding the entire tail. The countable-intersection fact follows directly: above any starting point choose an increasing sequence, visiting each club infinitely often; its [countable](../../../set-theory.md#countable-set) supremum belongs to every club by closure. For each $\xi$ let $n(\xi)$ be the least such $n$. One value $n_*$ occurs for uncountably many $\xi$, since a [countable](../../../set-theory.md#countable-set) union of [countable](../../../set-theory.md#countable-set) sets is [countable](../../../set-theory.md#countable-set). For that fixed $n_*$ the cells are pairwise disjoint, by injectivity of $e_\beta$. Enumerating those cells gives

$$
(S_\eta:\eta<\omega_1),
$$

a family of pairwise disjoint stationary subsets of $D$. This is the explicit [Ulam matrix on omega-one](../../../set-theory.md#ulam-matrix-on-omega-one) proof of [disjoint stationary subsets of omega-one](../../../set-theory.md#disjoint-stationary-subsets-of-omega-one).

For $A\subseteq\omega_1$ put $S(A)=\bigcup_{\eta\in A}S_\eta$. If $A\ne A'$, their symmetric difference contains an entire $S_\eta$ and is stationary. The [stationary encoding in an aleph-one-like dense order](../../../set.md#stationary-encoding-in-an-aleph-one-like-dense-order) therefore produces $2^{\aleph_1}$ pairwise nonisomorphic orders $L_{S(A)}$.

Finally, on a fixed carrier of size $\aleph_1$, every total order is a subset of its Cartesian square. That square has size $\aleph_1$, so there are at most $2^{\aleph_1}$ possible relations. Thus

$$
\boxed{2^{\aleph_1}\text{ pairwise nonisomorphic orders, the maximum possible}.}
$$

## 5

↑ **Parent:** [Paper 83](paper-83.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

An [Aronszajn tree](../../../set.md#aronszajn-tree) is a [set-theoretic tree](../../../set.md#set-theoretic-tree) of height $\omega_1$, with [countable](../../../set-theory.md#countable-set) levels and no [uncountable](../../../set-theory.md#uncountable-set) [chain in a partial order](../../../set.md#chain-in-a-partial-order), equivalently no [cofinal branch](../../../set.md#cofinal-branch). The strict predecessors of a node are well-ordered, and its height is their [order type](../../../set-theory.md#order-type). **Such trees exist in ZFC**, as the following [rationally labelled Aronszajn tree construction](../../../set.md#rationally-labelled-aronszajn-tree-construction) shows.

We build [countable](../../../set-theory.md#countable-set) nonempty levels $T_\alpha$ for all $\alpha<\omega_1$. A node $t\in T_\alpha$ is a strictly increasing function $t:\alpha\to\mathbb Q\cap(0,1)$, and the tree order is proper initial-segment extension. Every restriction $t\upharpoonright\beta$ must lie in $T_\beta$. Give nonempty $t$ the rational label

$$
\ell(t)=\sup\operatorname{ran}(t)<1,
$$

and give the empty root label $0$. We require labels to increase strictly along the tree. We also maintain the [bounded rational extension property](../../../set.md#bounded-rational-extension-property):

$$
s\in T_\beta,\quad \beta<\alpha,\quad
\ell(s)<q<1,\ q\in\mathbb Q
\quad\Longrightarrow\quad
(\exists t\in T_\alpha)\ s\subset t,\ \ell(t)<q.
$$

Keeping room below every rational cap is what makes the limit step possible.

Start with $T_0=\{\varnothing\}$. At a successor stage, for every $s\in T_\alpha$ and every rational $r$ with $\ell(s)<r<1$, include

$$
s^\frown r=s\cup\{(\alpha,r)\}
$$

in $T_{\alpha+1}$. Its label is $r$, strictly larger than its predecessor's. This level is [countable](../../../set-theory.md#countable-set). To extend an earlier node below a prescribed cap $q$, first extend to $T_\alpha$ below $q$ by the inductive property, if necessary, then choose a new rational label between that label and $q$. Thus the extension property is preserved.

Now let $\lambda<\omega_1$ be a nonzero limit. The whole tree below $\lambda$ is [countable](../../../set-theory.md#countable-set). For each pair $(s,q)$ with $s\in T_\beta$, $\beta<\lambda$, and $\ell(s)<q<1$, construct one node at height $\lambda$ extending $s$ below $q$. There are only countably many such pairs.

Choose a rational $r$ with $\ell(s)<r<q$ and an increasing sequence

$$
\beta=\alpha_0<\alpha_1<\cdots<\lambda,\qquad
\sup_n\alpha_n=\lambda.
$$

Set $s_0=s$. Given $s_n\in T_{\alpha_n}$ with $\ell(s_n)<r$, set

$$
r_n=\frac{r+\max\{\ell(s_n),\,r-1/(n+1)\}}2.
$$

This is rational and satisfies $\max\{\ell(s_n),r-1/(n+1)\}<r_n<r$. The successor rule supplies $u_n=s_n^\frown r_n$ at height $\alpha_n+1$. If $\alpha_{n+1}=\alpha_n+1$, take $s_{n+1}=u_n$; otherwise use the already established extension property below $\lambda$ to extend $u_n$ to $s_{n+1}\in T_{\alpha_{n+1}}$ with label below $r$.

The union $t=\bigcup_n s_n$ has domain $\lambda$ and extends $s$. It is strictly increasing, and every shorter restriction is already in its prescribed level. All its values are below $r$, while it contains the values $r_n>r-1/(n+1)$. Hence

$$
\sup\operatorname{ran}(t)=r\in\mathbb Q,\qquad \ell(t)=r<q.
$$

Every predecessor's label is below the label of some $s_n$, and hence below $r$. Thus strict increase of labels survives at the limit. Include one such $t$ for each pair $(s,q)$ in $T_\lambda$, discarding duplicates. This gives a [countable](../../../set-theory.md#countable-set) level and preserves every bounded extension requirement. In particular applying it to the root makes the level nonempty. The choices here are permitted by the ambient [axiom of choice](../../../set-theory.md#axiom-of-choice); [transfinite recursion](../../../set-theory.md#transfinite-recursion) through the set $\omega_1$ completes the construction.

Put $T=\bigcup_{\alpha<\omega_1}T_\alpha$. A node of domain $\alpha$ has exactly the restrictions of domains $\beta<\alpha$ as predecessors, so its height is $\alpha$. Therefore $T$ has height $\omega_1$ and [countable](../../../set-theory.md#countable-set) levels. Since $\ell:T\to\mathbb Q$ is strictly increasing on comparable nodes, an [uncountable](../../../set-theory.md#uncountable-set) chain would inject into the [countable](../../../set-theory.md#countable-set) set $\mathbb Q$, which is impossible. Each label fiber is a [tree antichain](../../../set.md#tree-antichain), so the tree is even a [special Aronszajn tree](../../../set.md#special-aronszajn-tree):

$$
\boxed{\text{ZFC proves the existence of a special Aronszajn tree}.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
