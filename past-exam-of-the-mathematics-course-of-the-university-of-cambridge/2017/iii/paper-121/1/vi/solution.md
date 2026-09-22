<h1 id="1/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Use the standard convention that a [strongly inaccessible cardinal](../../../../../../strongly-inaccessible-cardinal.md) is uncountable, regular and strong limit. **The printed explanatory definition omits uncountability**: literally it also admits $\kappa=\omega$, for which no finite cardinal is a [worldly cardinal](../../../../../../worldly-cardinal.md). Thus that omission makes the requested conclusion false under the literal abbreviated definition. The proof below applies to the usual, intended [strongly inaccessible cardinal](../../../../../../strongly-inaccessible-cardinal.md) convention $\kappa>\omega$.

First $|V_\gamma|<\kappa$ for every $\gamma<\kappa$. At successor stages this follows from the [strong limit cardinal](../../../../../../strong-limit-cardinal.md) property, and at limits from the [regular cardinal](../../../../../../regular-cardinal.md) property. Consequently $V_\kappa\models\mathsf{ZFC}$. In particular, for [Axiom schema of replacement](../../../../../../axiom-schema-of-replacement.md), a domain $a\in V_\kappa$ has size less than $\kappa$, so its functional image has fewer than $\kappa$ elements, so the supremum of the [rank of a set](../../../../../../rank-of-a-set.md) over its elements is below $\kappa$ by [regular cardinal](../../../../../../regular-cardinal.md) structure. All other axioms, including [axiom of choice](../../../../../../axiom-of-choice.md), have their witnesses at bounded ranks below $\kappa$; uncountability supplies [axiom of infinity](../../../../../../axiom-of-infinity.md).

Enumerate the [first-order formulas](../../../../../../first-order-formula.md) as $\varphi_0,\varphi_1,\ldots$. For each finite collection, reflection inside the set structure $V_\kappa$ gives a [closed unbounded subset](../../../../../../club-set.md) of $\kappa$ of agreeing ranks. To see why the witness bounds stay below $\kappa$, there are fewer than $\kappa$ parameter tuples at each $V_\gamma$, and the supremum of their least witness ranks remains below $\kappa$ by [regular cardinal](../../../../../../regular-cardinal.md) structure. Closing under these bounds and taking increasing countable limits gives the usual [reflection theorem for definable hierarchies](../../../../../../reflection-theorem-for-definable-hierarchies.md) argument. The countable intersection of these [closed unbounded subsets](../../../../../../club-set.md) is still [closed unbounded](../../../../../../club-set.md) because $\kappa$ is regular and uncountable. At each resulting $\alpha$,

$$
(V_\alpha,\in)\prec(V_\kappa,\in),\qquad V_\alpha\models\mathsf{ZFC}.
$$

The infinite [cardinal numbers](../../../../../../cardinal-number.md) below $\kappa$ also form a [closed unbounded subset](../../../../../../club-set.md): they are unbounded because $\lambda^+\leq2^\lambda<\kappa$ for infinite $\lambda<\kappa$, and a supremum of increasing [cardinal numbers](../../../../../../cardinal-number.md) is a [cardinal number](../../../../../../cardinal-number.md). Intersect the two [closed unbounded subsets](../../../../../../club-set.md). Every member of the intersection is a [worldly cardinal](../../../../../../worldly-cardinal.md), and an unbounded [subset](../../../../../../subset.md) of a [regular cardinal](../../../../../../regular-cardinal.md) $\kappa$ has size $\kappa$. Hence

$$
\boxed{\left|\{\alpha<\kappa:\alpha\text{ is a cardinal and }V_\alpha\models\mathsf{ZFC}\}\right|=\kappa.}
$$

In fact this proves the stronger [worldly cardinals below an inaccessible cardinal](../../../../../../worldly-cardinals-below-an-inaccessible-cardinal.md) result that these [worldly cardinals](../../../../../../worldly-cardinal.md) contain a [closed unbounded subset](../../../../../../club-set.md) of $\kappa$.

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [1](../../1.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
