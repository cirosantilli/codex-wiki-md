# Edit distance

↑ **Parent:** [Dynamic programming](dynamic-programming.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Edit_distance)

An [edit distance](edit-distance.md) is the minimum cost of allowed edits transforming one finite sequence into another. With unit insertion, deletion and substitution costs, the prefix table has boundaries $D[i,0]=i$, $D[0,j]=j$ and recurrence $D[i,j]=\min(D[i-1,j]+1,D[i,j-1]+1,D[i-1,j-1]+[x_i\ne y_j])$. The last alignment action gives one of these cases; appending that action to an optimal shorter alignment proves the converse inequality. Thus [induction](mathematical-induction.md) proves the recurrence, yielding $O(mn)$ [running time](running-time.md) for nonempty input lengths $m,n$. Two rolling rows suffice when only the distance is required; retaining predecessor actions supports reconstruction.

## ↑ Ancestors (5)

1. [Dynamic programming](dynamic-programming.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Edit distance](edit-distance.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms/7/a/solution.md)
