<h1 id="c4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use **[global sequence alignment](../../../../../global-sequence-alignment.md)**, for example the [Needleman-Wunsch algorithm](../../../../../needleman-wunsch-algorithm.md) with an appropriate [substitution matrix](../../../../../substitution-matrix.md) and [gap penalty](../../../../../gap-penalty.md). The two full-length [globin](../../../../../globin.md) [proteins](../../../../../protein-split.md) are related by [orthology](../../../../../orthology.md) and are from closely related species, so the expected correspondence extends across both complete sequences. Unmatched ends should normally contribute to the score rather than being discarded.

With a [linear gap penalty](../../../../../linear-gap-penalty.md) of magnitude $g$, the [dynamic programming](../../../../../dynamic-programming.md) entry $F_{ij}$ is the best score for the first $i$ and $j$ residues. It satisfies

$$
F_{ij}=\max\{F_{i-1,j-1}+s(a_i,b_j),\ F_{i-1,j}-g,\ F_{i,j-1}-g\},
$$

with $F_{i0}=-ig$, $F_{0j}=-jg$, and traceback from $F_{mn}$. An [affine gap penalty](../../../../../affine-gap-penalty.md) uses separate match and gap states.

## ↑ Ancestors (13)

1. [F](../f.md)
2. [C4](../../c4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
