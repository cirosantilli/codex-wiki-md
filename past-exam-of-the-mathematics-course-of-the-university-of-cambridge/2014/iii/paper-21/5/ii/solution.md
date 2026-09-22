<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**As printed, yes: the relation is universal.** The original PDF puts the existentially quantified element in the same subset as the universally quantified element; this is not an OCR substitution. For each element of that subset, choose the element itself as witness, using reflexivity of the underlying [well-quasi-ordering](../../../../../../well-quasi-ordering.md). For an empty subset the condition is vacuous. The truth value therefore never depends on the proposed target subset. On the [power set](../../../../../../power-set.md) this is a reflexive transitive relation, and every two terms of any infinite [sequence](../../../../../../sequence.md) are related:

$$
\boxed{\text{literal printed relation}=\mathcal P(X)\times\mathcal P(X),\qquad\text{hence it is a well-quasi-ordering}.}
$$

A [well-quasi-ordering](../../../../../../well-quasi-ordering.md) need not be antisymmetric, so universal comparability is allowed.

If the existential element is instead intended to belong to the target subset, the natural relation is the [Hoare domination preorder](../../../../../../hoare-domination-preorder.md)

$$
S\le_H T\quad\Longleftrightarrow\quad\forall s\in S\;\exists t\in T\;(s\le_Xt).
$$

**For arbitrary subsets the answer to that corrected question is no.** Here is a complete counterexample, the [Rado order](../../../../../../rado-order.md). Take

$$
R=\{(m,n)\in\mathbb N^2:m<n\},\qquad
(m,n)\le_R(k,l)\quad\Longleftrightarrow\quad
\bigl(m=k\text{ and }n\le l\bigr)\ \text{or}\ n<k.
$$

This is a [partial order](../../../../../../partially-ordered-set.md). Reflexivity is immediate. For transitivity, two same-row comparisons compose ordinarily. If the first comparison crosses rows and the second stays in its row, its target first coordinate is unchanged, so the cross-row inequality persists. If the first stays in its row and the second crosses, use $n\le l<k'$; if both cross, use $n<k<l<k'$. Antisymmetry follows because comparisons across distinct rows in both directions would require $n<k<l<m<n$.

The [Rado order](../../../../../../rado-order.md) is a [well-quasi-ordering](../../../../../../well-quasi-ordering.md). Given an infinite [sequence](../../../../../../sequence.md) $(m_i,n_i)$, if a first coordinate $m$ repeats infinitely often, its corresponding natural-number second coordinates have a nondecreasing pair, giving a same-row comparison. Otherwise each first coordinate occurs only finitely often, so the first coordinates in every tail are unbounded. In particular some later $m_j$ exceeds $n_0$, giving $(m_0,n_0)\le_R(m_j,n_j)$.

For each $m$, take the infinite row $S_m=\{(m,n):n>m\}$. For distinct $m,k$, choose $n>\max(m,k)$. The element $(m,n)\in S_m$ is below no member $(k,l)$ of $S_k$, since its first coordinate is different and $n<k$ fails. Thus $S_m\not\le_HS_k$ for every pair of distinct indices. These subsets form an infinite [antichain](../../../../../../antichain.md), so the [Hoare domination preorder](../../../../../../hoare-domination-preorder.md) on $\mathcal P(R)$ is not a [well-quasi-ordering](../../../../../../well-quasi-ordering.md).

If only finite subsets were intended, the answer changes again: **the [finite-subset lifting of a well-quasi-order](../../../../../../finite-subset-lifting-of-a-well-quasi-order.md) is a [well-quasi-ordering](../../../../../../well-quasi-ordering.md).** Enumerate each finite subset as a finite [word](../../../../../../string.md). [Higman lemma](../../../../../../higman-s-lemma.md) gives an earlier [word](../../../../../../string.md) embedding into a later one with every letter increased, which witnesses [Hoare domination preorder](../../../../../../hoare-domination-preorder.md) comparison of the underlying subsets. The PDF specifies no finiteness restriction, so this observation supplements rather than replaces the literal answer and the arbitrary-subset counterexample.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
