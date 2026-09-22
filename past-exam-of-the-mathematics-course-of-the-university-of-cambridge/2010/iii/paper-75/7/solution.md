<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Interpret the given relation by a [subobject](../../../../../subobject.md) $R\hookrightarrow A\times B$ and write its projections as $p:R\to A$, $q:R\to B$. Totality says that the image of $p$ is all of $A$, so $p$ is a [regular epimorphism](../../../../../regular-epimorphism.md). Single-valuedness makes $p$ monic: if $pr=ps$ for two arrows into $R$, the functionality sequent forces $qr=qs$, and the inclusion into $A\times B$ then gives $r=s$.

A regular epimorphism that is monic is invertible. Indeed its kernel pair consists of equal projections, and its coequalizer universal property supplies an inverse. Therefore define

$$
\boxed{f=q\circ p^{-1}:A\to B}.
$$

The graph of this map is exactly the original relation $R$, since $(p,q)=(1_A,f)p$. The graph also makes the map unique. This proves [total functional relations define morphisms](../../../../../total-functional-relations-define-morphisms.md), using regular-category semantics and no choice of individual witnesses.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
