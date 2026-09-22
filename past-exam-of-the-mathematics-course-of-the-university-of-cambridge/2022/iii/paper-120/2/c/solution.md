<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Ehrenfeucht-Mostowski theorem](../../../../../../ehrenfeucht-mostowski-theorem.md) says that if a first-order theory $T$ has an infinite model, then for every [total order](../../../../../../total-order.md) $I$ there is a model $M\models T$ generated as the [Skolem hull](../../../../../../skolem-hull.md) of distinct [order indiscernibles](../../../../../../order-indiscernible-sequence.md) $(a_i)_{i\in I}$, and every order automorphism of $I$ extends to an [automorphism](../../../../../../automorphism-of-a-first-order-structure.md) of $M$.

Given an infinite cardinal $\kappa$, let $I=\kappa\times\mathbb Q$ with the lexicographic order, viewed as $\kappa$ consecutive copies of the rational order. In each copy independently choose either the identity or a fixed nonidentity order automorphism of $\mathbb Q$. These choices give $2^\kappa$ distinct order automorphisms of $I$.

Apply the theorem to this order. Distinct order automorphisms act differently on the distinct generators $a_i$, so their extensions give an injection into the [automorphism group of a first-order structure](../../../../../../automorphism-group-of-a-first-order-structure.md) $\operatorname{Aut}(M)$. Therefore $|\operatorname{Aut}(M)|\geq2^\kappa$, proving that $T$ has [models with arbitrarily large automorphism groups](../../../../../../models-with-arbitrarily-large-automorphism-groups.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
