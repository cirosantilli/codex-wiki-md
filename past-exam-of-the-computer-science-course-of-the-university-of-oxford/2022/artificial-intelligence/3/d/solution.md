<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $F\subseteq\{1,\ldots,N\}^2$ for the prescribed occupied cells, with $k=|F|$. The source’s lowercase $n$ in its coordinate bound is read as the stated board size $N$. If two prescribed queens already attack each other, no completion exists. Each model below correctly expresses that impossibility as well as consistent inputs.

**Model 1: one [Boolean variable](../../../../../boolean-variable.md) per cell.** Let $B_{rc}\in\{0,1\}$ indicate occupancy. Require

$$
\sum_{r=1}^N\sum_{c=1}^N B_{rc}=N,\qquad B_{rc}=1\quad((r,c)\in F),
$$

and impose $B_{rc}+B_{st}\le1$ for every two distinct cells sharing a row, a column or a diagonal. Equivalently, impose exactly one queen in each row and column and at most one on each diagonal. Explicit diagonal constraints are

$$
\sum_{r-c=d}B_{rc}\le1\quad(-(N-1)\le d\le N-1),\qquad
\sum_{r+c=u}B_{rc}\le1\quad(2\le u\le2N).
$$

Together with the total-count constraint and the attacking-pair [binary constraints](../../../../../binary-constraint.md), these force exactly the intended boards. The count and diagonal-sum constraints are legitimate many-variable constraints; this model need not be binary.

**Model 2: one variable per labeled queen.** Let $Q_i=(R_i,C_i)\in\{1,\ldots,N\}^2$ for $1\le i\le N$. Enumerate $F=\{f_1,\ldots,f_k\}$ and restrict $D_i=\{f_i\}$ for $i\le k$. For every $i<j$, impose the [binary constraint](../../../../../binary-constraint.md)

$$
R_i\ne R_j,\qquad C_i\ne C_j,\qquad |R_i-R_j|\ne|C_i-C_j|.
$$

There are exactly $N$ variables and distinct rows, so these are $N$ distinct queens. Labeling the prescribed queens does not lose a board completion: the queens are physically indistinguishable, and any completion can be labeled to give the prescribed ones those indices. It does create redundant assignments for the remaining labels.

**Model 3: one variable per row.** Let $C_r\in\{1,\ldots,N\}$ be the queen’s column in row $r$. For every $r<s$, require

$$
C_r\ne C_s,\qquad |C_r-C_s|\ne s-r,
$$

and impose $C_r=c$ for every $(r,c)\in F$. These restrictions give $N$ queens, one per row; the [all-different constraint](../../../../../all-different-constraint.md) on the columns gives one per column. For $N$ nonattacking queens on $N$ rows, exactly one per row is forced by the [pigeonhole principle](../../../../../pigeonhole-principle.md), so no solutions are lost. Inconsistent prescribed positions in a single row give incompatible unary restrictions. All three are exact [constraint satisfaction problem](../../../../../constraint-satisfaction-problem.md) encodings of the [queens completion problem](../../../../../queens-completion-problem.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2022](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
