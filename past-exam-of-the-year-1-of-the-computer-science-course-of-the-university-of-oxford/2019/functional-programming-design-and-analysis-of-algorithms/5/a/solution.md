<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [divide-and-conquer algorithm](../../../../../divide-and-conquer-algorithm.md) handles a small input directly; otherwise it divides the input into smaller instances, recursively solves them, and combines their answers. With $a$ equally sized subproblems of size approximately $n/b$ and nonrecursive work $f(n)$, its [recurrence relation](../../../../../recurrence-relation.md) has the form $T(n)=aT(n/b)+f(n)$, with constant-size base cases, $a\ge1$ and $b>1$.

Write $p=\log_b a$. The basic [master theorem](../../../../../master-theorem.md) gives the following cases, with a fixed $\varepsilon>0$:

- If $f(n)=O(n^{p-\varepsilon})$, then **$T(n)=\Theta(n^p)$**.
- If $f(n)=\Theta(n^p)$, then **$T(n)=\Theta(n^p\log n)$**.
- If $f(n)=\Omega(n^{p+\varepsilon})$ and the regularity condition $af(n/b)\le cf(n)$ holds eventually for some $c<1$, then **$T(n)=\Theta(f(n))$**.

For the common extended middle case, $f(n)=\Theta(n^p\log^k n)$ with fixed $k\ge0$ gives $T(n)=\Theta(n^p\log^{k+1}n)$. A [recursion tree](../../../../../recursion-tree.md) explains the three cases: work is dominated by its leaves, spread across comparable levels, or dominated by its top levels. The regularity condition in the last case is part of the theorem, not an optional simplification.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
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
