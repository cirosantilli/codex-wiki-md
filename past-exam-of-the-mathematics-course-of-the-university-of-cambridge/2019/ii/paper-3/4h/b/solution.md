<h1 id="4h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [CYK algorithm](../../../../../../cyk-algorithm.md). For a nonempty input word $v=v_1\cdots v_n$, let $T_{i,j}$ be the set of nonterminals that derive the substring $v_i\cdots v_j$. Initialize

$$
T_{i,i}=\{A:A\to v_i\text{ is a production}\}.
$$

For increasing substring lengths, compute

$$
T_{i,j}=\bigcup_{k=i}^{j-1}
\{A:A\to BC,\ B\in T_{i,k},\ C\in T_{k+1,j}\}.
$$

Accept exactly when the start symbol belongs to $T_{1,n}$. The proof is a [mathematical induction](../../../../../../mathematical-induction.md) on substring length: a one-letter derivation uses a terminal production, while every longer [parse tree](../../../../../../parse-tree.md) has a root production $A\to BC$ whose two subtrees yield two adjacent nonempty substrings. The recurrence considers every possible split point and therefore finds exactly all possible roots. For a fixed grammar the algorithm uses $O(n^3)$ time. Under the strict form in part (a), it rejects $\epsilon$ immediately.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4H](../../4h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
