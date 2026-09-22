<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**The second procedure should reach large outputs faster**, because the first makes exactly $n$ expensive `MOD` operations when processing argument $n$, whereas the second tries only up to the [square root](../../../../../square-root.md) of a shrinking residual, with at most $\lfloor\log_2 n\rfloor$ successful `DIV` operations. Each successful division also requires a successful `MOD` test; each outer iteration adds one final unsuccessful `MOD` test. Thus its expensive-operation count is $O(\sqrt n+\log n)$ per argument, and at most $O(n^{3/2})$ cumulatively through argument $n$, compared with $\Theta(n^2)$ for direct counting.

The speedup is not an assertion that every single call uses fewer divisions: for $n=4$, the second code makes three `MOD` tests and two `DIV` operations, while the first makes four `MOD` tests. Small constant costs can go either way. The many small [prime factors](../../../../../prime-factor.md) in [highly composite numbers](../../../../../highly-composite-number.md) also shrink the residual early, which often helps further; the cumulative comparison includes every preceding argument, not only the printed records.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [2](../../2.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
