<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Explore the [connected component of a graph](../../../../../../component-graph-theory.md) containing a fixed vertex $v$ by [Breadth-first search](../../../../../../breadth-first-search.md). If the exploration discovers at least $m$ vertices, then before its $m$th discovery at least $m-1$ of at most $mn$ tested potential edges must be present. The tests are independent Bernoulli trials with parameter $p=(1-\varepsilon)/n$, so

$$
\mathbb P(|C(v)|\geq m)
\leq
\mathbb P(\operatorname{Bin}(mn,p)\geq m-1).
$$

The [binomial distribution](../../../../../../binomial-distribution.md) on the right has mean $(1-\varepsilon)m$. For $m\geq2/\varepsilon$, the [exponential Markov bound](../../../../../../exponential-markov-bound.md) gives

$$
\mathbb P(|C(v)|\geq m)\leq e^{-c\varepsilon^2m}
$$

for an absolute constant $c>0$. The [union bound](../../../../../../boole-s-inequality.md) over the $n$ choices of $v$ now gives

$$
\mathbb P\left(\max_v|C(v)|\geq m\right)
\leq ne^{-c\varepsilon^2m}.
$$

Taking $m=C_\varepsilon\log n$ with $C_\varepsilon>2/(c\varepsilon^2)$ makes this probability tend to zero. This proves the [subcritical component bound for a binomial random graph](../../../../../../subcritical-component-bound-for-a-binomial-random-graph.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
