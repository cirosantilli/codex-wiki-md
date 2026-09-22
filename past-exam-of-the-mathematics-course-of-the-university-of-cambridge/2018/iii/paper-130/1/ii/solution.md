<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\mathcal F$ be an [intersecting family](../../../../../../intersecting-family.md). For a word $w\in[m]^n$, put $S(w)=\{i:w_i=1\}$. Give $w$ the red color if $S(w)$ contains some member of $\mathcal F$, and the blue color otherwise.

Consider any [combinatorial line](../../../../../../combinatorial-line.md) with active set $A\in\mathcal F$. At variable value $1$, $A\subseteq S(w)$, so that word is red. At variable value $2$, $S(w)\cap A=\varnothing$. No member of $\mathcal F$ can be contained in this $S(w)$, because every member meets $A$. Thus that word is blue. No such line is [monochromatic](../../../../../../monochromatic-set.md), proving

$$
\boxed{\mathcal F\text{ intersecting }\Longrightarrow\mathcal F\text{ not adequate}.}
$$

If $\mathcal F$ is empty there is no permitted active set at all, so it is also not an [adequate family of active coordinate sets](../../../../../../adequate-family-of-active-coordinate-sets.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 130](../../../paper-130-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
