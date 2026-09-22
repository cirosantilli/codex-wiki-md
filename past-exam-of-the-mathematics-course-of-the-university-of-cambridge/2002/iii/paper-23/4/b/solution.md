<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An [atomic model](../../../../../../atomic-model.md) is a model in which every finite tuple's [complete type](../../../../../../complete-type.md) over the empty set is isolated by a formula. An [omega-saturated model](../../../../../../omega-saturated-model.md) realizes every [complete type](../../../../../../complete-type.md) in finitely many variables over every finite parameter set; equivalently it realizes all one-variable types over finite parameter sets, then successive realizations give the finite-tuple version.

Suppose $M$ is countable and omega-saturated. Every type in $S_n(T)$ is realized by a tuple in $M$, so $S_n(T)$ is countable. This is a compact Hausdorff [Stone space](../../../../../../stone-space.md) with a clopen basis. Its isolated points are dense. Indeed, if a nonempty clopen subset had no isolated point, split it into two disjoint nonempty clopen subsets and recursively split every resulting subset. Such splits exist because each subset has at least two points and the space is zero-dimensional. Compactness supplies a point in each nested sequence along an infinite binary branch, while disjoint siblings make different branches yield different points. This would give uncountably many points, contradicting countability.

For each $n$, let $\Gamma_n(\mathbf x)$ consist of the negations of all formulas that isolate complete $n$-types. Density of [isolated types](../../../../../../isolated-type.md) means that every consistent formula has a consistent refinement to an isolating formula $\delta$; this refinement excludes the member $\neg\delta$ of $\Gamma_n$. Thus $T$ locally omits every $\Gamma_n$. The [omitting types theorem](../../../../../../omitting-types-theorem.md) gives a countable model $A$ omitting them all. Every tuple in $A$ therefore satisfies some isolating formula, so **$A$ is atomic**. If some $\Gamma_n$ is itself inconsistent, its omission is automatic and does not obstruct this argument.

The converse about existence is **false**. Here is a [countable atomic model without a countable saturated model](../../../../../../countable-atomic-model-without-a-countable-saturated-model.md). Take a countable set $M$ with unary predicates $P_i$, $i\in\mathbb N$, such that every finite Boolean pattern of the predicates occurs infinitely often. For example, use finite binary words paired with a natural number, with $P_i$ recording the $i$th bit when it exists and false otherwise. Add a constant naming each element, and put $T=\operatorname{Th}(M)$ in this countable language. Every tuple of $M$ has its type isolated by equations to its named coordinates, so $M$ is a countable [atomic model](../../../../../../atomic-model.md).

For each infinite binary sequence $\eta$, the family

$$
\{x\ne c_a:a\in M\}\cup
\{P_i(x):\eta_i=1\}\cup\{\neg P_i(x):\eta_i=0\}
$$

is finitely satisfiable in $M$: realize its finitely many predicate requirements while avoiding finitely many named elements. By [compactness theorem](../../../../../../compactness-theorem.md), it extends to a complete one-type. Different sequences give different types, so $S_1(T)$ is uncountable. Any [omega-saturated model](../../../../../../omega-saturated-model.md) must realize all these empty-parameter types, which a countable model cannot do. This disproves the existence converse, rather than merely exhibiting an [atomic model](../../../../../../atomic-model.md) that is itself nonsaturated.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
