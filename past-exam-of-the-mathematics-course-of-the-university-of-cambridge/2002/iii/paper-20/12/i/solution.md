<h1 id="12/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [monoidal category](../../../../../../monoidal-category.md) consists of a [category](../../../../../../category-split.md) $\mathcal C$, a [bifunctor](../../../../../../bifunctor.md) $\otimes:\mathcal C\times\mathcal C\to\mathcal C$, a [monoidal unit object](../../../../../../monoidal-unit-object.md) $I$, and [natural isomorphisms](../../../../../../natural-isomorphism.md)

$$
\alpha_{A,B,C}:(A\otimes B)\otimes C\to A\otimes(B\otimes C),\quad
\lambda_A:I\otimes A\to A,\quad\rho_A:A\otimes I\to A.
$$

The [associator](../../../../../../associator.md) obeys the [pentagon identity for a monoidal category](../../../../../../pentagon-identity-for-a-monoidal-category.md),

$$
\alpha_{A,B,C\otimes D}\,\alpha_{A\otimes B,C,D}
=(1_A\otimes\alpha_{B,C,D})\,\alpha_{A,B\otimes C,D}\,(\alpha_{A,B,C}\otimes1_D),
$$

and the [unitors](../../../../../../unitor.md) obey the [triangle identity for a monoidal category](../../../../../../triangle-identity-for-a-monoidal-category.md),

$$
(1_A\otimes\lambda_B)\,\alpha_{A,I,B}=\rho_A\otimes1_B.
$$

[Composition in a category](../../../../../../composition-in-a-category.md) here acts from right to left. The first equation compares two paths from $((A\otimes B)\otimes C)\otimes D$ to $A\otimes(B\otimes(C\otimes D))$; the second compares two ways of removing the intervening unit.

It is precisely a [bicategory](../../../../../../bicategory.md) with one object $*$. The [category](../../../../../../category-split.md) $\mathcal B(*,*)$ is $\mathcal C$: its objects are the 1-morphisms and its [morphisms](../../../../../../morphism.md) are the 2-morphisms. Horizontal [composition in a category](../../../../../../composition-in-a-category.md) is $\otimes$, the identity 1-morphism is $I$, and the [associator](../../../../../../associator.md) and [unitors](../../../../../../unitor.md) give the weak associativity and unit constraints. Vertical [composition in a category](../../../../../../composition-in-a-category.md) is ordinary [composition in a category](../../../../../../composition-in-a-category.md) in $\mathcal C$; the interchange law follows because $\otimes$ is a [bifunctor](../../../../../../bifunctor.md). The bicategory pentagon and triangle axioms are exactly the two equations above. Conversely the sole hom-category of any one-object [bicategory](../../../../../../bicategory.md) gives these data, with the convention that horizontal [composition in a category](../../../../../../composition-in-a-category.md) uses the indicated ordering of tensor factors.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [12](../../12.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
