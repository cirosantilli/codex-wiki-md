<h1 id="b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $X$ count the four-vertex sets spanning a [clique](../../../../../clique-graph-theory.md). Its expectation is $\mu=\binom n4p^6$. If $p\ll n^{-2/3}$, then $\mu\to0$ and [Markov's inequality](../../../../../markov-s-inequality.md) gives $P(X>0)\to0$.

Now suppose $p\gg n^{-2/3}$. Then $\mu\to\infty$. Two distinct [clique](../../../../../clique-graph-theory.md) indicators are independent unless their vertex sets share at least two vertices. An overlap of two vertices gives $O(n^6)$ ordered pairs requiring eleven distinct edges; an overlap of three gives $O(n^5)$ pairs requiring nine edges. Consequently

$$
D=O(n^6p^{11}+n^5p^9),\qquad
\frac D{\mu^2}=O(n^{-2}p^{-1}+n^{-3}p^{-3})\longrightarrow0.
$$

The preceding second-moment bound therefore gives $P(X=0)\to0$. Thus

$$
\boxed{p_*(n)=n^{-2/3}}
$$

is a threshold for the appearance of a four-[clique](../../../../../clique-graph-theory.md). Sharing just one vertex creates no dependence because the two edge sets are disjoint.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
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
