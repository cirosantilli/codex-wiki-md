<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

[Forcing](../../../../../forcing-split.md) constructs new [first-order models](../../../../../model-of-a-first-order-theory.md) while controlling which ground-model properties survive. Fix a ground model $M$ and a [partially ordered set](../../../../../partially-ordered-set.md) $P\in M$, writing $q\leq p$ when $q$ is the stronger condition. A [generic filter](../../../../../generic-filter.md) is upward [closed](../../../../../closed-set.md), directed towards stronger conditions, and meets every ground-model [dense subset of a forcing order](../../../../../dense-subset-of-a-forcing-order.md). If $M$ is externally a [countable transitive model](../../../../../countable-transitive-model.md), enumerate its dense [subsets](../../../../../subset.md) and successively choose stronger conditions in them. The resulting filter is $M$-generic. External countability is crucial: this is not a claim that the ground model regards its own universe as [countable](../../../../../countable-set.md).

A [forcing name](../../../../../forcing-name.md) is built recursively from pairs $(\sigma,p)$ of earlier names and conditions. For a generic filter $G$, its [evaluation of a forcing name](../../../../../evaluation-of-a-forcing-name.md) is

$$
\tau_G=\{\sigma_G:(\sigma,p)\in\tau,\ p\in G\},\qquad
M[G]=\{\tau_G:\tau\in M\}.
$$

The [canonical forcing name](../../../../../canonical-forcing-name.md) $\check x=\{(\check y,1):y\in x\}$ evaluates to $x$, so $M\subseteq M[G]$. Recursive evaluation also proves transitivity. Name ranks bound the ranks of their evaluations, so an [ordinal](../../../../../ordinal.md) in the extension is below some ground [ordinal](../../../../../ordinal.md) and is already a ground [ordinal](../../../../../ordinal.md). Thus [forcing preserves ordinals](../../../../../forcing-preserves-ordinals.md).

The central link between syntax and generic interpretation is the [forcing theorem](../../../../../forcing-theorem.md). The relation $p\Vdash\varphi(\tau_1,\ldots,\tau_n)$ is definable in the ground model, and the [forcing truth lemma](../../../../../forcing-truth-lemma.md) says

$$
M[G]\models\varphi((\tau_1)_G,\ldots,(\tau_n)_G)
\quad\Longleftrightarrow\quad
(\exists p\in G)\ p\Vdash\varphi(\tau_1,\ldots,\tau_n).
$$

For an atomic membership assertion, densely many refinements must witness equality with a member-name whose associated condition is compatible with the refinement. Equality is obtained by recursive mutual inclusion of names. For [negation](../../../../../negation.md), $p\Vdash\neg\varphi$ means no stronger condition forces $\varphi$; for an [existential quantification](../../../../../existential-quantification.md), witnesses must be obtainable densely below $p$. Induction on name rank establishes the atomic clauses, and induction on formulas establishes definability and the truth lemma. The generic filter meets the relevant dense [sets](../../../../../set-split.md) at the existential step. An arbitrary semantic assertion about one chosen generic filter is insufficient: the definable relation must work uniformly for all generic interpretations.

This explains preservation of [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md). [Extensionality](../../../../../axiom-of-extensionality.md) and [foundation](../../../../../axiom-of-regularity.md) follow from transitivity; canonical names supply [infinity](../../../../../infinity.md). Pair and [union](../../../../../set-union.md) names give [pairing](../../../../../axiom-of-pairing.md) and [union](../../../../../set-union.md). For [separation](../../../../../axiom-schema-of-specification.md), restrict a name's members to conditions [forcing](../../../../../forcing-split.md) the defining formula. For [replacement](../../../../../axiom-schema-of-replacement.md), the definable [forcing](../../../../../forcing-split.md) relation lets ground [axiom schema of collection](../../../../../axiom-schema-of-collection.md) bound a [set](../../../../../set-split.md) of names for all possible witnesses to the unique outputs; evaluating their collected name gives the range. For [power set](../../../../../power-set.md), let $\tau$ name the given [set](../../../../../set-split.md) and let $D$ be the [set](../../../../../set-split.md) of its member-names. Every [subset](../../../../../subset.md) of $\tau_G$ has an equivalent name drawn from $\mathcal P(D\times P)$, by the truth lemma, so a ground [set](../../../../../set-split.md) of candidate names collects all its [subsets](../../../../../subset.md). Finally choose a ground [well-order](../../../../../well-order.md) of the relevant names; its evaluated image surjects onto the desired [set](../../../../../set-split.md), and choosing the first name for each value well-orders that [set](../../../../../set-split.md). This is why ordinary [forcing](../../../../../forcing-split.md) over a [choice](../../../../../axiom-of-choice.md) model preserves [choice](../../../../../axiom-of-choice.md).

