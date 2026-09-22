<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

This is [Ladner's theorem](../../../../../../ladner-s-theorem.md). Assume $\mathbf P\ne\mathbf{NP}$ and let $S$ be the [Boolean satisfiability problem](../../../../../../boolean-satisfiability-problem.md). Enumerate all clocked polynomial-time deterministic machines as $D_0,D_1,\ldots$ and all clocked polynomial-time candidate reductions as $R_0,R_1,\ldots$. A standard delayed-diagonalization schedule gives a nondecreasing, unbounded, polynomial-time computable function $s:\mathbb N\to\mathbb N$ that increases only by one. Define

$$
L=\{x\in S:s(|x|)\text{ is even}\}.
$$

The schedule alternates two requirements. At even stage $2j$, it holds $s$ fixed while searching successively larger finite sets of strings for an $x$ on which $D_j(x)$ disagrees with membership in $L$; after finding one it increments $s$. At odd stage $2j+1$, it searches for an $x$ such that

$$
x\in S\quad\Longleftrightarrow\quad R_j(x)\notin L,
$$

and then increments $s$. Length and simulation budgets are increased slowly enough that each finite search is eventually exhaustive but computing $s(n)$ still takes polynomial time. This is achieved, for example, by permitting only $n$ simulation steps and searches on strings of logarithmic length before deciding $s(n+1)$.

Every stage must finish. If an even stage $2j$ remained forever, then $s$ would eventually be a fixed even number, so $L$ and $S$ would differ on only finitely many strings. If $D_j$ decided $L$, those finitely many exceptions could be hardwired to decide $S$ in [P](../../../../../../p-complexity.md), contradicting $\mathbf P\ne\mathbf{NP}$. If an odd stage $2j+1$ remained forever, then $s$ would eventually be odd and $L$ would be finite. A correct [polynomial-time many-one reduction](../../../../../../polynomial-time-many-one-reduction.md) $R_j$ from $S$ to $L$ would again put $S$ in P. Thus every $D_j$ fails to decide $L$, and every $R_j$ fails to reduce $S$ to $L$.

Finally, $L\in\mathbf{NP}$: compute $s(|x|)$ and, when it is even, use the usual polynomial-time certificate for satisfiability. Hence

$$
\boxed{L\in\mathbf{NP}\setminus\mathbf P
\quad\text{and}\quad L\text{ is not NP-complete}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
