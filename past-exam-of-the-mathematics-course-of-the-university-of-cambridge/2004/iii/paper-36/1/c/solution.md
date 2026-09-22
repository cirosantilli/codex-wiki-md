<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First pass from the [preorder](../../../../../../preorder.md) $R$ to a [partial order](../../../../../../partially-ordered-set.md). Define the [indifference relation](../../../../../../indifference-relation.md) $y\sim z$ by $yRz$ and $zRy$. [Reflexivity](../../../../../../reflexive-relation.md) and [transitivity](../../../../../../transitive-relation.md) make this an [equivalence relation](../../../../../../equivalence-relation.md). On the quotient set $C=\mathbb R^L/{\sim}$, put

$$
[y]\unrhd[z]\quad\Longleftrightarrow\quad yRz.
$$

[Transitivity](../../../../../../transitive-relation.md) makes this independent of the representatives, and the quotient relation is antisymmetric, hence a [partial order](../../../../../../partially-ordered-set.md).

We need its order-extension property, including freedom to order incomparable classes. Here is the argument. Order all [partial order](../../../../../../partially-ordered-set.md) extensions of $\unrhd$ by inclusion. The union of a chain of extensions is again a [partial order](../../../../../../partially-ordered-set.md): any finite list of comparisons needed to check an axiom occurs together in one member of the chain. [Zorn's lemma](../../../../../../zorn-s-lemma.md) therefore supplies a maximal extension. If two classes $A,B$ remain incomparable, adjoin $A\unrhd B$ and take the [transitive closure of a relation](../../../../../../transitive-closure-relation.md). The only possible new comparisons have the form $X\unrhd A\unrhd B\unrhd Y$. A cycle would require a previously existing path $B\unrhd A$, contradicting incomparability. The enlarged relation is still a [partial order](../../../../../../partially-ordered-set.md), contradicting maximality. Consequently the maximal extension is a [total order](../../../../../../total-order.md). This also proves the [Szpilrajn extension theorem](../../../../../../szpilrajn-extension-theorem.md) used here.

Lift such a [total order](../../../../../../total-order.md) to the original bundles by comparing their equivalence classes. The lifted [preference relation](../../../../../../preference-relation.md) $R'$ is complete and [transitive](../../../../../../transitive-relation.md), contains $R$, and preserves its [strict preference](../../../../../../strict-preference.md): if $yPz$, their distinct classes satisfy $[y]\unrhd[z]$, and antisymmetry of the extended order prevents the reverse comparison. In particular, the class $\mathcal P$ is nonempty and $R\subseteq\bigcap_{R'\in\mathcal P}R'$.

For the reverse inclusion, take a pair with $\neg(yRz)$. If $zRy$, then $zPy$, so every member of $\mathcal P$ strictly ranks $z$ above $y$ and excludes $yR'z$. If neither comparison holds, their classes are incomparable. First adjoin $[z]\unrhd[y]$, which creates no cycle by the preceding argument, and then extend to a [total order](../../../../../../total-order.md). Its lift belongs to $\mathcal P$ and again excludes $yR'z$. Thus every pair outside $R$ is outside at least one member of $\mathcal P$, proving

$$
\boxed{\bigcap_{R'\in\mathcal P}R'=R.}
$$

The intersection proof is an order-theoretic fact about any [preorder](../../../../../../preorder.md). The [congruence axiom](../../../../../../congruence-axiom.md) additionally ensures exact rationalization of the observed [demand correspondence](../../../../../../demand-correspondence.md): every chosen bundle weakly outranks every affordable bundle, while an affordable unchosen bundle is strictly worse by part (b). Hence each completion's budget-maximizing set is exactly the observed chosen set.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
