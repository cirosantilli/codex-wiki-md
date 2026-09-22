<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

A [coherent category](../../../../../coherent-category.md) is a [regular category](../../../../../regular-category.md) with finite unions of [subobjects](../../../../../subobject.md), including the empty union, stable under pullback. Thus it has [finite limits](../../../../../finite-limit.md), pullback-stable regular-epimorphism/monomorphism image factorizations, and pullback-stable finite joins in each subobject lattice.

Write $U=A\vee B\hookrightarrow X$ and $C=A\wedge B=A\times_XB$. Their inclusions give a commutative square

$$
\begin{array}{ccc}C&\longrightarrow&B\\\downarrow&&\downarrow\\A&\longrightarrow&U.\end{array}
$$

To establish the [pushout](../../../../../pushout.md) property, take arrows $a:A\to Y$, $b:B\to Y$ agreeing on $C$. Regard their graphs as subobjects of $U\times Y$ and form their union $R$. Internally, this relation says that a point of $U$ is related to its $a$-value when it lies in $A$, or to its $b$-value when it lies in $B$.

The relation is total because every point of $U$ belongs to at least one of $A,B$. It is single-valued: two witnesses in the same summand give the same value by functionality of that map; witnesses in different summands have their shared point in $C$, where the two maps agree. By the relation argument proved in Question 7's unheaded continuation, the projection $R\to U$ is both a regular epimorphism and monic, hence an isomorphism. It consequently gives a map $h:U\to Y$ restricting to $a,b$.

For uniqueness, the equalizer of two possible maps contains $A$ and $B$, hence contains their union $U$ and is all of $U$. Thus the square is a pushout, proving

$$
\boxed{A\vee B\cong A\amalg_{A\wedge B}B}.
$$

This is the [unions of subobjects are pushouts](../../../../../unions-of-subobjects-are-pushouts.md) property; it does not assume arbitrary pushouts already exist in a coherent category.

## ↑ Ancestors (10)

1. [8](../8.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
