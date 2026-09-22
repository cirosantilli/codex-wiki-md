<h1 id="strassen-s-algorithm">Strassen's algorithm</h1>

↑ **Parent:** [Matrix multiplication](matrix-multiplication.md)

The [matrix multiplication](matrix-multiplication.md) algorithm of [Volker Strassen](volker-strassen.md) using seven half-size block products and quadratically many scalar additions per recursion level. Its recurrence is $T(n)=7T(n/2)+\Theta(n^2)$, giving $\Theta(n^{\log_2 7})$ arithmetic operations by the [Master theorem](master-theorem.md).[ACM SIGACT, 2008 Knuth Prize citation, the 1969 matrix-multiplication contribution](https://staging.sigact.hosting.acm.org/prizes/knuth/2008.html)

## ↑ Ancestors (9)

1. [Matrix multiplication](matrix-multiplication.md)
2. [Matrix](matrix.md)
3. [Linear map](linear-map.md)
4. [Vector space](vector-space-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/functional-programming-design-and-analysis-of-algorithms/8/b/solution.md)
- [Volker Strassen](volker-strassen.md)
