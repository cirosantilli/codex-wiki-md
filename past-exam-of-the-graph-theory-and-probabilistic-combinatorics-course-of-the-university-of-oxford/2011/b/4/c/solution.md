<h1 id="b/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The requested scale is $\boxed{k=\Theta(\sqrt{\log n})}$. To see its first-moment origin, the number $X_k$ of $k$-cliques has [expectation](../../../../../expected-value-split.md)

$$
\mathbb E X_k=\binom nk2^{-\binom k3}.
$$

For $k$ on the proposed scale, taking base-two [logarithms](../../../../../logarithm.md) gives

$$
\log_2\mathbb E X_k=k\log_2 n-\frac{k^3}6+O(k^2+k\log k).
$$

The leading terms balance at $k\approx\sqrt{6\log_2 n}$. In particular, for any fixed $c>\sqrt6$, taking $k$ near $c\sqrt{\log_2 n}$ makes the [expectation](../../../../../expected-value-split.md) tend to zero, so such [cliques](../../../../../clique-graph-theory.md) are absent with [probability](../../../../../probability.md) tending to one.

Thus the first-moment estimate places the largest-clique scale at a [constant](../../../../../constant-mathematics.md) multiple of $\sqrt{\log n}$, as requested. A diverging [expectation](../../../../../expected-value-split.md) below that balance does not itself prove existence; a corresponding probabilistic lower-bound proof would require an additional argument and is not part of the requested first-moment estimate.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
