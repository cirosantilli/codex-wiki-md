<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $D_{i,j}$ be the optimal score for aligning the complete prefixes of lengths $i,j$. The boundary values and recurrence are

$$
D_{0,0}=0,\quad D_{i,0}=-gi,\quad D_{0,j}=-gj,
$$



$$
\boxed{D_{i,j}=\max\left\{D_{i-1,j}-g,\ D_{i,j-1}-g,\ D_{i-1,j-1}+1\ \text{only if }x[i-1]=y[j-1]\right\}.}
$$

The last candidate is omitted when the letters differ. Fill rows or columns in increasing index order and return **$D_{m,n}$**. The final-column cases in part (a) exhaust all legal alignments and each can be appended to an optimal smaller alignment, proving the recurrence by [induction](../../../../../mathematical-induction.md) on $i+j$.

There are $(m+1)(n+1)$ entries and at most three constant-time candidates per interior entry. Thus the time is **$O(mn)$** for positive $m,n$, or $O(mn+m+n+1)$ including empty-input boundary cases, with the same full-table space bound. Computing only the score can reduce auxiliary storage to $O(\min(m,n)+1)$ by retaining two rows. This is [global sequence alignment without mismatches](../../../../../global-sequence-alignment-without-mismatches.md); admitting a diagonal move on unequal letters would solve a different problem.

## ↑ Ancestors (12)

1. [B](../b.md)
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
