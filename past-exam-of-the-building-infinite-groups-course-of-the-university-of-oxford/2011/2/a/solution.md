<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $|g|_S$ be the least length of a word in $S\cup S^{-1}$ representing $g$, and write $B_S(r)=\{g:|g|_S\le r\}$. [Polynomial growth of a group](../../../../polynomial-growth-of-a-group.md) of degree at most $d$ means that, for some constant $C$, 

$$
|B_S(r)|\le C(1+r)^d\qquad(r\ge0).
$$

In particular these balls are finite. For the usual convention $S$ is finite; finiteness of $B_S(1)$ would force that in any case.

For a finite subset $T$, set $L=\max(1,\max_{t\in T}|t|_S)$. Replacing each letter of a $T$-word by an $S$-word gives

$$
B_T(r)\subseteq B_S(Lr).
$$

Thus $|B_T(r)|\le C(1+Lr)^d\le CL^d(1+r)^d$. This proves the same degree bound for $\langle T\rangle$. If $T$ is empty the [subgroup](../../../../subgroup.md) is trivial and the assertion is immediate.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the building infinite groups course of the University of Oxford](../../../split.md)
5. [Building infinite groups course of the University of Oxford](../../../../building-infinite-groups-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
