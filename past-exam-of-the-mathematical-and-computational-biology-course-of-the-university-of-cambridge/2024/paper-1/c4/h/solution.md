<h1 id="c4/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

The gain comes from avoiding a full [dynamic programming](../../../../../dynamic-programming.md) table for every target. [BLAST](../../../../../blast.md) searches for short, sufficiently high-scoring word matches between query and database, then extends promising seeds. Modern versions reserve expensive gapped refinement for candidates passing earlier filters. [FASTA sequence search](../../../../../fasta-sequence-search.md) similarly starts from short word matches, collects promising runs along alignment diagonals, and refines or joins selected regions. Word lookup and database indexing make candidate discovery inexpensive compared with considering every pair of positions.[pp. 403–406, word matches and hit extension](../../../../../basic-local-alignment-search-tool-by-stephen-f-altschul-and-others.md)[pp. 2444–2446, FASTA search stages](../../../../../improved-tools-for-biological-sequence-comparison-by-william-r-pearson-and-david-j-lipman.md)

These are [heuristic algorithms](../../../../../heuristic-algorithm.md): a good [local sequence alignment](../../../../../local-sequence-alignment.md) can be missed if it has no acceptable seed, contains many interruptions, or is filtered before extension. Longer words and higher seed-score thresholds usually speed the search but reduce sensitivity; shorter words and looser thresholds recover weaker similarities at greater cost. Repetitive or compositionally biased regions can create many uninformative hits and erode both speed and specificity. No guarantee remains of finding the optimal [sequence alignment](../../../../../sequence-alignment.md) for the chosen scoring scheme.

Thus the practical work depends on word length, thresholds, database composition and the number of hits. The speed-up is substantial on typical data, but does not establish a universal improved worst-case bound over $O(mn)$: an input producing many candidate hits can still require extensive refinement.

## ↑ Ancestors (13)

1. [H](../h.md)
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
