<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use unit-cost insertion, deletion and substitution of one symbol. Their minimum total cost is the [edit distance](../../../../../edit-distance.md). Let $D[i,j]$ be the [edit distance](../../../../../edit-distance.md) between the first $i$ symbols of the first sequence and the first $j$ of the second. Initialize $D[i,0]=i$ and $D[0,j]=j$. For $i,j>0$ compute

$$
D[i,j]=\min\left\{D[i-1,j]+1,\ D[i,j-1]+1,\ D[i-1,j-1]+[x_i\ne y_j]\right\}.
$$

The cases delete the final source symbol, insert the final target symbol, or align the two final symbols, paying one for substitution and zero for a match. Every optimal alignment ends in one of these cases, and each case extends a valid shorter alignment. [Induction](../../../../../mathematical-induction.md) on $i+j$ proves the [dynamic programming](../../../../../dynamic-programming.md) recurrence correct.

Fill rows or columns in increasing order so every dependency is already available. There are $(m+1)(n+1)$ entries with constant work per interior entry: **$O(mn)$ [running time](../../../../../running-time.md)** for nonempty sequences, or $O((m+1)(n+1))$ including the boundary cases. The full table has [space complexity](../../../../../space-complexity.md) $O(mn)$; two rows give $O(n)$ [auxiliary space](../../../../../auxiliary-space.md) when only the distance is wanted. Predecessor choices in the full table recover an optimal edit sequence.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
