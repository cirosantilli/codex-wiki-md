<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We prove the [locally dense graph thinning lemma](../../../../../../locally-dense-graph-thinning-lemma.md). Fix an integer $m>8/\varepsilon$ and then choose $\delta<1/(3m)$. Partition the vertex set equitably as $V_1\sqcup\cdots\sqcup V_m$. For sufficiently large $n$, every part has at least $\delta n$ vertices. Consequently every pair $V_i,V_j$ has density

$$
d_{ij}=\frac{e_G(V_i,V_j)}{|V_i||V_j|}\geq p.
$$

Delete all edges within parts. For each edge of $G$ joining $V_i$ to $V_j$, retain it independently with probability $p/d_{ij}$.

For fixed disjoint $A,B$, writing $A_i=A\cap V_i$ and $B_i=B\cap V_i$ gives

$$
\mathbb E e_{G'}(A,B)
=p\sum_{i\ne j}|A_i||B_j|.
$$

The omitted diagonal contribution satisfies

$$
p\sum_i|A_i||B_i|
\leq\frac14\sum_i|V_i|^2
<\frac{n^2}{2m}
<\frac{\varepsilon n^2}{4}.
$$

The retained-edge indicators are independent. The [exponential Markov bound](../../../../../../exponential-markov-bound.md) therefore gives, for each fixed $(A,B)$,

$$
\mathbb P\left(
|e_{G'}(A,B)-\mathbb Ee_{G'}(A,B)|>\frac{\varepsilon n^2}{2}
\right)
\leq2e^{-c\varepsilon^2n^2}.
$$

There are at most $3^n$ ordered pairs of disjoint vertex sets. A [union bound](../../../../../../boole-s-inequality.md) shows that, with positive probability, no pair violates this estimate. For that realization,

$$
|e_{G'}(A,B)-p|A||B||\leq\varepsilon n^2
$$

simultaneously for all disjoint $A,B$. As usual for a dense asymptotic statement, $n$ is taken sufficiently large; a lower-order integrality error is unavoidable for bounded $n$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
