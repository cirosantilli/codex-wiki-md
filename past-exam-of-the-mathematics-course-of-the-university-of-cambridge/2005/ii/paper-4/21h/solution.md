<h1 id="21h/solution">Solution</h1>

↑ **Parent:** [21H](../21h.md)

Use [relative homology](../../../../../relative-homology.md). Every simplex of $X=B\cup C$ lies in $B$ or $C$, and those lying in both are exactly the simplices of $A$. Consequently inclusion induces a chain-complex [isomorphism](../../../../../isomorphism.md)

$$
C_*(B)/C_*(A)\ \cong\ C_*(X)/C_*(C).
$$

It is bijective on the respective bases of simplices and commutes with boundary because it comes from inclusion. Thus

$$
H_j(B,A)\cong H_j(X,C)\quad\text{for every }j.
$$

For any pair $(Y,Z)$, the [long exact sequence in homology](../../../../../long-exact-sequence-in-homology.md) shows that inclusion induces [isomorphisms](../../../../../isomorphism.md) in every degree exactly when $H_j(Y,Z)=0$ for every $j$. To verify both directions, if all relative groups vanish, exactness makes each $H_j(Z)\to H_j(Y)$ injective and surjective. Conversely, if the inclusion maps are [isomorphisms](../../../../../isomorphism.md), the map from $H_j(Y)$ into the relative group is zero, while the relative connecting map is injective and has zero image because the next inclusion is injective; hence the relative group itself is zero. This includes degree zero, with the negative-degree ordinary group zero.

Apply the criterion first to $(B,A)$ and then to $(X,C)$ using the chain [isomorphism](../../../../../isomorphism.md). It proves

$$
\boxed{H_*A\longrightarrow H_*B\text{ is an isomorphism}
\ \Longleftrightarrow\
H_*C\longrightarrow H_*X\text{ is an isomorphism}}.
$$

## ↑ Ancestors (10)

1. [21H](../21h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
