<h1 id="c4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [BLOSUM](../../../../../blosum.md) [substitution matrix](../../../../../substitution-matrix.md) is estimated from conserved, ungapped blocks of related [protein](../../../../../protein-split.md) sequences. Closely related sequences are clustered to reduce overrepresentation, and aligned [amino acid](../../../../../amino-acid.md) pairs from different clusters are counted. Let $q_{ij}$ be their normalized observed pair frequency, and $e_{ij}$ the frequency expected from independent draws at the background [amino acid](../../../../../amino-acid.md) frequencies. With unordered pairs, $e_{ii}=p_i^2$ and $e_{ij}=2p_ip_j$ for $i\ne j$.

For [BLOSUM62](../../../../../blosum62.md), scores are rounded half-bit [logarithms](../../../../../logarithm.md) of these odds:

$$
\boxed{s_{ij}\simeq2\log_2(q_{ij}/e_{ij})}.
$$

A positive entry means that the aligned pair occurs more often in related sequences than the independent-background model predicts; a negative entry means less often. Adding these scores accumulates evidence across aligned positions. A score is neither a percentage identity nor a direct substitution [probability](../../../../../probability.md).[The choice of substitution scores; The PAM and BLOSUM amino acid substitution matrices](../../../../../the-statistics-of-sequence-similarity-scores-by-national-center-for-biotechnology-information.md)

## ↑ Ancestors (13)

1. [A](../a.md)
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
