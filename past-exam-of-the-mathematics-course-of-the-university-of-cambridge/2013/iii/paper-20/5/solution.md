<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [equivalence classes](../../../../../equivalence-class.md) of an [equivalence relation](../../../../../equivalence-relation.md) are nonempty, pairwise disjoint, and partition $\mathbb N$. To construct a [transversal of a set family](../../../../../hitting-set.md) for them, choose the least member of each class. Its set is

$$
\boxed{S=\{n\in\mathbb N:\forall m<n\;m\not\sim n\}.}
$$

Every class has a least element by the [well-ordering principle for the natural numbers](../../../../../well-ordering-principle-for-the-natural-numbers.md), and that element satisfies the displayed condition. A nonleast element fails it because a smaller equivalent element exists. Therefore **$S$ meets every class in exactly one point**, not merely infinitely many classes.

The [complement](../../../../../complement-of-a-set.md) of $\sim$ is [semidecidable](../../../../../recursively-enumerable-set.md), so for a given $n$ run the finitely many semidecision procedures for $m\not\sim n$, $0\leq m<n$, in parallel. Accept $n$ once all have accepted. If $n$ is a least representative, all finitely many computations halt; otherwise at least one never accepts. For $n=0$, the empty list of tests succeeds immediately. This proves that $S$ is [semidecidable](../../../../../recursively-enumerable-set.md). Equivalently, enumerate inequivalent pairs and output $n$ once all pairs $(m,n)$ with $m<n$ have appeared, dovetailing the requirements over all $n$. This is the [semidecidable least-representative transversal](../../../../../semidecidable-least-representative-transversal.md) of a [co-computably enumerable equivalence relation](../../../../../co-computably-enumerable-equivalence-relation.md). Infinitely many classes make $S$ infinite, but that hypothesis is unnecessary for the existence and semidecidability of a complete transversal.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
