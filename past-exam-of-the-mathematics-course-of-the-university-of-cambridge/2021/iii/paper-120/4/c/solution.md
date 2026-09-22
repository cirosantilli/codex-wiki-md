<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $T$ have a [semidecidable axiomatization](../../../../../../semidecidable-axiomatization.md). If $T$ is inconsistent, the singleton axiom set $\{\bot\}$ is decidable and independent. If $T$ has no nonlogical axioms, the empty set already works. In the remaining case assume $T$ is consistent, choose a total computable enumeration $A_1,A_2,\ldots$ of its axioms, allowing repetitions, and conservatively enlarge the language by fresh nullary predicates $P_1,P_2,\ldots$.

For each $i\geq1$, let $B_i$ be the conjunction of $i$ copies of $P_i\land A_i$. The range $\{B_i:i\geq1\}$ is decidable by the [Craig trick](../../../../../../craig-trick.md). Given a candidate formula of length $m$, only indices $i\leq m$ are possible; compute $A_1,\ldots,A_m$, form the corresponding $B_i$, and compare the finite list syntactically.

The new theory has exactly the same consequences in the original language. Every model of $T$ expands to a model of all $B_i$ by interpreting every $P_i$ as true, while the reduct of any model of all $B_i$ satisfies every $A_i$. The axioms are independent: after deleting $B_i$, take any model of $T$, interpret $P_j$ as true for $j\ne i$, and interpret $P_i$ as false. This expansion satisfies every remaining $B_j$ but not $B_i$. Hence the $B_i$ form an [independent tagged axiomatization](../../../../../../independent-tagged-axiomatization.md) that is decidable. Here equivalence means a conservative extension, or equivalently equality of all consequences in the original language.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
