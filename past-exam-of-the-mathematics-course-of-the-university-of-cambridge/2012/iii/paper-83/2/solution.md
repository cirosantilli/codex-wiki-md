<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

We work in the ambient theory [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md) for this question. Write $t(x)=\operatorname{TC}(\{x\})$, using the [transitive closure](../../../../../transitive-closure.md) convention that $t(x)$ contains $x$ and all its membership descendants.

**First construct a set containing exactly the intended objects.** If $t(x)$ is a [countable set](../../../../../countable-set.md), apply [well-founded induction](../../../../../well-founded-induction.md) to membership on this [transitive set](../../../../../transitive-set.md). If all members $z$ of $y\in t(x)$ have [countable](../../../../../countable-set.md) [set-theoretic rank](../../../../../rank-of-a-set.md), then

$$
\operatorname{rank}(y)=\sup_{z\in y}\bigl(\operatorname{rank}(z)+1\bigr)<\omega_1.
$$

Indeed $y\subseteq t(x)$ is [countable](../../../../../countable-set.md), and a [countable union of countable sets](../../../../../countable-union-of-countable-sets.md) is [countable](../../../../../countable-set.md) in [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md). The induction therefore gives $\operatorname{rank}(x)<\omega_1$. The collection

$$
C=\{x\in V_{\omega_1}:t(x)\text{ is countable}\}
$$

is now a genuine [set](../../../../../set-split.md) by the [axiom schema of separation](../../../../../axiom-schema-of-specification.md) inside the [cumulative hierarchy](../../../../../cumulative-hierarchy.md) level $V_{\omega_1}$, and it contains every [hereditarily countable set](../../../../../hereditarily-countable-set.md). It is a [transitive set](../../../../../transitive-set.md), since $y\in x$ implies $t(y)\subseteq t(x)$.

If $a$ is a [countable](../../../../../countable-set.md) subset of $C$, then

$$
t(a)\subseteq\{a\}\cup\bigcup_{x\in a}t(x).
$$

The right side is [countable](../../../../../countable-set.md), so $a\in C$. Thus $C$ has [countable-subset closure](../../../../../countable-subset-closure.md). This proves existence of a set with the required closure before taking any intersection.

To make the least-set argument precise, form the nonempty set

$$
\mathcal F=\{B\subseteq C:\text{every countable subset of }B\text{ belongs to }B\}.
$$

It is a subset of $\mathcal P(C)$ and contains $C$. Its [intersection](../../../../../set-intersection.md) $H=\bigcap\mathcal F$ is also closed: a [countable](../../../../../countable-set.md) subset of $H$ is a [countable](../../../../../countable-set.md) subset of every $B\in\mathcal F$ and therefore belongs to each such $B$. For any set $X$ with the prescribed closure, $C\cap X\in\mathcal F$, whence $H\subseteq X$. This is leastness among all such sets, not just among subsets of $C$.

Finally, [well-founded induction](../../../../../well-founded-induction.md) on $C$ shows $C\subseteq X$ for every such $X$: when all members of $x\in C$ are in $X$, the [countable](../../../../../countable-set.md) set $x$ is a [countable](../../../../../countable-set.md) subset of $X$, so $x\in X$. Hence $H=C$, proving that the definition gives precisely

$$
\boxed{HC=\{x:\operatorname{TC}(\{x\})\text{ is countable}\}.}
$$

**For the cardinal bound, code the entire [countable](../../../../../countable-set.md) membership ancestry.** A code is a triple $(D,R,n)$, where $D\subseteq\omega$, $R\subseteq D^2$ is a [well-founded relation](../../../../../well-founded-relation.md) and an [extensional relation](../../../../../extensional-relation.md), and $n\in D$ is distinguished. There are at most $2^{\aleph_0}$ such codes: $D$ and $R$ are coded by subsets of [countable](../../../../../countable-set.md) sets, and a [Cantor pairing function](../../../../../cantor-pairing-function.md) with finitely many tags codes the triple as a subset of $\omega$.

The [well-founded recursion](../../../../../well-founded-recursion.md)

$$
c_R(k)=\{c_R(l):lRk\}
$$

