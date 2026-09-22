<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

We take $\mathbb N=\{1,2,\ldots\}$ and require the [common difference](../../../../../common-difference.md) of an [arithmetic progression](../../../../../arithmetic-progression.md) to be positive. An [ultrafilter](../../../../../ultrafilter.md) $\mathcal U$ is a proper [filter on a set](../../../../../filter-set-theory.md) deciding each [subset](../../../../../subset.md): exactly one of $B$ and $\mathbb N\setminus B$ belongs to $\mathcal U$.

For the fixed length $m$, let $\mathcal B_m$ be the family of sets containing no m-term [arithmetic progression](../../../../../arithmetic-progression.md). Any acceptable [ultrafilter](../../../../../ultrafilter.md) must contain every complement $\mathbb N\setminus B$ with $B\in\mathcal B_m$. These mandatory sets have the [finite intersection property](../../../../../finite-intersection-property.md). Otherwise finitely many $B_1,\ldots,B_r\in\mathcal B_m$ would cover $\mathbb N$. Colour an [integer](../../../../../integer.md) by the first $i$ for which it belongs to $B_i$. The [Van der Waerden theorem](../../../../../van-der-waerden-theorem.md) gives a [monochromatic](../../../../../monochromatic-set.md) m-term [arithmetic progression](../../../../../arithmetic-progression.md), contained in the corresponding $B_i$, a contradiction.

Generate a proper [filter](../../../../../filter-set-theory.md) from those complements and extend it by the [ultrafilter lemma](../../../../../ultrafilter-lemma.md). If some $B\in\mathcal U$ were in $\mathcal B_m$, its complement would also belong to $\mathcal U$, forcing the empty set into the [filter](../../../../../filter-set-theory.md). Thus

$$
\boxed{\exists\mathcal U_m\quad\forall B\in\mathcal U_m,\ B\text{ contains an }m\text{-term arithmetic progression}.}
$$

Notice that sets avoiding one fixed length need not be closed under finite unions; the argument uses the [finite intersection property](../../../../../finite-intersection-property.md), not an unsupported ideal claim.

For the unbounded-length version, let $\mathcal B$ consist of sets whose [arithmetic progression](../../../../../arithmetic-progression.md) lengths are bounded. Each $B_i\in\mathcal B$ fails to contain a progression of some length $m_i$, and hence of every greater length. If finitely many $B_i$ covered $\mathbb N$, colour by the first containing index and apply the [Van der Waerden theorem](../../../../../van-der-waerden-theorem.md) at length $M=\max_i m_i$. Again a contradiction results. The complements of all members of $\mathcal B$ therefore have the [finite intersection property](../../../../../finite-intersection-property.md). Extending their generated [filter](../../../../../filter-set-theory.md) gives an [ultrafilter with arithmetic-progression-rich members](../../../../../ultrafilter-with-arithmetic-progression-rich-members.md):

$$
\boxed{\exists\mathcal U\quad\forall B\in\mathcal U\quad\forall m\ge1,\ B\text{ contains an }m\text{-term arithmetic progression}.}
$$

All [finite sets](../../../../../finite-set.md) lie in $\mathcal B$, so this [ultrafilter](../../../../../ultrafilter.md) contains every [cofinite set](../../../../../cofinite-set.md) and is a [nonprincipal ultrafilter](../../../../../nonprincipal-ultrafilter.md). The same is true of the fixed-length construction when $m\ge2$, because no singleton is allowed; for $m=1$ a [principal ultrafilter](../../../../../principal-ultrafilter.md) also works. These constructions illustrate [ultrafilter selection from a partition-rich family](../../../../../ultrafilter-selection-from-a-partition-rich-family.md).

The infinite-length answer is **no**. Colour $n$ by $\lfloor\log_2n\rfloor\bmod2$, so successive intervals $[2^j,2^{j+1})$ alternate colours. An infinite [arithmetic progression](../../../../../arithmetic-progression.md) $a+td$, $t\ge0$, meets every sufficiently large such interval: its first term at least $2^j$ is less than $2^j+d$, which is at most $2^{j+1}$ once $2^j\ge d$. It therefore has terms of both colours. Neither colour class contains an infinite [arithmetic progression](../../../../../arithmetic-progression.md), but every [ultrafilter](../../../../../ultrafilter.md) contains one of the two colour classes. This [dyadic block obstruction to infinite arithmetic progressions](../../../../../dyadic-block-obstruction-to-infinite-arithmetic-progressions.md) rules out the proposed [ultrafilter](../../../../../ultrafilter.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
