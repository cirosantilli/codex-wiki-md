<h1 id="8/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Two unary predicates suffice. Require all four [unary predicate types](../../../../../unary-predicate-type.md) to be inhabited:

$$
\boxed{
\exists x\,(P(x)\land Q(x))\ \land\
\exists x\,(P(x)\land\neg Q(x))\ \land\
\exists x\,(\neg P(x)\land Q(x))\ \land\
\exists x\,(\neg P(x)\land\neg Q(x)).}
$$

There are no constants, no [logical equality](../../../../../logical-equality.md) and no nonunary predicates. Any two of these conditions disagree on at least one predicate, so one domain element cannot witness both. Hence every satisfying [first-order structure](../../../../../first-order-structure.md) has at least four elements, by [distinct witnesses from incompatible unary predicates](../../../../../distinct-witnesses-from-incompatible-unary-predicates.md). Conversely take domain $\{a,b,c,d\}$, $P=\{a,b\}$ and $Q=\{a,c\}$: the four elements realize the four displayed [unary predicate types](../../../../../unary-predicate-type.md), respectively. These element names describe the example; they are not constants in the [first-order sentence](../../../../../first-order-sentence.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [8](../../8.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