defines its collapse, as in the [Mostowski collapse theorem](../../../../../mostowski-collapse-theorem.md). The range $\{c_R(k):k\in D\}$ is [countable](../../../../../countable-set.md) and transitive; thus each decoded $c_R(n)$ belongs to $HC$. Conversely, for $x\in HC$, choose a [bijection](../../../../../bijection.md) $e:D\to t(x)$ and the point $n$ with $e(n)=x$. Set $lRk$ exactly when $e(l)\in e(k)$. Transitivity of $t(x)$ makes this relation extensional, and [Axiom of foundation](../../../../../axiom-of-regularity.md) makes it well-founded. The recursion then gives $c_R(k)=e(k)$, so this code decodes to $x$.

We have a [surjection](../../../../../surjective-function.md) from a set of at most continuum many codes onto $HC$. Using the permitted [axiom of choice](../../../../../axiom-of-choice.md), well-order the codes and assign each $x$ its least code; this is an [injection](../../../../../injective-function.md). In fact every subset of $\omega$ is hereditarily [countable](../../../../../countable-set.md), giving the reverse bound as well:

$$
\boxed{|HC|=2^{\aleph_0},\quad\text{in particular }|HC|\le 2^{\aleph_0}.}
$$

Every member has rank below $\omega_1$, while every [countable](../../../../../countable-set.md) [ordinal](../../../../../ordinal.md) $\alpha$ belongs to $HC$ and has rank $\alpha$. Consequently

$$
\boxed{\operatorname{rank}(HC)=\omega_1.}
$$

**The axioms hold except Power Set.** [axiom of extensionality](../../../../../axiom-of-extensionality.md) and [Axiom of foundation](../../../../../axiom-of-regularity.md) are inherited by this transitive structure. The empty set and $\omega$ belong to it, giving the empty-set axiom and the [axiom of infinity](../../../../../axiom-of-infinity.md). The [axiom of pairing](../../../../../axiom-of-pairing.md) follows from [countable](../../../../../countable-set.md)-subset closure. For $a\in HC$, $\bigcup a$ is a [countable](../../../../../countable-set.md) subset of $HC$, giving the [Axiom of union](../../../../../axiom-of-union.md). Any subset of $a$ is [countable](../../../../../countable-set.md) and lies in $HC$, so the [axiom schema of separation](../../../../../axiom-schema-of-specification.md) holds for all formulas interpreted in $(HC,\in)$.

For the [Axiom schema of replacement](../../../../../axiom-schema-of-replacement.md), let a formula interpreted in $(HC,\in)$ assign a unique $y\in HC$ to each $x\in a\in HC$. Relativize that formula to the set $HC$ and use the ambient [Axiom schema of replacement](../../../../../axiom-schema-of-replacement.md) to collect its range. The range is [countable](../../../../../countable-set.md) and consists of members of $HC$, hence belongs to $HC$. The same argument, selecting one witness for each member of the [countable](../../../../../countable-set.md) domain, proves [axiom schema of collection](../../../../../axiom-schema-of-collection.md). An ambient choice function on a family $a\in HC$ has a [countable](../../../../../countable-set.md) graph of ordered pairs of hereditarily [countable](../../../../../countable-set.md) sets. Each such pair is in $HC$, and [countable](../../../../../countable-set.md)-subset closure puts the graph in $HC$, proving the internal [axiom of choice](../../../../../axiom-of-choice.md).

However, all external subsets of $\omega$ are elements of $HC$. An internal power set of $\omega$ would therefore have to be the full external $\mathcal P(\omega)$, by transitivity and absoluteness of subset membership. That is [uncountable](../../../../../uncountable-set.md) by [Cantor's theorem](../../../../../cantor-s-theorem.md), whereas every member of $HC$ is [countable](../../../../../countable-set.md). Thus the [axioms satisfied by hereditarily countable sets](../../../../../axioms-satisfied-by-hereditarily-countable-sets.md) are

$$
\boxed{HC\models\mathrm{ZFC}\text{ with Power Set deleted},\qquad
HC\not\models\mathrm{Power\ Set}.}
$$

Here the asserted axiom list includes both [Axiom schema of replacement](../../../../../axiom-schema-of-replacement.md) and [axiom schema of collection](../../../../../axiom-schema-of-collection.md); no equivalence relying on Power Set is being silently invoked.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 83](../../paper-83-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