For a concrete example, [Cohen forcing](../../../../../cohen-forcing.md) consists of finite partial [functions](../../../../../function-split.md) $\omega\to2$, ordered by extension. The generic [union](../../../../../set-union.md) $c=\bigcup G$ is total because deciding each coordinate is dense. For every ground real $x$, the [set](../../../../../set-split.md) of conditions disagreeing with $x$ somewhere is dense, so $c\ne x$. This construction changes the universe by adding a genuinely new real without changing its [ordinals](../../../../../ordinal.md).

The size and compatibility of conditions determine what else changes. With the [countable chain condition for forcing](../../../../../countable-chain-condition-for-forcing.md), an ordinal-valued name has only countably many possible values at each coordinate: take a maximal antichain deciding that value. Therefore the possible range of a name for a map with infinite ground domain of [cardinality](../../../../../cardinality.md) $\mu$ lies in a ground [set](../../../../../set-split.md) of size at most $\mu\cdot\aleph_0=\mu$. This prevents [cardinal](../../../../../cardinal-number.md) collapse and changes of uncountable regular [cofinalities](../../../../../cofinality.md). [Forcing](../../../../../forcing-split.md) by finite partial [functions](../../../../../function-split.md) $\lambda\times\omega\to2$ is ccc: the [delta-system lemma](../../../../../delta-system-lemma.md) thins any uncountable family of finite domains to a delta-system, and a further thinning makes their values agree on its finite root. Two remaining conditions are compatible. Distinct coordinates add distinct reals.

For example, start with [GCH](../../../../../generalized-continuum-hypothesis.md) and take $\lambda=\aleph_2$. This [forcing](../../../../../forcing-split.md) has size $\lambda$ and adds $\lambda$ distinct reals. A [nice name for a real](../../../../../nice-name-for-a-real.md) uses countably many antichains, and each antichain is [countable](../../../../../countable-set.md). The ground arithmetic $\lambda^{\aleph_0}=\lambda$ bounds the number of such names by $\lambda$. Hence

$$
\boxed{M[G]\models 2^{\aleph_0}=\aleph_2,}
$$

giving a relative-consistency example of the failure of [CH](../../../../../continuum-hypothesis.md). The ground [choice](../../../../../axiom-of-choice.md) of GCH is available through the [constructible universe](../../../../../constructible-universe.md); no claim that every starting model has this arithmetic is needed.

By contrast, [countably closed forcing](../../../../../countably-closed-forcing.md) adds no new [countable](../../../../../countable-set.md) [sequences](../../../../../sequence.md) of ground [ordinals](../../../../../ordinal.md). Given a name, recursively strengthen a condition to decide each coordinate, then take a lower bound of the descending [sequence](../../../../../sequence.md). That condition decides the entire [sequence](../../../../../sequence.md). Closure and chain conditions thus control different features; neither should be silently substituted for the other.

Further applications include changing [cofinalities](../../../../../cofinality.md), adding branches through trees, and constructing prescribed continuum patterns. If the aim is to violate [choice](../../../../../axiom-of-choice.md), an ordinary generic extension of a [choice](../../../../../axiom-of-choice.md) model will not do: one restricts to a suitable symmetric collection of names, checking the [axioms](../../../../../axiom.md) again. These examples also mark a limitation: [forcing](../../../../../forcing-split.md) proves relative consistency, not absolute consistency of the background theory. The countable-transitive-model picture gives a concrete semantic construction; the definable [forcing](../../../../../forcing-split.md) relation and Boolean-valued formulation supply the corresponding formal consistency arguments without asserting that a transitive ground model can be proved to exist.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
