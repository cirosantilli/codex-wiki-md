<h1 id="section-i/1-6/solution">Solution</h1>

↑ **Parent:** [1.6](../1-6.md)

Choose a cutoff on the ranked score and call every eligible locus above it positive. Compare those calls with the fixed reference labels, count $TP,FP,TN,FN$, and plot $(FP/(FP+TN),TP/(TP+FN))$. Repeating over cutoffs generates the [receiver operating characteristic](../../../../../receiver-operating-characteristic.md).

A very restrictive cutoff starts near $(0,0)$; a cutoff calling everything positive ends at $(1,1)$. The reference labels and eligible locus set must stay fixed during this sweep. Tied scores need a consistent treatment. A single cutoff gives one operating point, whereas the curve describes the trade-off across many possible cutoffs.

## ↑ Ancestors (13)

1. [1.6](../1-6.md)
2. [Section I](../../section-i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [2024](../../../split.md)
5. [Past exam of the systems biology course of the University of Cambridge](../../../../split.md)
6. [Systems Biology course of the University of Cambridge](../../../../../systems-biology-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
