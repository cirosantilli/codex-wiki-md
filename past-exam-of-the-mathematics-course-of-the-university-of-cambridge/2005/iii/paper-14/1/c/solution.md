<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Since $X$ is an [irreducible variety](../../../../../../irreducible-variety.md), every nonempty open subset is irreducible and the [sheaf of nonzero rational functions on an irreducible variety](../../../../../../sheaf-of-nonzero-rational-functions-on-an-irreducible-variety.md) has value $k(X)^*$ there. All its restriction maps between nonempty opens are identities, and restriction to the empty set is [surjective](../../../../../../surjective-function.md). Thus $\mathcal K_X^*$ is a [flabby sheaf](../../../../../../flasque-sheaf.md), and the introductory argument gives $H^1(X,\mathcal K_X^*)=0$.

Apply the [long exact sequence in sheaf cohomology](../../../../../../long-exact-sequence-in-sheaf-cohomology.md) to the [short exact sequence of sheaves](../../../../../../short-exact-sequence-of-sheaves.md)

$$
1\longrightarrow\mathcal O_X^*\longrightarrow\mathcal K_X^*
\longrightarrow\mathcal D\longrightarrow1.
$$

Its relevant portion is

$$
H^0(X,\mathcal K_X^*)\longrightarrow H^0(X,\mathcal D)
\xrightarrow{\;\partial\;}H^1(X,\mathcal O_X^*)
\longrightarrow H^1(X,\mathcal K_X^*)=0.
$$

The [connecting homomorphism](../../../../../../connecting-homomorphism.md) is therefore [surjective](../../../../../../surjective-function.md), with kernel the image of $k(X)^*$. The computation in part (a) now gives

$$
\boxed{\operatorname{Cl}(X)\cong H^1(X,\mathcal O_X^*).}
$$

Concretely, local rational equations $f_i$ of a [divisor on an algebraic curve](../../../../../../divisor-on-an-algebraic-curve.md) differ by regular units on overlaps. Their ratios give the gluing data of an [invertible sheaf](../../../../../../line-bundle.md); changing the local equations by units changes those data by a coboundary. This is the transition-function interpretation of the identification with the [Picard group](../../../../../../picard-group.md). Reversing all transition ratios replaces a class by its inverse; either consistent convention gives the same group [isomorphism](../../../../../../isomorphism.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
