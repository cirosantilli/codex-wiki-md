<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A set $R\subseteq V(G)$ is [$(s,k)$-rich](../../../../../../rich-set-in-a-graph.md) if every $s$-element subset of $R$ has at least $k$ common neighbours.

Choose $x_1,\ldots,x_t$ independently and uniformly from $V(G)$, with repetition, and put

$$
W=N(x_1)\cap\cdots\cap N(x_t).
$$

By convexity,

$$
\mathbb E|W|
=\sum_{v\in V(G)}\left(\frac{d(v)}n\right)^t
\ge n\left(\frac{2m}{n^2}\right)^t
=\frac{(2m)^t}{n^{2t-1}}.
$$

Let $Y$ count the $s$-subsets $S\subseteq W$ having fewer than $k$ common neighbours in $G$. For each such $S$,

$$
\mathbb P(S\subseteq W)
=\left(\frac{|N(S)|}{n}\right)^t
<\left(\frac kn\right)^t,
$$

and therefore

$$
\mathbb EY\le\binom ns\left(\frac kn\right)^t.
$$

Delete one vertex from every bad $s$-subset of $W$. The remaining set $R$ is $(s,k)$-rich and satisfies $|R|\ge|W|-Y$. The hypothesis gives

$$
\mathbb E(|W|-Y)\ge r,
$$

so some choice has $|R|\ge r$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 132](../../../paper-132-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
