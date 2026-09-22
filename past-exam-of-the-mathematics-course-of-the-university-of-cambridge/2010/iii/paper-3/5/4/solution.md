<h1 id="5/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

To compute the [first Tor of a cyclic quotient](../../../../../../first-tor-of-a-cyclic-quotient.md), start a [free resolution](../../../../../../free-resolution.md) of $A/I$ with $P_0=A$, take a free module $P_1$ surjecting onto $I$, and take $P_2$ surjecting onto the kernel of $P_1\to I$. Tensor right exactness identifies

$$
\operatorname{coker}(P_2\otimes_AM\longrightarrow P_1\otimes_AM)
\simeq I\otimes_AM.
$$

By definition, the degree-one [Tor functor](../../../../../../tor-functor.md) is the kernel of $P_1\otimes_AM\to A\otimes_AM$ modulo the image from $P_2\otimes_AM$. Quotienting first by that image consequently gives the natural identification

$$
\boxed{\operatorname{Tor}_1^A(A/I,M)\simeq
\ker(\mu_I:I\otimes_AM\longrightarrow M).}
$$

Equivalently the calculation gives the exact sequence

$$
0\longrightarrow\operatorname{Tor}_1^A(A/I,M)
\longrightarrow I\otimes_AM\xrightarrow{\mu_I}M
\longrightarrow M/IM\longrightarrow0.
$$

Thus its first term vanishes for every ideal exactly when each multiplication map is injective, proving

$$
\boxed{(3)\Longleftrightarrow(4).}
$$

Together with the preceding implications, **all four conditions are equivalent**. The proof used explicit extension arguments, character duality and the definition of the [Tor functor](../../../../../../tor-functor.md), rather than an unproved flatness or injectivity criterion.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [5](../../5.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
