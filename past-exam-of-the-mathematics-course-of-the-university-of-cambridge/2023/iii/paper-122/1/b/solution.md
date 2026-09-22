<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $X$ count the [triangles](../../../../../../triangle-in-a-graph.md) of the [binomial random graph](../../../../../../binomial-random-graph.md) $G(n,p)$. Then

$$
\mu=\mathbb EX=\binom n3p^3=\Theta(n^3p^3).
$$

Two distinct triangle indicators are dependent only when the triangles share an edge. Hence their ordered [Janson dependency sum](../../../../../../janson-dependency-sum.md) is

$$
\Delta=\Theta(n^4p^5).
$$

If $0<p\leq n^{-1/2}$, then $\Delta=O(\mu)$. The first [Janson inequality](../../../../../../janson-inequality.md) gives

$$
\mathbb P(X=0)\leq e^{-\Omega(\mu)}.
$$

For the reverse bound, the events that individual triangles are absent are decreasing, so [Harris' inequality](../../../../../../harris-inequality.md) gives

$$
\mathbb P(X=0)
\geq(1-p^3)^{\binom n3}
=e^{-O(n^3p^3)},
$$

where $p<1/2$ keeps the logarithmic estimate uniform. Thus the probability is $e^{-\Theta(p^3n^3)}$.

If $n^{-1/2}\leq p<1/2$, the extended Janson bound gives

$$
\mathbb P(X=0)
\leq
\exp\left(-\Omega\left(\frac{\mu^2}{\Delta}\right)\right)
=e^{-\Omega(pn^2)}.
$$

For a lower bound, fix a balanced bipartition of the vertices and require every edge inside either part to be absent. The resulting graph is [bipartite](../../../../../../bipartite-graph.md), hence [triangle-free](../../../../../../triangle-free-graph.md), and this event has probability

$$
(1-p)^{2\binom{\lfloor n/2\rfloor}{2}}
=e^{-O(pn^2)}.
$$

Combining the bounds proves the second regime.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
