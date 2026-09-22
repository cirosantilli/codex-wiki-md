<h1 id="c4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

An [affine gap penalty](../../../../../affine-gap-penalty.md) charges a larger opening cost than extension cost, reflecting that a single insertion or deletion event can span several residues. For a gap of length $\ell\geq1$, explicitly choose

$$
g(\ell)=o+e(\ell-1),\qquad o=4,\quad e=1.
$$

The supplied [sequence alignment](../../../../../sequence-alignment.md) has two gap runs, of lengths one and two. Its residue–residue score remains $24$, so this choice gives

$$
\boxed{S=24-g(1)-g(2)=24-4-5=15}.
$$

More generally, this [affine gap penalty](../../../../../affine-gap-penalty.md) convention gives $S=24-2o-e$. There is no unique numerical rescore until opening and extension costs are chosen. A concave length-dependent [gap penalty](../../../../../gap-penalty.md) can make very long gaps progressively cheaper per added residue; distinct terminal [gap penalties](../../../../../gap-penalty.md) can accommodate incomplete sequence ends. Each choice encodes a different assumption about insertions, deletions or sequence completeness.

## ↑ Ancestors (13)

1. [E](../e.md)
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
