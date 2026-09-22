<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The countable form of the [omitting types theorem](../../../../../omitting-types-theorem.md) is as follows. Let $L$ be a countable [first-order language](../../../../../first-order-language.md) and $T$ a consistent [first-order theory](../../../../../first-order-theory.md) in $L$. For any countable family $p_0,p_1,\ldots$ of [nonprincipal partial types](../../../../../nonprincipal-partial-type.md) in finite tuples of variables, there is an at most countable [first-order model](../../../../../model-of-a-first-order-theory.md) of $T$ omitting all of them. Nonprincipality means that no $T$-consistent [first-order formula](../../../../../first-order-formula.md) $\theta(\mathbf x)$ entails every member of the type modulo $T$. A complete [first-order theory](../../../../../first-order-theory.md) with nonisolated [complete types](../../../../../complete-type.md) is the usual special case; neither an uncountable language nor an arbitrary uncountable family is covered by this statement.

Use the [Godel completeness theorem](../../../../../godel-s-completeness-theorem.md) to pass between consistency and the existence of a [first-order model](../../../../../model-of-a-first-order-theory.md). Adjoin a countable stock $C$ of new constants. Construct finite conditions $\Gamma_s$ with $T\cup\Gamma_s$ consistent, interleaving three countable lists of requirements: decide each $L(C)$-sentence; provide a fresh constant witness for each existential sentence; and, for each $p_i$ and each tuple $\mathbf t$ of closed terms of its arity, add $\neg\psi(\mathbf t)$ for some $\psi\in p_i$. Sentence decisions preserve consistency by choosing a consistent sign. For an existential sentence $\exists x\,\varphi(x)$, add $\exists x\,\varphi(x)\to\varphi(c)$ with $c$ fresh for that condition and [first-order formula](../../../../../first-order-formula.md). This is consistent: any [first-order model](../../../../../model-of-a-first-order-theory.md) of the old condition can interpret $c$ as a witness if one exists, and otherwise arbitrarily in the nonempty domain.

The omission step is the key [Henkin omission extension lemma](../../../../../henkin-omission-extension-lemma.md). Let $\sigma(\mathbf c)$ be the [logical conjunction](../../../../../logical-conjunction.md) of the current finite condition, listing every new constant occurring either there or in $\mathbf t$. If adding $\neg\psi(\mathbf t)$ were inconsistent for every $\psi\in p_i$, then $T$ would entail $\sigma(\mathbf c)\to\psi(\mathbf t(\mathbf c))$ for each such $\psi$. Replace the new constants by fresh variables $\mathbf z$ and form

$$
\theta(\mathbf x)=\exists\mathbf z\bigl(\sigma(\mathbf z)\land\bigwedge_j x_j=t_j(\mathbf z)\bigr).
$$

It is consistent with $T$ and entails every $\psi\in p_i$, contradicting nonprincipality. Hence some omission extension is consistent. The construction need not be computable; countability merely permits all these requirements to be scheduled.

Let $T^*$ be the deductive closure of $T\cup\bigcup_s\Gamma_s$. It is consistent by the [finite character of formal proofs](../../../../../finite-character-of-formal-proofs.md), complete by sentence decisions, and has the [Henkin witness property](../../../../../henkin-witness-property.md). Its [term model](../../../../../term-model.md) consists of closed terms modulo provable [logical equality](../../../../../logical-equality.md) and has at most countably many elements. The [truth lemma for a Henkin term model](../../../../../truth-lemma-for-a-henkin-term-model.md) proves that it is a [first-order model](../../../../../model-of-a-first-order-theory.md) of $T^*$. Every tuple in it is represented by closed terms, whose scheduled omission requirement supplies a negated member of each corresponding type. Thus

$$
\boxed{\text{there is an at most countable }M\models T\text{ omitting every }p_i.}
$$

A [universal sentence](../../../../../universal-sentence.md) has the form $\forall\mathbf x\,\psi(\mathbf x)$ with quantifier-free $\psi$, including an empty quantifier block. Embeddings preserve and reflect quantifier-free truth, so [universal sentences](../../../../../universal-sentence.md) pass to [substructures of a first-order structure](../../../../../substructure-of-a-first-order-structure.md). For the converse [Łoś-Tarski preservation theorem](../../../../../los-tarski-preservation-theorem.md), let $T_\forall$ be all universal consequences of an arbitrary [first-order theory](../../../../../first-order-theory.md) $T$, and take $A\models T_\forall$. We claim $T\cup\operatorname{Diag}(A)$ is consistent, where the [diagram of a structure](../../../../../diagram-mathematical-logic.md) contains both atomic and negated atomic sentences in constants naming the elements of $A$.

If inconsistent, the [compactness theorem](../../../../../compactness-theorem.md) gives a finite [logical conjunction](../../../../../logical-conjunction.md) $\delta(c_{a_1},\ldots,c_{a_r})$ of diagram sentences for which $T\models\neg\delta(c_{a_1},\ldots,c_{a_r})$. The added constants do not occur in $T$, so

$$
T\models\forall x_1\cdots x_r\,\neg\delta(x_1,\ldots,x_r).
$$

This [universal sentence](../../../../../universal-sentence.md) belongs to $T_\forall$ but is false in $A$ at the named tuple, a contradiction. The [compactness theorem](../../../../../compactness-theorem.md) therefore produces $B\models T$ containing an isomorphic embedded copy of $A$. The signed diagram ensures a genuine [substructure of a first-order structure](../../../../../substructure-of-a-first-order-structure.md): [functions](../../../../../function-split.md) are preserved, constants are included and relations are preserved and reflected. If the [first-order model](../../../../../model-of-a-first-order-theory.md) class of $T$ is closed under [substructures of a first-order structure](../../../../../substructure-of-a-first-order-structure.md), this copy, and hence $A$, is a [first-order model](../../../../../model-of-a-first-order-theory.md) of $T$. We have proved

$$
\boxed{\operatorname{Mod}(T)=\operatorname{Mod}(T_\forall).}
$$

No countability assumption is needed for this second argument. An inconsistent [first-order theory](../../../../../first-order-theory.md) is covered as well, with a universally false axiom and an empty [first-order model](../../../../../model-of-a-first-order-theory.md) class.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 135](../../paper-135-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
