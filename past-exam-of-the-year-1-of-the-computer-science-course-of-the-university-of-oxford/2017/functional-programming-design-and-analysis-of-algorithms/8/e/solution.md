<h1 id="8/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For [local sequence alignment without mismatches](../../../../../local-sequence-alignment-without-mismatches.md), let $L_{i,j}$ maximize the score of alignments of a suffix of each prefix of lengths $i,j$, allowing both suffixes to be empty. Initialize $L_{i,0}=L_{0,j}=0$ and fill

$$
\boxed{L_{i,j}=\max\left\{0,\ L_{i-1,j}-g,\ L_{i,j-1}-g,\ L_{i-1,j-1}+1\ \text{only if }x[i-1]=y[j-1]\right\}.}
$$

Zero starts a new alignment; the remaining candidates append the possible last columns. The same optimal-substructure argument as before proves the recurrence. Because $g\geq0$, an alignment with a negative-scoring leading portion can be improved by dropping that portion, which is exactly what the zero reset permits.

Return **$\max_{0\leq i\leq m,\,0\leq j\leq n}L_{i,j}$**, since an optimal pair of substrings may finish before either full string ends. The time is **$O(mn)$** for positive input lengths, with $O(mn)$ full-table space or linear rolling-row space for the score alone. If an alignment is wanted, start [alignment traceback](../../../../../alignment-traceback.md) at a maximum entry and stop at zero. No mismatching diagonal is introduced.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
