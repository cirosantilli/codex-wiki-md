<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

If $f:A\to B$ has a section $g:B\to A$, functoriality gives $H_fH_g=1_{H_B}$. Thus $H_f$ is a [split epimorphism](../../../../../../split-epimorphism.md) and in particular an [epimorphism](../../../../../../epimorphism.md).

For the converse, justify the needed pointwise surjectivity directly. Let $I\subseteq H_B$ be the image subpresheaf of $H_f$. Form a new presheaf by taking, at every object, two copies of $H_B(U)$ and identifying their elements in $I(U)$. Restriction maps descend because $I$ is a subpresheaf. The two canonical transformations $j_1,j_2:H_B\to H_B\amalg_IH_B$ agree after $H_f$. If any component of $I$ is proper, an element outside it distinguishes $j_1$ from $j_2$. Therefore epimorphicity forces every component of $H_f$ to be surjective.

In particular, its component at $B$ has $1_B$ in its image: there is $g:B\to A$ with $fg=1_B$. This proves the [Yoneda embedding detects split epimorphisms](../../../../../../yoneda-embedding-detects-split-epimorphisms.md) criterion

$$
\boxed{H_f\text{ is epic if and only if }f\text{ is split epic}.}
$$

Ordinary epimorphicity of $f$ alone would not suffice.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
