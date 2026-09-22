<h1 id="c4/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Use **[local sequence alignment](../../../../../local-sequence-alignment.md)**, such as the [Smith-Waterman algorithm](../../../../../smith-waterman-algorithm.md), to compare the [globin](../../../../../globin.md) fragment with the matching region of each full-length target. A [global sequence alignment](../../../../../global-sequence-alignment.md) would penalize long target flanks absent from the fragment. For a [linear gap penalty](../../../../../linear-gap-penalty.md) the [dynamic programming](../../../../../dynamic-programming.md) recurrence includes a restart option:

$$
H_{ij}=\max\{0,\ H_{i-1,j-1}+s(a_i,b_j),\ H_{i-1,j}-g,\ H_{i,j-1}-g\}.
$$

Initialize boundary entries to zero, start traceback at the largest entry anywhere, and stop at zero. If the entire query is known to be valid and must be retained, [fitting sequence alignment](../../../../../fitting-sequence-alignment.md) is a suitable refinement: align the whole fragment while leaving target flanks unpenalized.

First check the sequence alphabet: the prompt calls the targets “genes”. If the [FASTA format](../../../../../fasta-format.md) file contains [DNA](../../../../../deoxyribonucleic-acid.md) rather than [protein](../../../../../protein-split.md), translate the relevant coding sequences into [amino acids](../../../../../amino-acid.md) before a protein-to-protein [sequence alignment](../../../../../sequence-alignment.md). If coding frames are unknown, search translated frames. A file in [FASTA format](../../../../../fasta-format.md) specifies storage syntax, not whether the contents are nucleotides or residues.

## ↑ Ancestors (13)

1. [G](../g.md)
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
