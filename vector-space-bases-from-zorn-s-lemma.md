<h1 id="vector-space-bases-from-zorn-s-lemma">Vector space bases from Zorn's lemma</h1>

↑ **Parent:** [Zorn's lemma](zorn-s-lemma.md)

Every [vector space](vector-space-split.md) $V$ over a [field](field.md) $F$ has a [basis](basis.md), assuming the [axiom of choice](axiom-of-choice.md). More generally, any [linearly independent](linear-independence.md) [subset](subset.md) $A\subseteq V$ extends to a [basis](basis.md). This is an algebraic [Hamel basis](basis.md): each representation uses a finite [linear combination](linear-combination.md), even when the [basis](basis.md) is infinite.[Zorn’s Lemma and Some Applications, §4, pp. 18–19, Theorem 4.1 and Corollary 4.2](zorn%E2%80%99s-lemma-and-some-applications-by-keith-conrad.md)

Use the [poset](partially-ordered-set.md) of [linearly independent](linear-independence.md) [subsets](subset.md) containing $A$:

$$
\mathcal P_A=\{S\subseteq V:A\subseteq S,\ S\text{ is linearly independent over }F\},
\qquad S\leq T\Longleftrightarrow S\subseteq T.
$$

It is a [set](set-split.md), being a [subset](subset.md) of the [power set](power-set.md) of $V$, and is nonempty because $A\in\mathcal P_A$.

A short proof outline supplies both essential steps:
- For a nonempty [chain in a partial order](chain-in-a-partial-order.md) $\mathcal C\subseteq\mathcal P_A$, put $U=\bigcup_{S\in\mathcal C}S$. Any finite [linear relation](linear-relation.md) in $U$ lies in one member of $\mathcal C$: among finitely many containing members, one contains the rest. Its [linear independence](linear-independence.md) makes every [coefficient](coefficient.md) zero. Thus $U\in\mathcal P_A$ is an [upper bound](upper-bound-in-a-partially-ordered-set.md). For the empty [chain in a partial order](chain-in-a-partial-order.md), use $A$; its empty [union](set-union.md) need not contain $A$.
- [Zorn's lemma](zorn-s-lemma.md) gives a [maximal element](maximal-element-of-a-partially-ordered-set.md) $B$. If a [vector](vector.md) $v$ lies outside its [linear span](linear-span.md), then $B\cup\{v\}$ is [linearly independent](linear-independence.md): a [linear relation](linear-relation.md) with nonzero [coefficient](coefficient.md) on $v$ would express $v$ in that [linear span](linear-span.md). This contradicts maximality, so $B$ is a [spanning set](spanning-set.md) and hence a [basis](basis.md).[Zorn’s Lemma and Some Applications, §4, pp. 18–19, chain-union proof of Theorem 4.1 and extension argument of Corollary 4.2](zorn%E2%80%99s-lemma-and-some-applications-by-keith-conrad.md)

Taking $A=\varnothing$ proves existence, including $V=\{0\}$, whose [basis](basis.md) is the [empty set](empty-set.md). The [chain in a partial order](chain-in-a-partial-order.md) need not be indexed by the [natural numbers](natural-number.md): only the finitely many members needed for a particular [linear relation](linear-relation.md) are compared. An arbitrary [union](set-union.md) of [linearly independent](linear-independence.md) [sets](set-split.md) can fail: $\{v\}$ and $\{2v\}$ for a nonzero [vector](vector.md) over the [real numbers](real-number.md) are each [linearly independent](linear-independence.md), but their [union](set-union.md) is [linearly dependent](linear-dependence.md). The nesting of a [chain in a partial order](chain-in-a-partial-order.md) is what prevents this failure.

## ↑ Ancestors (6)

1. [Zorn's lemma](zorn-s-lemma.md)
2. [Set theory](set-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
