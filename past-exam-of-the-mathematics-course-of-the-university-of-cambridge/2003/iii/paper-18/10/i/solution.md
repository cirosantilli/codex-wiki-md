<h1 id="10/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [monoidal category](../../../../../../monoidal-category.md) consists of a category $\mathcal C$, a bifunctor $\otimes:\mathcal C\times\mathcal C\to\mathcal C$, a unit object $I$, and natural [isomorphisms](../../../../../../isomorphism.md) $a_{X,Y,Z}:(X\otimes Y)\otimes Z\to X\otimes(Y\otimes Z)$, $l_X:I\otimes X\to X$ and $r_X:X\otimes I\to X$. They satisfy the [pentagon identity for a monoidal category](../../../../../../pentagon-identity-for-a-monoidal-category.md)

$$
a_{W,X,Y\otimes Z}a_{W\otimes X,Y,Z}=(1_W\otimes a_{X,Y,Z})a_{W,X\otimes Y,Z}(a_{W,X,Y}\otimes1_Z)
$$

and the [triangle identity for a monoidal category](../../../../../../triangle-identity-for-a-monoidal-category.md) $(1_X\otimes l_Y)a_{X,I,Y}=r_X\otimes1_Y$. These axioms make different coherent rebracketings and unit removals agree.

It defines a [bicategory](../../../../../../bicategory.md) with one object $*$. The hom-category $\mathcal B(*,*)$ is $\mathcal C$; objects of $\mathcal C$ are its 1-cells and morphisms of $\mathcal C$ its 2-cells. Horizontal composition is the tensor bifunctor, the identity 1-cell is $I$, and the associator and unitors are the bicategorical coherence 2-cells. Vertical composition is composition of morphisms in $\mathcal C$, and the interchange law follows from bifunctoriality of $\otimes$. Conversely the hom-category of any one-object [bicategory](../../../../../../bicategory.md) has exactly this monoidal structure. Thus **a monoidal category is precisely a one-object [bicategory](../../../../../../bicategory.md)**, not necessarily a strict one-object 2-category.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [10](../../10.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
