<h1 id="14h/solution">Solution</h1>

↑ **Parent:** [14H](../14h.md)

[Zorn lemma](../../../../../zorn-s-lemma.md) states that a [partially ordered set](../../../../../partially-ordered-set.md) in which every [chain in a partially ordered set](../../../../../chain-in-a-partially-ordered-set.md) has an upper bound has a [maximal element](../../../../../maximal-element-of-a-partially-ordered-set.md). Include the empty [chain in a partially ordered set](../../../../../chain-in-a-partially-ordered-set.md), so the hypotheses imply that the [set](../../../../../set-split.md) $P$ is nonempty. Suppose there were no [maximal element](../../../../../maximal-element-of-a-partially-ordered-set.md). Every [chain in a partially ordered set](../../../../../chain-in-a-partially-ordered-set.md) $C$ has an upper bound $u$, and some $v>u$; therefore the [set](../../../../../set-split.md) of elements strictly above every member of $C$ is nonempty. The [axiom of choice](../../../../../axiom-of-choice.md) selects one such element $f(C)$ for each [chain in a partially ordered set](../../../../../chain-in-a-partially-ordered-set.md) (and an element of $P$ when $C$ is empty).

By [Hartogs theorem](../../../../../hartogs-theorem.md), there is an [ordinal](../../../../../ordinal.md) $\kappa$ which does not inject into $P$. [Transfinite recursion](../../../../../transfinite-recursion.md) defines $x_\alpha=f(\{x_\beta:\beta<\alpha\})$ for all $\alpha<\kappa$: previous elements form a strictly increasing [chain in a partially ordered set](../../../../../chain-in-a-partially-ordered-set.md), including at [limit ordinal](../../../../../limit-ordinal.md) stages. All $x_\alpha$ are distinct, giving the forbidden injection. This proves [Zorn lemma](../../../../../zorn-s-lemma.md); **the choice of $f$ is the use of the [axiom of choice](../../../../../axiom-of-choice.md)**.

Apply [Zorn lemma](../../../../../zorn-s-lemma.md) to [linearly independent](../../../../../linear-independence.md) [subsets](../../../../../subset.md) of $\mathbb R$ over $\mathbb Q$, ordered by inclusion. A [union](../../../../../set-union.md) along a [chain in a partially ordered set](../../../../../chain-in-a-partially-ordered-set.md) is [linearly independent](../../../../../linear-independence.md) because each finite linear relation occurs in one member of that [chain in a partially ordered set](../../../../../chain-in-a-partially-ordered-set.md). A maximal independent [set](../../../../../set-split.md) spans $\mathbb R$, since a [vector](../../../../../vector.md) outside its span could be adjoined. Thus **$\mathbb R$ has a Hamel [basis](../../../../../basis.md) over $\mathbb Q$**.

For a finite [basis](../../../../../basis.md), the [Steinitz exchange lemma](../../../../../steinitz-exchange-lemma.md) proves equality of [basis](../../../../../basis.md) sizes. This also rules out an infinite [basis](../../../../../basis.md) when a finite spanning [set](../../../../../set-split.md) exists: write each member of the finite spanning [set](../../../../../set-split.md) using finitely many elements of another [basis](../../../../../basis.md); their finite [union](../../../../../set-union.md) spans, and independence leaves no other [basis](../../../../../basis.md) elements. If a [basis](../../../../../basis.md) $B$ is infinite with [cardinality](../../../../../cardinality.md) $\lambda$, the finite-support description of every [vector](../../../../../vector.md) and countability of $\mathbb Q$ give

$$
 \lambda\leq|V|\leq\sum_{n<\omega}|B|^n|\mathbb Q|^n=\lambda.
$$

Here infinite [cardinal arithmetic](../../../../../cardinal-arithmetic.md) uses the [axiom of choice](../../../../../axiom-of-choice.md). Thus any infinite [basis](../../../../../basis.md) has [cardinality](../../../../../cardinality.md) $|V|$, proving **all [bases](../../../../../basis.md) have the same [cardinality](../../../../../cardinality.md)**. The zero space has its unique empty [basis](../../../../../basis.md).

## ↑ Ancestors (10)

1. [14H](../14h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
