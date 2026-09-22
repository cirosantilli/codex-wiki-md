<h1 id="r/r2/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

For an $m\times n$ rectangle, let $S_j$ be the symbols absent from column $j$. Each has size $n-m$. Across all columns, each symbol is absent exactly $n-m$ times, because it appears once in each existing row. For any set $J$ of columns, count incidences between those columns and their missing symbols. There are $|J|(n-m)$ incidences, while each distinct symbol in the union contributes at most $n-m$. Therefore $|\bigcup_{j\in J}S_j|\ge|J|$.

Hall's theorem supplies distinct representatives, one per column, forming an additional row with all $n$ symbols. This extends the rectangle without any column repetition. Repeat with $m+1$ rows, then successively until there are $n$ rows. Hence **every finite latin rectangle extends to a [Latin square](../../../../../latin-square.md)** by adding the required rows.

## ↑ Ancestors (13)

1. [V](../v.md)
2. [R2](../../r2.md)
3. [R](../../../r.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
