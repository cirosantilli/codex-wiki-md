<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A set $R\subseteq V(G)$ is [$(s,k)$-rich](../../../../../../rich-set-in-a-graph.md) when every $s$-element subset of $R$ has at least $k$ common neighbours.

Choose $t$ vertices $x_1,\ldots,x_t$ independently and uniformly from $V(G)$, allowing repetitions, and let

$$
X=N(x_1)\cap\cdots\cap N(x_t).
$$

By [Jensen inequality](../../../../../../jensen-s-inequality.md) applied to the convex function $z\mapsto z^t$,

$$
\mathbb E|X|
=\sum_{v\in V(G)}\left(\frac{d(v)}n\right)^t
\geq n\left(\frac{2m}{n^2}\right)^t
=\frac{(2m)^t}{n^{2t-1}}.
$$

Let $Y$ count the $s$-subsets $S\subseteq X$ having fewer than $k$ common neighbours in $G$. For each such $S$, the probability that $S\subseteq X$ is

$$
\left(\frac{|N(S)|}{n}\right)^t<\left(\frac kn\right)^t,
$$

so

$$
\mathbb EY\leq\binom ns\left(\frac kn\right)^t.
$$

The assumed inequality gives $\mathbb E(|X|-Y)\geq r$, so some choice has $|X|-Y\geq r$. Delete one vertex from each bad $s$-subset of $X$. The remaining set $R$ has size at least $|X|-Y\geq r$ and contains no bad $s$-subset, so it is $(s,k)$-rich. This is the basic [dependent random choice](../../../../../../dependent-random-choice.md) argument.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
