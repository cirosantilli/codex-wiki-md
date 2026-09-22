<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take a fresh [CSP event](../../../../../csp-event.md) $h$ and define

$$
\boxed{P=(h\to P)\setminus\{h\}.}
$$

The apparent guard is removed by [CSP hiding](../../../../../csp-hiding.md). Each unfolding can perform a [CSP internal action](../../../../../csp-internal-action.md) and return to the same situation without any visible [CSP event](../../../../../csp-event.md). Operationally this is an infinite internal loop, a [CSP divergence](../../../../../csp-divergence.md), so the equation is not a [guarded recursion](../../../../../guarded-recursion.md). This is precisely why a syntactic test that counts every occurrence of $\to$ would be wrong.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Concurrency](../../../concurrency-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
