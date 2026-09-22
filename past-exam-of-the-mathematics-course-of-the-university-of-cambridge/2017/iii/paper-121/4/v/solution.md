<h1 id="4/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

The [Rasiowa–Sikorski lemma](../../../../../../rasiowa-sikorski-lemma.md) constructs a [generic filter](../../../../../../generic-filter.md) $G_i$ over each $M_i$. Every resulting [generic extension](../../../../../../generic-extension.md) remains a [countable transitive model](../../../../../../countable-transitive-model.md) of [ZFC](../../../../../../zermelo-fraenkel-set-theory-with-choice.md): there are only countably many ground-model names externally. The order $\mathbb P$ has the same elements and ordering at every stage, and [atomless forcing order](../../../../../../atomless-forcing-order.md) structure is absolute because all its quantifiers are bounded to $\mathbb P$. Hence the [generic filter for an atomless order is new](../../../../../../generic-filter-for-an-atomless-order-is-new.md) result gives $G_i\notin M_i$ for every $i$.

The increasing union $N=\bigcup_{i<\omega}M_i$ is transitive and contains $\mathbb P$. If it satisfied [Axiom of power set](../../../../../../axiom-of-power-set.md) for $\mathbb P$, there would be a [set](../../../../../../set-split.md) $A\in N$ with

$$
N\models\forall z\,(z\subseteq\mathbb P\leftrightarrow z\in A).
$$

Choose $i$ with $A\in M_i$. The next-stage [generic filter](../../../../../../generic-filter.md) $G_i$ belongs to $M_{i+1}\subseteq N$ and is an actual [subset](../../../../../../subset.md) of $\mathbb P$. This subset assertion is absolute for the [transitive set](../../../../../../transitive-set.md) $N$, so $G_i\in A$. Transitivity of $M_i$ and $A\in M_i$ then give $G_i\in M_i$, a contradiction. Thus the [power-set failure in an increasing union of generic extensions](../../../../../../power-set-failure-in-an-increasing-union-of-generic-extensions.md) occurs already at the fixed ground-model order:

$$
\boxed{N\not\models\mathsf{PowerSet}\quad\text{because no }\mathcal P^N(\mathbb P)\text{ belongs to }N.}
$$

The stages form an increasing chain, not an elementary chain, so the [elementary chain theorem](../../../../../../elementary-chain-theorem.md) does not assert [ZFC](../../../../../../zermelo-fraenkel-set-theory-with-choice.md) for their union.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [4](../../4.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
