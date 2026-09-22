<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**The factorization-based version should produce the later outputs faster in this cost model.** For an input $m$, it performs at most $O(\sqrt m)$ trial-factor tests and $O(\log m)$ successful divisions, because each successful division removes a factor at least two. The square test uses multiplication, so it does not introduce an extra division on every loop test.

Across all candidates through $n$, the number of costly division or remainder operations is therefore at most

$$
O\!\left(\sum_{m=1}^{n}(\sqrt m+\log m)\right)=O(n^{3/2}+n\log n),
$$

compared with $\Theta(n^2)$ remainder operations for the straightforward routine. Small cases can still be affected by constant overhead; the conclusion concerns the growing enumeration workload, not a promise that every single call is faster.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [1](../../1.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
