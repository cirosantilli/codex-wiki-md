<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Name every element $a\in A$ by a new constant $c_a$, distinct from the symbols already in $L'$. Let $\operatorname{Diag}(A)$ be its full atomic and negated atomic [diagram of a structure](../../../../../../diagram-mathematical-logic.md). A model of this diagram contains an isomorphic copy of $A$ as an $L$-[substructure](../../../../../../substructure-of-a-first-order-structure.md). We claim

$$
T'\cup\operatorname{Diag}(A)
$$

is satisfiable.

Otherwise [compactness theorem](../../../../../../compactness-theorem.md) gives a finite diagram conjunction $\delta(c_{a_1},\ldots,c_{a_m})$ inconsistent with $T'$. Replace these new constants by variables. Since $T'$ says nothing about the new names, it then entails the [universal sentence](../../../../../../universal-sentence.md)

$$
\forall x_1\cdots\forall x_m\,\neg\delta(x_1,\ldots,x_m).
$$

The conjunction $\delta$ uses only symbols of $L$, so this is one of the universal $L$-consequences assumed true in $A$. But $A$ satisfies $\delta(a_1,\ldots,a_m)$, a contradiction. A model of the consistent enlarged theory gives **an embedding of $A$ into the $L$-reduct of a model of $T'$**. Negated atomic facts and disequalities in the diagram ensure that this is a [structure embedding](../../../../../../structure-embedding.md), not merely a homomorphism.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
