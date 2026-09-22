<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A useful [local search](../../../../../local-search.md) state is any occupied-square [subset](../../../../../subset.md) $S\subseteq Q$, allowing temporary attacks. Let $C(S)$ count unordered attacking pairs and $N=n^2$. Maximize

$$
\boxed{F(S)=|S|-(N+1)C(S).}
$$

ACTIONS can offer insertion at an empty square, deletion of an occupied square, and relocation of one knight to an empty square. RESULT is respectively $S\cup\{q\}$, $S\setminus\{p\}$, and $(S\setminus\{p\})\cup\{q\}$. Insertions and deletions alone connect the whole [state space](../../../../../state-space.md); relocation is a useful additional proposal.

Every conflicting state has $F(S)\leq N-(N+1)<0$, whereas the empty board has score zero. Every conflict-free state has score exactly its knight count. Hence **every global maximizer is a maximum-size nonattacking placement**. If a knight participates in $r\geq1$ conflicts, deleting it changes the score by $-1+(N+1)r>0$, so a positive-conflict local stopping point cannot persist when improving deletions are considered.

From a random board, choose score-improving moves, with random restarts or occasional non-improving proposals to escape poor conflict-free local optima. A maximal placement is not necessarily a maximum placement: accepting only legal insertions can get stuck too early. This [objective function](../../../../../objective-function.md) defines the intended optimization precisely; a finite heuristic run still gives no general global-optimality certificate.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
