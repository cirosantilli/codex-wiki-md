<h1 id="b/7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Every vertex in the component can be reached from $v$ by a simple path. The number of potential length-$\ell$ simple paths beginning at $v$ is at most $n^\ell$, and each has probability $(1/(2n))^\ell$ of being present. Counting such paths may count a vertex more than once, so it gives an upper bound on the expected number of reached vertices:

$$
E|C(v)|\le\sum_{\ell=0}^{n-1}n^\ell(1/(2n))^\ell\le\sum_{\ell\ge0}2^{-\ell}=2.
$$

Thus $\boxed{K=2}$ works for every $n$. Equivalently the dominating [branching process](../../../../../branching-process.md) has mean offspring one half and expected [total progeny](../../../../../total-progeny-of-a-branching-process.md) two.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
