<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

A [transitive class](../../../../../transitive-class.md) $M$ satisfies $x\in M\Rightarrow x\subseteq M$. Its membership structure therefore does not omit elements of its members. In particular bounded membership statements are absolute between a transitive model and the ambient universe, and its membership relation is the actual well-founded relation, rather than an arbitrary externally ill-founded coding.

For a set $x$, put $x_0=x$ and $x_{n+1}=\bigcup x_n$, and define

$$
\boxed{\operatorname{TC}(x)=\bigcup_{n<\omega}x_n.}
$$

This is a set, contains $x$ as a subset, and is transitive: an element of an element of $x_n$ belongs to $x_{n+1}$. Any transitive set containing $x$ as a subset contains every $x_n$ by induction, so this construction is the least such set. Shifting the union index gives

$$
\boxed{\operatorname{TC}(x)=x\cup\operatorname{TC}(\bigcup x),\qquad
\operatorname{TC}(\{x\})=\{x\}\cup\operatorname{TC}(x).}
$$

These formulas use the specified subset convention for [transitive closure](../../../../../transitive-closure.md).

Work in the usual ambient set theory with Choice. If $x$ is a [hereditarily countable set](../../../../../hereditarily-countable-set.md), then every member of $\operatorname{TC}(\{x\})$ is countable. Iterated countable unions show that this entire closure is countable. Conversely a countable [transitive closure](../../../../../transitive-closure.md) makes each of its members countable. This equivalent criterion makes the following closure arguments explicit.

If $y\in x\in\mathrm{HC}$, then $\operatorname{TC}(\{y\})\subseteq\operatorname{TC}(\{x\})$, so $y\in\mathrm{HC}$: **HC is transitive**. If $x\in\mathrm{HC}$, its union is countable and its descendant sets are descendants of $x$, so $\bigcup x\in\mathrm{HC}$. The actual union therefore witnesses the [Axiom of union](../../../../../axiom-of-union.md) inside $(\mathrm{HC},\in)$.

For [axiom schema of separation](../../../../../axiom-schema-of-specification.md), take any formula with parameters in HC and a set $x\in\mathrm{HC}$. Form the subset of $x$ consisting of the elements that satisfy that formula with all quantifiers relativized to HC. Ambient Separation supplies this set. It is a subset of a [countable set](../../../../../countable-set.md), and all its descendants are inherited from $x$, so it belongs to HC. No claim that the formula itself is absolute is needed.

The [axioms satisfied by hereditarily countable sets](../../../../../axioms-satisfied-by-hereditarily-countable-sets.md) also include Extensionality, Empty Set, Pairing, Infinity, Foundation and Replacement. Extensionality and Foundation follow from transitivity and ambient well-foundedness. Empty Set and $\omega$ belong to HC, and a pair of HC sets has countable [transitive closure](../../../../../transitive-closure.md). For Replacement, the domain is countable; a definable image of its elements is a countable family of HC sets, whose combined transitive closures form a countable union of [countable sets](../../../../../countable-set.md), so the range again belongs to HC. Ambient Choice additionally gives Choice internally: a well-order of a countable HC set has a hereditarily countable relation and hence lies in HC.

**Power Set fails.** Every subset of $\omega$ is hereditarily countable, so an internal power-set witness would have to contain all ambient subsets of $\omega$. That collection is uncountable by [Cantor theorem](../../../../../cantor-s-theorem.md), whereas every HC set is countable. Thus HC satisfies the other ZF axioms and, in this ambient setting, Choice, but not the [Axiom of power set](../../../../../axiom-of-power-set.md).

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
