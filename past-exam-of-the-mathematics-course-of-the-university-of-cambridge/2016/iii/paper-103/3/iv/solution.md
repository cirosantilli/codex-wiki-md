<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

We verify all three [content vector of a standard Young tableau](../../../../../../content-vector-of-a-standard-young-tableau.md) conditions using the spectral rules proved in part (i).

The first coordinate is zero by part (ii). For the neighbour condition, suppose some $a_j$ has neither $a_j-1$ nor $a_j+1$ among earlier coordinates. Try moving $a_j$ successively to the left. Each encountered difference is not $\pm1$; if it is zero, we have an impossible adjacent equality, while otherwise the local spectral rule permits the swap. If $a_j=0$, this procedure must encounter the original first coordinate $0$ and give that contradiction. If $a_j\ne0$, it moves $a_j$ to the first position, contradicting $X_1=0$. Therefore an earlier neighbour always exists. Starting from $a_1=0$, this also proves inductively that every coordinate is an integer.

For the repeated-value condition, suppose it fails and choose a failing pair of equal coordinates $a$ with the shortest interval. There is no intervening $a$, since a shorter pair would then also fail. There must be at least one intervening neighbour: otherwise the right-hand $a$ could be moved next to the left-hand $a$ by admissible swaps. Suppose, for example, that $a+1$ is missing. There cannot be two occurrences of $a-1$ in the interval: between them the required neighbour $a$ is missing, producing a shorter failing pair. Thus there is exactly one $a-1$. All other intervening values differ from $a$ by more than $1$, so the two copies of $a$ can be moved towards that unique neighbour until the forbidden consecutive pattern $(a,a-1,a)$ appears. Part (i) excludes it. The case in which $a-1$ is missing is identical, using $(a,a+1,a)$. Both neighbours must therefore occur.

For completeness, these conditions really encode [standard Young tableaux](../../../../../../standard-young-tableau.md). If $a$ occurs for the $r$th time, place the next label in

$$
\begin{cases}
(r,r+a),&a\geq0,\\
(r-a,r),&a<0.
\end{cases}
$$

This is the next unfilled cell on diagonal of content $a$. On the first occurrence of a positive diagonal, the earlier-neighbour condition forces its first left predecessor to exist: earlier diagonal values form an interval containing $0$, so a first positive $a$ can only be reached through $a-1$. The negative case uses the predecessor above. On later occurrences, the two neighbours appearing since the previous occurrence ensure that the new cell's left and upper predecessors have already been filled. For diagonal $0$, the same two-neighbour condition supplies both predecessors after the first box. Thus each addition is an [addable node of a Young diagram](../../../../../../addable-node-of-a-young-diagram.md), and the labels form a [standard Young tableau](../../../../../../standard-young-tableau.md).

Conversely, a [standard Young tableau](../../../../../../standard-young-tableau.md) starts at $(1,1)$; any later cell has a left or upper predecessor of neighbouring content. Two cells on one diagonal have the cells immediately to the right and below the earlier one between them in the tableau order, supplying both neighbours. Hence its [content vector of a standard Young tableau](../../../../../../content-vector-of-a-standard-young-tableau.md) satisfies precisely the stated conditions. The next position on a diagonal is unique, so this construction is a [bijection](../../../../../../bijection.md) between [content vectors of standard Young tableaux](../../../../../../content-vector-of-a-standard-young-tableau.md) and [standard Young tableaux](../../../../../../standard-young-tableau.md).

We have now proved **$\boxed{\operatorname{Spec}(n)\subseteq\operatorname{Cont}(n)}$** without assuming the desired spectrum identification.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
