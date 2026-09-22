<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The standard three-case [master theorem](../../../../../master-theorem.md) concerns

$$
T(n)=aT(n/b)+f(n),\qquad a\geq1,\quad b>1,
$$

with constant base-case cost and eventually nonnegative $f$. Put $d=\log_b a$.

- If $f(n)=O(n^{d-\epsilon})$ for some $\epsilon>0$, then $T(n)=\Theta(n^d)$.
- If $f(n)=\Theta(n^d)$, then $T(n)=\Theta(n^d\log n)$.
- If $f(n)=\Omega(n^{d+\epsilon})$ for some $\epsilon>0$ and $a f(n/b)\leq c f(n)$ eventually for a constant $c<1$, then $T(n)=\Theta(f(n))$.

In a [divide-and-conquer algorithm](../../../../../divide-and-conquer-algorithm.md), $a$ counts recursive subproblems, $n/b$ is their size, and $f$ accounts for splitting and combining. The comparison with $n^{\log_b a}$ identifies whether leaves, all levels, or the upper levels dominate the [running time](../../../../../running-time.md). The polynomial gap and the third case's regularity condition are part of this version of the theorem.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
