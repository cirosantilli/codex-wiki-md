<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Split each input into its more and less significant $n$-[bit](../../../../../bit.md) halves: $a=2^na_H+a_L$ and $b=2^nb_H+b_L$. Let the two [digital comparators](../../../../../digital-comparator.md) produce $(L_H,G_H)$ and $(L_L,G_L)$. The more significant halves are equal exactly when $E_H=\neg(L_H\lor G_H)$. The [comparator composition](../../../../../comparator-composition.md) is therefore

$$
\boxed{L=L_H\lor(E_H\land L_L),\qquad G=G_H\lor(E_H\land G_L).}
$$

Implement $E_H$ with a [logical disjunction](../../../../../logical-disjunction.md) followed by a [negation](../../../../../negation.md), then use two [AND gates](../../../../../and-gate.md) and two more [logical disjunction](../../../../../logical-disjunction.md) [logic gates](../../../../../logic-gate.md). If $a_H\ne b_H$, the difference $2^n(a_H-b_H)$ has magnitude at least $2^n$, whereas $|a_L-b_L|\le2^n-1$; hence the more significant comparison decides the result. If $a_H=b_H$, the lower comparison decides it. This proves correctness in every case using a constant number of extra [logic gates](../../../../../logic-gate.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
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
