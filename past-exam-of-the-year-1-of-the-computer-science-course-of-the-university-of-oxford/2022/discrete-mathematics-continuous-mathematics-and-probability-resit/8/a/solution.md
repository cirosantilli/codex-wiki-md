<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $(B_j)$ be a finite or countable [partition of a set](../../../../../partition-of-a-set.md) of the [sample space](../../../../../sample-space.md) into disjoint [events](../../../../../event.md), with $\mathbb P(B_j)>0$. For any [event](../../../../../event.md) $A$, the [law of total probability](../../../../../law-of-total-probability.md) is

$$
\boxed{\mathbb P(A)=\sum_j\mathbb P(A\mid B_j)\mathbb P(B_j).}
$$

To prove it, the intersections $A\cap B_j$ are disjoint and have union $A$. [Countable additivity](../../../../../countable-additivity.md) and the definition of [conditional probability](../../../../../conditional-probability.md) therefore give

$$
\mathbb P(A)=\sum_j\mathbb P(A\cap B_j)=\sum_j\mathbb P(A\mid B_j)\mathbb P(B_j).
$$

It is enough that the union of the partition [events](../../../../../event.md) has [probability](../../../../../probability.md) one. Parts of [probability](../../../../../probability.md) zero contribute zero in the intersection formula and can be omitted before writing [conditional probabilities](../../../../../conditional-probability.md); conditioning by division on a zero-[probability](../../../../../probability.md) part would be undefined.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [Discrete mathematics, continuous mathematics and probability resit](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
